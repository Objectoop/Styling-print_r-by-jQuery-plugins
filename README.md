print_r function in javascript (like print_r in PHP)

jquery plugins

Example :
<pre>
&lt;script&gt;
$(document).ready(function(){
	var ar = [0,1,2,3,4,5,[123,13,[3,3,3],{"a":1,"c":[1,2,3]}]];
	$(".console-area").print_r(ar);
});

&lt;/script&gt;

&lt;div class="console-area"&gt;&lt;/div&gt;
</pre>
Output :
<pre>
Array 
(
    [0] => 0
    [1] => 1
    [2] => 2
    [3] => 3
    [4] => 4
    [5] => 5
    [6] => Array 
            (
                [0] => 123
                [1] => 13
                [2] => Array 
                        (
                            [0] => 3
                            [1] => 3
                            [2] => 3
                        )
                [3] => Object 
                        (
                            [a] => 1
                            [c] => Array 
                                    (
                                        [0] => 1
                                        [1] => 2
                                        [2] => 3
                                    )
                        )
            )
)
</pre>