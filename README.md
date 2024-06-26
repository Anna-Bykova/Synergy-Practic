# Синергия-Практика 
from datetime import datetime
from calendar import day_name, isleap
from art import text2art
import locale
def get_weekday(day, month, year):

    date_obj = datetime (год, месяц, день)
    locale.setlocale (locale.LC_ALL, 'ru_RU.UTF-8')
    russian_day_name = day_name [date_obj.weekday ()] .capitalize () # Получам название день недели на русский
    вернуть russian_day_name

def is_leap_year(year):

    обратный кран (год)

def calculate_age(birth_date):

    сегодня = datetime.now ()
    age = today.year - birth_date.year - ((today.month, today.day) < (birth_date.month, birth_date.day))
    обратный возраст

def main():

    день = int ("Введите день вашего рожен (число):"))
    month = int ("Введите месяц вашего рожен (число):"))
    год = int ("Введите год вашего рожен (четыре цифры):"))
    будний день = get_weekday (день, месяц, год)
    speap_year = is_leap_year (год)
    birth_date = datetime (год, месяц, день)
    возраст = count_age (birth_date)

    # Вывод картинки
    birth_date_str = f "{day: 02d}.{месяц: 02d}.{год: 04d}"
    ascii_art = text2art (birth_date_str, font = '')
    ascii_art = ascii_art.replace ('#', '*')

    print ("\ nData vasshego rosdenia:")
    print (ascii_art)

    print (f "\ nDenj nedeli vasshego rosdenia: {weekday}")
    print (f "Год вашего роженства {'високосный', если speak_year else 'ne високосный'}")
    print (f "Ваш возраст: {age} лет")

if _имя_ == "_главный_«:
    main()
