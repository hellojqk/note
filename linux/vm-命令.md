#多行输出path项
path=$PATH;echo -e ${path//:/\\n}

[Ctrl] + [f]	萤幕『向下』移动一页，相当于[Page Down]按键( 常用 )
[Ctrl] + [b]	萤幕『向上』移动一页，相当于[Page Up]按键( 常用 )
[Ctrl] + [d]	萤幕『向下』移动半页
[Ctrl] + [u]	萤幕『向上』移动半页


+	游标移动到非空白字元的下一列
-	游标移动到非空白字元的上一列
0   或功能键[Home]	这是数字『 0 』：移动到这一列的最前面字元处( 常用 )
$   或功能键[End]	移动到这一列的最后面字元处( 常用 )


H	游标移动到这个萤幕的最上方那一列的第一个字元
M	游标移动到这个萤幕的中央那一列的第一个字元
L	游标移动到这个萤幕的最下方那一列的第一个字元
G	移动到这个档案的最后一列( 常用 )


nG	n 为数字。移动到这个档案的第n 列。例如20G 则会移动到这个档案的第20 列(可配合:set nu)
gg	移动到这个档案的第一列，相当于1G啊！( 常用 )
n<Enter>	n为数字。游标向下移动n列( 常用 )

/word	向游标之下寻找一个名称为word的字串。例如要在档案内搜寻vbird这个字串，就输入/vbird即可！( 常用 )
?word	向游标之上寻找一个字串名称为word 的字串。
n	这个n是英文按键。代表『重复前一个搜寻的动作』。举例来说，如果刚刚我们执行/vbird去向下搜寻vbird这个字串，则按下n后，会向下继续搜寻下一个名称为vbird的字串。如果是执行?vbird的话，那么按下n则会向上继续搜寻名称为vbird的字串！
N	这个N 是英文按键。与n 刚好相反，为『反向』进行前一个搜寻动作。例如/vbird 后，按下N 则表示『向上』搜寻vbird 。
使用/word 配合n 及N 是非常有帮助的！可以让你重复的找到一些你搜寻的关键字！
:n1,n2s/word1/word2/g	n1与n2为数字。在第n1与n2列之间寻找word1这个字串，并将该字串取代为word2 ！举例来说，在100到200列之间搜寻vbird并取代为VBIRD则：
『:100,200s/vbird/VBIRD/g』。( 常用 )
:1,$s/word1/word2/g	从第一列到最后一列寻找word1字串，并将该字串取代为word2 ！( 常用 )
:1,$s/word1/word2/gc	从第一列到最后一列寻找word1字串，并将该字串取代为word2 ！且在取代前显示提示字元给使用者确认(confirm)是否需要取代！( 常用 )

