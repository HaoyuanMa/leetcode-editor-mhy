删除多余目录，为每道题目单独创建目录。

[原插件链接](https://github.com/shuzijun/leetcode-editor):
<https://github.com/shuzijun/leetcode-editor>


go模板

```
package main
import "fmt"

//${question.frontendQuestionId}.${question.title}.${question.titleSlug}

${question.code}

func main() {
    result := $!velocityTool.smallCamelCaseName(${question.titleSlug})()
    fmt.Println(result)
}
```


c++模板

```
\#include "iostream"
using namespace std;

//${question.frontendQuestionId}.${question.title}.${question.titleSlug}

${question.code}

int main(){
    cout << (new Solution()).$!velocityTool.smallCamelCaseName(${question.titleSlug})() << endl;
    return 0;
}
```
