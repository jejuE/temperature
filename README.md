# temperature

def convert_to_celsius(fahrenheit: float) :
    """ 화씨와 동일한 섭씨를 반환한다.

    >>>convert_to_celsius(75)
    23.88888888889
    """

    return float (fahrenheit - 32.0) * 5.0 / 9.0


def above_freezing(celsius: float) :
    """ celsius가 어는점보다 높으면 True를 반환한다.

    >>>above_freezing(5.2)
    Ture
    >>>above_freezing(-2)
    flase
    """
    
    return celsius > 0

fahrenheit = float(input('온도를 화씨로 입력하세요. :'))
celsius = convert_to_celsius(fahrenheit)
if above_freezing(celsius) == True :
    print('어는점보다 높습니다.')
else :
    print('어는점보다 낮습니다.')
