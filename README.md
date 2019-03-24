
# Datetime
简单全面好用的日期时间插件


## 1.通过id使用 ##
HTML代码
       

    <h3>日期时间选择器</h3>
    <input type="text" value="" id="datetimepicker"/><br><br>
      
js代码

   
        $('#datetimepicker').datetimepicker({
        dayOfWeekStart : 1,
        lang:'en',
        disabledDates:['1996/01/08','1996/01/09','1996/01/10'],
        startDate:	'1996/01/05'
        });
        $('#datetimepicker').datetimepicker({value:'2019/03/24 05:03',step:10});
        
      

## 2.通过class使用 ##
HTML代码

      <h3>通过Class使用</h3>
	<input type="text" class="some_class" value="" id="some_class_1"/></br>
   
js代码

   
    $('.some_class').datetimepicker();
 
## 3.只有时间 ##
HTML代码
     

          
    <h3>只有时间</h3>
    		<input type="text" id="datetimepicker1"/><br><br></br>


js代码
    

      $('#datetimepicker1').datetimepicker({
    	datepicker:false,
    	format:'H:i',
    	step:5
        });

## 4.带有按钮 ##	
HTML代码

    <h3>带按钮的</h3>
    <input type="text" value="2016/12/03 18:00" id="datetimepicker4"/>
    <input id="open" type="button" value="open"/>
    <input id="close" type="button" value="close"/>
    <input id="reset" type="button" value="reset"/>

js代码	
  

      $('#datetimepicker4').datetimepicker();
        $('#open').click(function(){
        	$('#datetimepicker4').datetimepicker('show');
        });
        $('#close').click(function(){
        	$('#datetimepicker4').datetimepicker('hide');
        });
        $('#reset').click(function(){
        	$('#datetimepicker4').datetimepicker('reset');
        });

## 5.黑色主题 ##
HTML代码
	

    <h3>黑色主题</h3>
    	 <input type="text" id="datetimepicker_dark"/>

js代码
   

     $('#datetimepicker_dark').datetimepicker({theme:'dark'})
        $('#datetimepicker_dark').datetimepicker({
        dayOfWeekStart : 1,
        lang:'en',
        disabledDates:['1996/01/08','1996/01/09','1996/01/10'],
        startDate:	'1996/01/05'
        });
        $('#datetimepicker_dark').datetimepicker({value:'2019/03/25 05:03',step:1});
