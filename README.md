#Wust rm 作业
##task1
```cpp
#include <iostream>
#include <yaml-cpp/yaml.h>

using namespace std;

int main() {
    try {
        // 读文件
        YAML::Node config = YAML::LoadFile("config.yaml");
        // 输入 a 和 b
        YAML::Node aNode = config["a"];
        YAML::Node bNode = config["b"];
        int a = aNode.as<int>();
        int b = bNode.as<int>();
        // 输出
        cout << "a+b = " << (a + b) << endl;
    } 
    catch (const YAML::BadFile& e) {
        cout << "找不到 config.yaml 文件" << endl;
    }
    catch (const YAML::Exception& e) {
        cout << "YAML 格式不对" << endl;
    }

    return 0;
}```
##task2
```bash
#!/bin/bash
echo "-----------------------------------------------"
echo "     肯         肯       德德德        基基基    "
echo "      肯       肯        德           基    基  "
echo "       肯     肯         德德德       基    基  "
echo "        肯   肯              德       基    基  "
echo "         肯 肯           德德德        基基基    "
echo "                                               "
echo "               疯狂星期四，V我50               "
echo "-----------------------------------------------"```