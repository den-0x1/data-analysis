# data-analysis

#### 1. Анализ набора данных о рейсах авиакомпаний
- Источник: [Airlines Flights Data](https://www.kaggle.com/datasets/rohitgrewal/airlines-flights-data)
- [Дашборд](https://datalens.yandex/psdf16kfemw08?_share_link=public)

#### 2. E-Commerce
- Источник:
```python
    NUM_RECORDS = 1000
    START_DATE = datetime(2025, 1, 1)
    END_DATE = datetime(2026, 12, 31)
    data = []
    print("Generating e-commerce mock data...")
    for _ in range(NUM_RECORDS):
        sale_date = random_date(START_DATE, END_DATE).strftime("%Y-%m-%d")
        date_object = datetime.strptime(sale_date, "%Y-%m-%d")
        quantity = random.randint(1, 11) * date_object.month
        record = {
            "shop": f"Магазин №{random.randint(1, 5)}",
            "product_name": f"Товар {random.randint(1, 10)}",
            "quantity": quantity,
            "price": round(random.uniform(5.0, 1000.0), 2),
            "sale_date": sale_date,
        }
        data.append(record)
    # Convert to pandas DataFrame and save to CSV
    df = pd.DataFrame(data)
    df.to_csv("data.csv", index=False)
    print("Data generation complete")
```
- [Дашборд](https://datalens.yandex/fi9za0z9syocy?_share_link=public)

#### 3. Анализ набора данных о аукционе автомобилей
- Источник: [US Cars Dataset](https://www.kaggle.com/datasets/doaaalsenani/usa-cers-dataset)
- [Дашборд](https://datalens.yandex/hkg4tg46zruw0?_share_link=public)

#### 4. Кластеризация вин при помощи метода DBSCAN
- Источник: [Wine Dataset for Clustering](https://www.kaggle.com/datasets/harrywang/wine-dataset-for-clustering)
- [Дашборд](https://datalens.yandex/nqo4qcerrp4k6?_share_link=public)

#### 5. Прогнозирование временных рядов
- Источник: [French bakery daily sales](https://www.kaggle.com/datasets/matthieugimbert/french-bakery-daily-sales)
- [Дашборд](https://datalens.yandex/jn3z1nl5vgvc2?_share_link=public)
