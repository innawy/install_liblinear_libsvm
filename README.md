# Install liblinear and libsvm on iOS with anaconda3

### libsvm 

1. Download libsvm-3.24.tar.gz file from https://www.csie.ntu.edu.tw/~cjlin/libsvm/ 
2. Unzip the .tar file in Terminal: $ tar xzvf libsvm-3.24.tar.gz 
3. Run $ make in both of the directories below: libsvm-3.24 and libsvm-3.24/python
4. Move the folder libsvm-3.24 to usr/local/lib
5. Copy svm.py, svmutil.py, and commonutil.py from libsvm-3.24/python to anaconda3/lib/python3.7
6. Copy libsvm.so.2 from libsvm-3.24 to anaconda3/lib

### liblinear 
1. Download liblinear-2.30.tar.gz file from https://www.csie.ntu.edu.tw/~cjlin/liblinear/
2. Unzip the .tar file in Terminal: $ tar xzvf liblinear-2.30.tar.gz
3. Run $ make in both of the directories below: liblinear-2.30 and liblinear-2.30/python
4. Move the folder liblinear-2.30 to the same directory of Jupyter Notebook, rename as liblinear_local
5. When import package, use: from liblinear_local.python.liblinearutil import *


Source:
Chih-Chung Chang and Chih-Jen Lin, LIBSVM : a library for support
vector machines. ACM Transactions on Intelligent Systems and
Technology, 2:27:1--27:27, 2011. Software available at
http://www.csie.ntu.edu.tw/~cjlin/libsvm
