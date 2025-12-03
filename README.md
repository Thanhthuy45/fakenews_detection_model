# fakenews_detection_model


1. Mục tiêu của bài toán này là xây dựng và so sánh hiệu quả của các mô hình trong phát hiện tin giả. Thông qua đó, nghiên cứu hướng tới việc đề xuất các giải pháp cải tiến nhằm nâng cao khả năng phát hiện tin giả, đồng thời mở rộng mô hình theo hướng kết hợp thêm thông tin ngữ cảnh hoặc dữ liệu đa phương thức để tăng tính chính xác và khả năng ứng dụng trong thực tế.

2. dataset: WELFake News
- Đây là 1 bộ data nổi tiếng lấy từ kaggle: https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification/data/code

- Bộ dữ liệu WELFake có 72.134 bài báo, trong đó có 35.028 tin thật và 37.106 tin giả, bao gồm bốn cột: id (bắt đầu từ 0); Title (về tiêu đề tin tức văn bản); Text (về nội dung tin tức); và Lable (0 = giả và 1 = thật).

3. Nội dung thư mục gồm các file code xử lý dữ liệu và xây dựng các model từ truyền thống, học sâu đến mô hình tiền huấn luyện.

- model_ml_dense.ipynb : file chứa code thực hiện các bước tiền xử lý dữ liệu, xây dựng và huấn luyện mô hình học máy truyền thống, mô hình học sâu Dense, đánh giá độ chính xác của các mô hình.

- model_LSTM_fake_news_detection.ipynb : file thực hiện bước xử lý dữ liệu, xây dựng và huấn luyện mô hình học sâu LSTM.

- model_bert_fakenews.ipynb : file thực hiện xây dựng huấn luyện mô hình tiền huấn luyện BERT, đánh giá độ chính xác của mô hình trên tập dữ liệu phát hiện tin giả.

- kiem_tra_cheo_với_distilbert_tinhchinh.ipynb : file thực hiện kiểm tra chéo với distilbert và tiến hành tinh chỉnh mô hình.

- file: xoa_trung_lap_tinh_chỉnh_distilbert.ipynb : file thực hiện tinh chỉnh mô hình distilbert nhưng khác với những mô hình trước ở việc xử lý phần dữ liệu bị trùng lặp nhằm giúp mô hình học tốt hơn.

4. Chú ý:
- Trong trường hợp máy tính cá nhân chưa cung cấp đủ gpu, môi trường hoặc các thư viện cần thiết thì đề xuất có thể chạy file code trên môi trường google colab (có hỗ trợ gpu) 
