# Karadeniz Ereğli Hava Kalitesi Tahmini

Günlük hava kalitesi ölçümlerinden ertesi günün PM2.5 AQI puanını tahmin eder.

## Nasıl çalıştırılır?

Python ile proje klasöründe powershell'de şu komutları çalıştır:

```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

Gömülü virtual environment'ı kernel olarak set ettikten sonra:

1. `data_preparation.ipynb` ./data/raw klasör yolundaki CSV’yi işler ve işlenmiş veriyi `data/processed/` klasörüne kaydeder.
2. `model_configuration.ipynb` modeli eğitir, sonuçları gösterir ve eğitilmiş modeli `models` yoluna(yoksa oluşturur) kaydeder.
