# digit-recognition
- Mỗi lớp có 100 ảnh. Sau khi aug thành 400.
- Sau khi train có nhận xét:
  Train loss giảm đều theo epoch, cho thấy mô hình học được các đặc trưng của dữ liệu huấn luyện.
  Validation/Test loss cũng giảm theo, và có xu hướng ổn định sau một số epoch nhất định.
  Khoảng cách giữa train loss và validation/test loss không quá lớn, không xuất hiện hiện tượng validation loss tăng mạnh trong khi train loss tiếp tục giảm.
- Đánh giá:
  Mô hình không bị overfitting nghiêm trọng.
  Quá trình huấn luyện diễn ra ổn định.
  Số epoch được lựa chọn là phù hợp, mô hình đã hội tụ.
  Tuy nhiên có điểm bất hợp lý là val lại cao hơn train có thể là do aug mạnh ở train
-  So sánh có và không sử dụng Data Augmentation:
Tiêu chí	            Không Augmentation	  Có Augmentation
Train accuracy	      Cao	                  Cao
Validation accuracy	  Thấp hơn	            Cao hơn
Overfitting	          Dễ xảy ra	            Giảm rõ rệt
Khả năng tổng quát	  Kém hơn	              Tốt hơn
