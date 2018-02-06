# datePicker
//datePicker日期控件 v1.0

var calendar = new datePicker();
calendar.init({
    'trigger': '#demo1', /*选择器，触发弹出插件*/
    'type': 'date',/*date 调出日期选择 datetime 调出日期时间选择 time 调出时间选择 ym 调出年月选择*/
    'minDate':'1900-1-1',/*最小日期*/
    'maxDate':new Date().getFullYear()+'-'+(new Date().getMonth()+1)+'-'+new Date().getDate(),/*最大日期*/
    'onSubmit':function(){/*确认时触发事件*/
        var theSelectData=calendar.value;
    },
    'onClose':function(){/*取消时触发事件*/
    }
});
