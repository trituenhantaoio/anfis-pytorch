# ANFIS in pyTorch #


Đây là cài đặt của hệ ANFIS sử dụng pyTorch.


### ANFIS

ANFIS là cách biểu diễn hệ logic mờ (FIS) như một chuối
các tầng số để có thể huấn luyện như một mạng nơ ron.

Bài báo gốc có thể xem tại
[Jyh-Shing Roger Jang](http://mirlab.org/jang/):

* Jang, J.-S.R. (1993). "ANFIS: adaptive-network-based fuzzy inference
  system". IEEE Transactions on Systems, Man and Cybernetics. 23 (3):
  665–685. doi:10.1109/21.256541

Chú ý rằng, nó dựa trên Giải mờ theo phong cách Takagi Sugeno Kang (TSK) hơn là Mamdani.


### Các cài đặt khác

Code C gốc của Jang cài đặt hệ ANFIS cùng với test case được lưu trữ
[tại đây](https://www.cs.cmu.edu/Groups/AI/areas/fuzzy/systems/anfis/).

Phiên bản nhiều người sử dụng là
[ANFIS library for Matlab](https://www.mathworks.com/help/fuzzy/anfis.html).
[Tài liệu của họ](https://www.mathworks.com/help/fuzzy/neuro-adaptive-learning-and-anfis.html) khá hữu ích để hiểu cách ANFIS hoạt động, dù có dùng Matlab hay không.

Một cài đặt khác sử dụng R của Cristobal Fresno và Elmer
A. [BioScience Data Mining Group](http://www.bdmg.com.ar/?page_id=176) tại Argentina
Tài liệu của họ cũng rất hữu ích
[xem](./Anfis-vignette.pdf) here).  Nó chứa các ví dụ từ bài báo của Jang.

Một bản cài đặt khác bằng Python mang tên [anfis](https://github.com/twmeggs/anfis) bởi Tim Meggs.


### Điều hướng

ANFIS framework chứa 3 file chính:

* [anfis.py](./anfis.py) Định nghĩa các lớp của ANFIS dưới dạng Torch module.

* [membership.py](./membership.py) Hiện tại mới có hàm thành viên Bell và
  Gaussian, các hàm khác sẽ được bổ sung vào đây.

* [experimental.py](./experimental.py) Ví dụ để huấn luyện và kiểm thử FIS với các đồ thị thể hiện kết quả.


Các ví dụ có thể chạy được:

* [jang_examples.py](./jang_examples.py) chứa 4 ví dụ từ bài báo của Jang

* [vignette_examples.py](./vignette_examples.py) chứa 3 ví dụ từ bài báo Vignette



### Cài đặt

Cần có Python và PyTorch.

Phiên bản của tác giả
[Python 3.6.5](https://www.python.org/downloads/)
[Anaconda 4.6.11](https://www.anaconda.com/distribution/)
[PyTorch](https://pytorch.org) phiên bản 1.0.1


### Tác giả ###

* [James Power](http://www.cs.nuim.ie/~jpower/), Maynooth University.
