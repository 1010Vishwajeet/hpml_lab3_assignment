## C++ Chatbot using Pytorch C++ (LibTorch) and Torchscript model

**File Name:** nonPython_chatbot.cc

## Code Details:
**Classes:**\
class Voc => Vocabulary Class to store and build word/index map. \
class Utils => Helper class to process strings and dataset. \
class TorchModel => Interface for accessing loaded model.

main() method => Chatbot using above classes


## How to Run:

**Step 1:** **Building:**\
Within the directory where nonPython_chatbot.cc and CMakeLists.txt are present, run following commands:
```
cmake -DCMAKE_PREFIX_PATH=/path/to/libtorch
cmake --build . --config Release
```
For example:
```
cmake -DCMAKE_PREFIX_PATH="/root/snap/HPML/libtorch"
cmake --build . --config Release
```

**Step 2:** **Run**:\
Run executable file with following command:
```
./nonPython_chatbot <path/to/scripted_chatbot_cpu.pt> <path/to/vocab.csv>
```
For example (if all files are in same directory):
```
./nonPython_chatbot scripted_chatbot_cpu.pt vocab.csv
```
OR
```
 ./nonPython_chatbot "/root/snap/HPML/Lab3/scripted_chatbot_cpu.pt" "/root/snap/HPML/Lab3/vocab.csv"
```






