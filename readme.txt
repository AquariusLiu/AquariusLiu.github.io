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

changes:
WRC-2533GHBK-1 -> WRC-2533GHBK-I
add WXR-1750DHP/Y
R8500-100JPS -> R8500
WMR-433W -> WMR-433W-BK
PA-WG2600HP2 -> WG2600HP2
PA-WG1800DP2 -> WG1800DP2
PA-WG1200HS -> WG1200HS