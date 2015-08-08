# $ionicModal

    modal是一个内容窗格，可以临时越过用户的主视图。通常被用来选择或编辑一个条目，需要将modal的内容放到<ion-modal-view>中。
    
##### [DEMO1点击查看](http://xinhualufang-org.github.io/ionic/Components-Modal/demo1.html)

##### [DEMO2点击查看](http://xinhualufang-org.github.io/ionic/Components-Modal/demo2.html)

###方法

* **fromTemplate(templateString, options)**
    * templateString,string类型，html字符串作为modal的内容；
    * options
    ```
        {
            scope: $scope,
            animation: "slide-in-up",
            focusFirstInput: false,
            backdropClickToClose: true,
            hardwareBackButtonClose
        }
    ```
    
    * **scope**，{object}，:octocat:不知道这个参数有什么作用
    * **animation**，{string}，modal显示和隐藏的动画，缺省值为`slide-in-up`。:octocat:其他动画需要自己实现，怎么实现未尝试
    


* **fromTemplateUrl(templateUrl, options)**


    Cannot call modal.show() after remove(). Please create a new modal instance.
