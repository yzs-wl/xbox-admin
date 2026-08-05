var expense = $data.findById('expense\_detail', 1);
data.remark = expense.remark;



// 查询其他模型的单条数据
var order = $data.findById('order', 1001);
data.customerName = order.customerName;



// 按条件查询
var customer = $data.findOne('customer', {code: data.customerCode});
data.customerLevel = customer ? customer.level : 'normal';



// 查询列表
var items = $data.findList('order\_item', {orderId: data.id});
var totalAmount = 0;
for (var i = 0; i < items.length; i++) {
totalAmount += items\[i].amount;
}
data.totalAmount = totalAmount;



// 分页查询
var page = $data.findPage('product', {category: 'A'}, 1, 20);
// page.content = 数据列表, page.total = 总记录数



// 统计数量
var count = $data.count('order', {status: 'pending'});

// 跨模型新增数据
$data.save('log', {action: 'update', targetId: data.id, operator: 'system'});



// 跨模型删除数据
$data.delete('temp\_data', 999);



// 在服务脚本中调用其他服务

var r = $service.invoke({ key: "sv\_expense\_detail\_add", params: { /\* ... \*/ } });



// 模型按钮绑定（extensionConfig）

// { "position": "toolbar", "label": "ccc", "type": "service", "serviceKey": "sv\_expense\_detail\_add", "params": { "id": "${row.id}" } }

