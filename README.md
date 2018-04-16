# javaScript
js，jQuery 常用代码

var winHeight = $(window).height();   //获取当前页面高度
$(window).resize(function(){
   var thisHeight=$(this).height();
    if(winHeight - thisHeight >50){
         //当软键盘弹出，在这里面操作
    $(".footer").css("position","static")
    }else{
        //当软键盘收起，在此处操作
   $(".footer").css("position","absolute")
    }
});
