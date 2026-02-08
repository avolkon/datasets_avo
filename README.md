Репозиторий для загрузки датасетов

# Скачать датасет из GitHub (вставить свой raw-url)
url = 'https://raw.githubusercontent.com/yougit/yuor_repo/main/real_estate_data.csv'

df = pd.read_csv(url, sep='\t') # проверить какой точно будет разделитель
варианты: ('moscow_places.csv', sep=',', decimal='.')

print(f"Загружено {len(df)} строк, {len(df.columns)} столбцов")
print("\nПервые 5 строк:")
display(df.head())
