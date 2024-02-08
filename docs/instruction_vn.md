## Cấu trúc đề thi Tensorflow

*Dành cho lớp học TF*

### Lưu ý quan trọng

**1/ Hệ thống chấm bài:**

Mỗi đầu bài đều có ghi rõ input shape của grading system, để khớp với data/model

Nếu submit sai dimension, hệ thống sẽ báo là sai Dimension (vd: `inputEmbedding shape is 120, but expecting 100`)

Không được dùng lambda layer.

**2/ Các đường dẫn quan trọng**

- Hướng dẫn thi: [Hướng dẫn thi](https://www.tensorflow.org/extras/cert/TF_Certificate_Candidate_Handbook.pdf)
- Đăng ký thi tại: [Đăng ký thi](https://app.trueability.com/google-certificates/tensorflow-developer)

**3/ Dàn bài thi**

**Bài 1. Linear Regression**

- Đề mẫu: [Đề mẫu](https://protonx.io/courses/64241ad3a251d4001aac5d92/topics/6519164a6921ef001a0234f3?activeAId=6519164a6921ef001a023514)
- Lời giải mẫu: Chú ý: Không có tập validation nên train tầm 500 - 1000 epochs để đảm bảo đạt acc

**Bài 2. Phân loại: MNIST, Fashion MNIST, IRIS**

- Đề mẫu: [Đề mẫu](https://protonx.io/courses/64241ad3a251d4001aac5d92/topics/6519164a6921ef001a0234f3?activeAId=6519164a6921ef001a023516)
- Lời giải mẫu: Hướng dẫn xây mô hình trên bộ MNIST: [Video](https://youtu.be/8WxENdR46qA)
- Chú ý: 
  - Bài này chỉ cần sử dụng mạng Neural Network với vài lớp Dense, không dùng CNN (nếu dùng sẽ báo lỗi)
  - Đề có thể cho tf.dataset, nhớ chia ảnh đầu vào cho 255

**Bài 3. Phân loại ảnh thực tế:**

- Dataset: Chó - mèo, Ngựa - người, Dao - Búa - Kéo
- Đề mẫu: [Đề mẫu](https://protonx.io/courses/64241ad3a251d4001aac5d92/topics/6519164a6921ef001a0234f3?activeAId=6519164a6921ef001a023518)
- Lời giải mẫu: 
  - Chó mèo: [Video](https://youtu.be/kShvYHDXvvg)
  - Ngựa người: [Video](https://youtu.be/ee9tF9xEf04)
  - Dao búa kéo: [Notebook](https://www.tensorflow.org/datasets/catalog/rock_paper_scissors)
- Chú ý:
  - Ưu tiên không sử dụng Transfer Learning sớm, sử dụng một mô hình CNN thông thường.
  - Nếu cần sử dụng Transfer Learning - ưu tiên MobileNet

**Bài 4. Phân loại mỉa mai - Detecting sarcasm (chưa đổi đề)**

- RNN, sentiment classification, chú ý sử dụng tokenizer + padding
- Độ chính xác khoảng 84-87%
- Tokenizer mỉa mai
- Xây dựng mô hình RNN
<!-- **Bài 5. Phân loại cảm xúc câu,  (chưa đổi đề)**

- Độ chính xác khoảng 84-87%
- Tokenizer mỉa mai
- Xây dựng mô hình RNN -->

**Bài 5. Một bài Time-series: Sunspot trên coursera (chưa đổi đề)**

- MAE < 0.12
- Min Max Scale
- Chiều của LSTM hoặc chiều của h phù hợp với chiều thứ 3

Tài liệu chuẩn bị:

- [Video hướng dẫn](https://www.youtube.com/watch?v=j5HxIJoOJms&list=PLMm4sOMuA2QI5x_0KlNT3LuKDi6-ByboB)
- [Coursera - TensorFlow in Practice](https://www.coursera.org/specializations/tensorflow-in-practice)
- [GitHub repository](https://github.com/lmoroney/dlaicourse)