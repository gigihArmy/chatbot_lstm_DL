# Chatbot LSTM Tan Malaka
## Deskripsi
Project ini menggunakan bahasa Python dengan bantuan tools Google Colab. Chatbot ini memanfaatkan dataset berbahasa Indonesia mengenai biografi Tan Malaka. Algoritma Deep Learning LSTM (Long-Short Term Memory) dimanfaatkan untuk klasifikasi pola pertanyaan pada tag tertentu. Model yang telah dilatih memprediksi user input dan memberikan respon.

## Dataset (dataset_dl.json)
Domain atau cakupan dataset sebatas mengenai biografi Tan Malaka. Dataset berisi intens yang didalamnya terdapat tag untuk menentukan knowledge base yang terdapat pattern dan response. Pattern berisi pola pertanyaan yang mungkin user inputkan sebagai data latih. Response berisi data yang disajikan model untuk menjawab user, model hanya memilih salah satu response.

## Preprocessing
Terdapat 3 tahapan Preprocessing Data :
- Cleaning
- Lemmatize
- Tokenisasi
- Label Encoding

## Embedding
Penggunaan embedding pretrained Fast-Text bahasa Indonesia untuk meningkatkan akurasi model dengan merepresentasikan teks dalam bentuk numerik, mengurangi dimensi dan meningkatkan efisiensi, dan menangkap hubungan semantik antar kata.

## LSTM Model (chatbot_lstm_model.keras)
LSTM Bidirectional (BiLSTM) cocok untuk kasus NLP karena memahami hubungan antar kata lebih baik dibandingkan LSTM Unidirectional. Akurasi dan Validation Akurasi model ini mencapai 62%.

#### Note: Jika ingin langsung uji coba model (chatbot_lstm_model.keras) pada file notebook (lstm_chatbot_tanmalaka.ipynb), lakukan tahapan Import Library hingga Text Preprocessing lalu scroll ke tahapan Load Model Chatbot keras. 
