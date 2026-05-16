def total_salary(path):
    try:
        total = 0
        count = 0
        with open(path, "r", encoding="utf-8") as fh:
            for line in fh:
                name, salary = line.strip().split(',', 1)
                total += float(salary)
                count += 1
        average = total / count if count > 0 else 0
        return total, average
    except FileNotFoundError:
        print("Файл не знайдено")
        return None

total_, average_ = total_salary("file.txt")

print(f"Сума: {total_}, Середня: {average_}")
