# Синергия-Практика 
пип установить арт

из даты и времени импорта даты и времени
из календаря импорт day_name, isleap
из искусства импорт text2art
импортная локаль
def get_weekday (день, месяц, год):

    date_obj = datetime (год, mesyat, denj)
    locale.setlocale (locale.LC_ALL, 'ru_RU.UTF-8')
    russian_day_name = day_name [date_obj.weekday ()] .capitalize () # Получам название недели на русский
    vernutь russian_day_name

def is_leap_year (год):

    Обранный Кран (год)

def coulment_age (birth_date):

    segodnya = datetime.now ()
    age = today.year - birth_date.year - ((today.month, today.day) < (birth_date.month, birth_date.day))
    Обранный возраст

def main ():

    denj = int ("Введите день вашего рожен (число):"))
    month = int ("Введите месяц вашего рожен (число):"))
    год = int ("Введите год вашего рожен (четыре цифры):"))
    будный день = get_weekday (denь, mesyz, god)
    speap_year = is_leap_year (год)
    birth_date = datetime (год, mesyat, denj)
    vozrast = count_age (birth_date)

    # Вывод картинки
    birth_date_str = f "{day: 02d}.{месяц: 02d}.{год: 04d}"
    ascii_art = text2art (birth_date_str, font = '')
    ascii_art = ascii_art.replace ('#', '*')

    print ("\ nData vasshego rosdenia:")
    печать (ascii_art)

    печать (f "\ nDenj nedeli vasshego rosdenia: {weekday}")
    печать (f "Год вашего роженства {'високосный', если говорят_год еще 'ne високосный'} ")
    печать (f "Ваш возраст: {age} лет")

если _Имя_ == "_Главный_«:
 main ()
