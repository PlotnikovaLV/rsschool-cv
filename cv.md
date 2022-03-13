# Liudmila Plotnikava
![PREVIEW photographer's portfolio](/img/ava.jpg)

## Contacts
* Phone: +375(29)256-80-11
* Email: l.plotikova.v@gmail.com
* Telegram: @plv2121
* LinkedIn: [@plv2121](https://www.linkedin.com/in/plv2121/)
* GitHub: [PlotnikovaLV](https://github.com/PlotnikovaLV)
* discord-nik: Plotnikova#7817
* Location: Uzda, Belarus

## About Me
I like to learn, improve and grow. Even at school, I chose a mathematical profile of study, and after graduating from university, I switched to programming. I am fascinated by mental work, I am fascinated by ideological work. My goal is to become the best front-end developer. My hobbies are hiking and running. I love my kids and driving a car)))

## Experience
* System Administrator, 2014 to the present...
* Software Engineer, 2012-2014.
* Computer Science Teacher, 2007-2011.

## Skills
1. Windows OS, LAN, WLAN, MS Office - advanced
2. Routing protocols - confident
3. Python, JavaScript - intermediate
4. HTML5, CSS3, Django, Git, GitHub, Editors: VSCode and PyCharm - beginner
5. SQLite3 - basic

## Code Example
+ **JavaScript**

#### Function strCount (takes an object as an argument) count all string values inside the object, including nested ones:
```
function strCount(obj){
  let n = 0;
  for (let key in obj){
    if (typeof obj[key] === 'string'){
      n += 1;
    }else if (typeof obj[key] === 'object' && obj[key]!==null){
      n += strCount(obj[key]);
      };
  };
  return n;
}
```

+ **Python**

#### Creating a 9x9 Sudoku table:
#### def_file.py

```
def print_square(lst):
    a = 0
    b = 3
    while b <= 9:
        c = 0
        d = 3
        while d <= 9:
            for i in range(a, b):
                for j in range(c, d):
                    print(f' {lst[i][j]} ', end='')
                print('|', end='')
            c += 3
            d += 3
            print()
        for i in range(30):
            print('-', end='')
        print()
        a += 3
        b += 3
```

#### sudoku.py

```
import random
import def_file

def num_square() -> tuple:
    square = []
    flag = True
    for i in range(3, 10, 3):
        for n in range(0, 9):
            if len(square) < 9:
                square.append([])
            set_num = set()
            j = 0
            while len(square[n]) < i:
                num = random.randint(1, 9)
                flag_append = False
                if n == 0:
                    if square[n].count(num) == 0:
                        square[n].append(num)
                if n == 1:
                    if square[n].count(num) == 0 and (num not in square[n-1][i-3:i]):
                        square[n].append(num)
                if n == 2:
                    if square[n].count(num) == 0 and (num not in square[n-1][i-3:i]) and (
                            num not in square[n-2][i-3:i]):
                        square[n].append(num)
                if n == 3:
                    if square[n].count(num) == 0 and (num not in square[n-3][0 + j: 7 + j: 3]):
                        flag_append = True
                elif n == 4:
                    if square[n].count(num) == 0 and (num not in square[n-1][i-3:i]) and (
                            num not in square[n-3][0 + j: 7 + j: 3]):
                        flag_append = True
                elif n == 5:
                    if square[n].count(num) == 0 and (num not in square[n-1][i-3:i]) and (
                            num not in square[n-2][i-3:i]) and (num not in square[n-3][0 + j: 7 + j: 3]):
                        flag_append = True
                elif n == 6:
                    if square[n].count(num) == 0 and (num not in square[n-3][0 + j: 7 + j: 3]) and (
                            num not in square[n-6][0 + j: 7 + j: 3]):
                        flag_append = True
                elif n == 7:
                    if square[n].count(num) == 0 and (num not in square[n-1][i-3:i]) and (
                            num not in square[n-3][0 + j: 7 + j: 3]) and (num not in square[n-6][0 + j: 7 + j: 3]):
                        flag_append = True
                elif n == 8:
                    if square[n].count(num) == 0 and (num not in square[n-1][i-3:i]) and (
                            num not in square[n-2][i-3:i]) and (num not in square[n-3][0 + j: 7 + j: 3]) and (
                            num not in square[n-6][0 + j: 7 + j: 3]):
                        flag_append = True
                if flag_append:
                    square[n].append(num)
                    j += 1
                set_num.add(num)
                if len(set_num) == 9 and len(square[n]) != i:
                    flag = False
                    break
            if not flag:
                break
        if not flag:
            break
    if not flag:
        return square, False

    return square, True

tuple_square = num_square()
while tuple_square[1] == False:
    tuple_square = num_square()
for i in tuple_square[0]:
    print(i)

def_file.print_square(tuple_square[0])
```

## Study projects
+ ### [Photographer's portfolio](https://rolling-scopes-school.github.io/plotnikovalv-JSFEPRESCHOOL/portfolio/ "go to site")
[![PREVIEW photographer's portfolio](/img/portfolio-photographer.jpg)](https://rolling-scopes-school.github.io/plotnikovalv-JSFEPRESCHOOL/portfolio/)
+ ### [Movie application](https://rolling-scopes-school.github.io/plotnikovalv-JSFEPRESCHOOL/movie-app/ "go to service")
[![PREVIEW movie application](/img/movie-app.jpg)](https://rolling-scopes-school.github.io/plotnikovalv-JSFEPRESCHOOL/movie-app/)
+ ### [Tetris game](https://rolling-scopes-school.github.io/plotnikovalv-JSFEPRESCHOOL/tetris-game/ "go to game")
[![PREVIEW tetris game](/img/tetris-game.jpg)](https://rolling-scopes-school.github.io/plotnikovalv-JSFEPRESCHOOL/tetris-game/)

## Education
* Republican Institute of Advanced Training and Retraining of Personnel. Software engineer.
* Belarusian State Pedagogical University. Teacher of physics, mathematics and computer science.

## Courses
* IT-Overone. [Python programming language, Python back-end developer](https://overone.by/python#!/tab/403925666-1 "Course program").
* RS School. [JS / front-end, stage 0 (ru)](https://app.rs.school/certificate/dxg6778o "Certificate").
* at moment student RS School. [JS / front-end (ru)](https://rs.school/js/ "Course «JavaScript/Front-end»").

## Languages
- Belarusian, Russian: native
- German: A1
- English: A1