# AI Project 2 - Decision Tree Classification

## Mô tả dự án

Dự án này xây dựng, huấn luyện và đánh giá các mô hình Cây quyết định (Decision Tree) trên nhiều bộ dữ liệu thực tế: Dry Bean, Titanic, Heart Disease, Penguins. Mục tiêu là phân tích, trực quan hóa dữ liệu, áp dụng các kỹ thuật tiền xử lý, huấn luyện mô hình, đánh giá hiệu quả và tối ưu tham số cho từng bài toán phân loại.

Các bước chính trong mỗi notebook:
- Khám phá, phân tích và trực quan hóa dữ liệu.
- Tiền xử lý dữ liệu: kiểm tra giá trị thiếu, encode nhãn, tách đặc trưng và nhãn.
- Chia dữ liệu thành các tập train/test với nhiều tỷ lệ khác nhau (40/60, 60/40, 80/20, 90/10) và đảm bảo phân tầng nhãn.
- Huấn luyện mô hình Decision Tree với các tiêu chí khác nhau (entropy, gini).
- Đánh giá mô hình bằng confusion matrix, classification report, cross-validation.
- Trực quan hóa cây quyết định bằng Graphviz.
- Phân tích ảnh hưởng độ sâu cây, tối ưu tham số với GridSearchCV.
- Phân tích tầm quan trọng của các đặc trưng.

## Cấu trúc thư mục

```
.
├── Decision-Tree-AI-Project-main/
│   ├── Bean.ipynb
│   ├── Titanic.ipynb
│   ├── heart.ipynb
│   ├── penguins.ipynb
│   ├── Data/
│   │   ├── Dry_Bean.csv
│   │   ├── Titanic.csv
│   │   ├── processed.cleveland.csv
│   │   └── penguins.csv
│   └── ...
├── requirements.txt
├── README.md
├── AI - Project 2 (1).pdf
└── ...
```

## Yêu cầu môi trường

- Python >= 3.7
- Các thư viện: numpy, pandas, matplotlib, seaborn, scikit-learn, graphviz, jupyter, ucimlrepo

## Cài đặt thư viện

Chạy lệnh sau trong terminal để cài đặt tất cả thư viện cần thiết:
```sh
pip install -r requirements.txt
```

Nếu bạn chưa có Jupyter Notebook, cài đặt bằng:
```sh
pip install jupyter
```

## Hướng dẫn chạy chương trình

1. **Clone hoặc tải về mã nguồn dự án.**
2. **Cài đặt thư viện như hướng dẫn ở trên.**
3. **Mở file notebook mong muốn:**
   - Chạy lệnh:
     ```sh
     jupyter notebook
     ```
   - Sau đó mở một trong các file sau trên giao diện Jupyter Notebook:
     - `Decision-Tree-AI-Project-main/Bean.ipynb` (Dry Bean)
     - `Decision-Tree-AI-Project-main/Titanic.ipynb` (Titanic)
     - `Decision-Tree-AI-Project-main/heart.ipynb` (Heart Disease)
     - `Decision-Tree-AI-Project-main/penguins.ipynb` (Penguins)
4. **Chạy tuần tự từng cell trong notebook để thực hiện toàn bộ quy trình phân tích, huấn luyện, đánh giá và trực quan hóa mô hình.**

## Lưu ý

- Đảm bảo các file dữ liệu (`Dry_Bean.csv`, `Titanic.csv`, `processed.cleveland.csv`, `penguins.csv`) nằm đúng trong thư mục `Data/` như cấu trúc trên.
- Nếu gặp lỗi với graphviz, hãy cài đặt thêm phần mềm Graphviz phù hợp với hệ điều hành và đảm bảo biến môi trường PATH đã được thiết lập.
- Mỗi notebook có thể có hướng dẫn chi tiết riêng cho từng bộ dữ liệu.

## Tham khảo

- [Dry Bean Dataset - UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Dry+Bean+Dataset)
- [Titanic Dataset - Kaggle](https://www.kaggle.com/c/titanic/data)
- [Heart Disease Dataset - UCI](https://archive.ics.uci.edu/ml/datasets/heart+Disease)
- [Palmer Penguins Dataset](https://github.com/allisonhorst/palmerpenguins)
- [Scikit-learn Decision Tree Documentation](https://scikit-learn.org/stable/modules/tree.html)

---

**Tác giả:**  
- [Tên nhóm/Sinh viên