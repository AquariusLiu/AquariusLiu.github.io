Chrome 添加运行参数（具体怎么设置自己百度）： --args --disable-web-security --user-data-dir

例如：
"C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" --args --disable-web-security --user-data-dir --allow-running-insecure-content

然后打开 .html 就可以了

这个是初步的版本，先凑合用，之后我有空再改进

Mac
$ cd "/Applications/Google Chrome.app/Contents/MacOS"/
$ sudo mv "Google Chrome" Google.real
$ sudo printf '#!/bin/bash\ncd "/Applications/Google Chrome.app/Contents/MacOS"\n"/Applications/Google Chrome.app/Contents/MacOS/Google.real" --args --disable-web-security --user-data-dir --allow-running-insecure-content "$@"\n' > Google\ Chrome
$ sudo chmod u+x "Google Chrome"