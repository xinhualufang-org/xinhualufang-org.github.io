>“本文为原创文章，会经常更新知识点以及修正一些错误，因此转载请保留原出处，方便溯源，避免陈旧错误知识的误导，同时有更好的阅读体验。” --[张鑫旭](http://www.zhangxinxu.com/)<br>
:octocat:此标记为需要去实践验证后修改或本人目前不懂的知识点，希望读者一起完善。

# $ionicModal

    modal是一个内容窗格，可以临时越过用户的主视图。通常被用来选择或编辑一个条目，需要将modal的内容放到<ion-modal-view>中。
    
##### [DEMO1点击查看](http://xinhualufang-org.github.io/ionic/Components-Modal/demo1.html)

##### [DEMO2点击查看](http://xinhualufang-org.github.io/ionic/Components-Modal/demo2.html)

###方法

* **fromTemplate(templateString, options)**
    * **templateString**，string类型，html字符串作为modal的内容；
    * **options**
        ```
            {
                scope: $scope,
                animation: "slide-in-up",
                focusFirstInput: false,
                backdropClickToClose: true,
                hardwareBackButtonClose
            }
        ```
        
        * scope，`{object}`。:octocat:不知道这个参数有什么作用
        * animation，`{string}`。modal显示和隐藏的动画，缺省值为`slide-in-up`。:octocat:其他动画需要自己实现，怎么实现未尝试
        * focusFirstInput，`{boolean}`。Modal显示的时候modal的第一个input是否自动获取焦点，IOS中会显示键盘，在Android中需要使用keyboard插件强制显示键盘，缺省值为`false`。
        * backdropClickToClose，`{boolean}`。当点击modal之外时是否关闭modal，缺省值为`true`。
        * hardwareBackButtonClose，{boolean}。在Andoird或类似设备上点击物理返回时，modal是否能够被关闭，缺省值为`true`。
    
* **fromTemplateUrl(templateUrl, options)**


    Cannot call modal.show() after remove(). Please create a new modal instance.
