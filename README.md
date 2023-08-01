from datetime import datetime
import pyjokes
from application.salary import calculate_salary as calculate_s
from application.db.people import get_employees as get_emp


def date_now():
    today = datetime.today()
    print(today)


if __name__ == '__main__':
    print("Дата:")
    date_now()
    print()
    get_emp()
    print()
    calculate_s()
    print()
    print(pyjokes.get_joke())
