# Pandas basic
> Pandas problem-solving study for Data Analysis



## Introduction

> 본 directory 학습내용의 출처는 [FutureSkill](https://futureskill.io/)의 [Contents](https://futureskill.io/content/903ab63c-2b24-4be0-ba1c-a3ba34dce258)입니다.

 **Pandas** 는 파이썬 데이터 분석 라이브러리(Python Data Analysis Library)의 약자로서, 표 형태의 DataFrame 을 자유자재로 잘 다룰 수 있도록 도와주는 라이브러리이다. 이런 표 형태의 데이터를 정형 데이터(Structured Data, Tabular Data)라고 한다.

Pandas를 통해서 우리는 정형 데이터 분석을 손쉽게 할 수 있다. 따라서 본 contents를 통해 데이터 분석에서 가장 많이 사용하는 정형 데이터를 효과적으로 다루는 연습을 해 보고자 한다.

> p.s. pandas는 내부적으로 numpy array를 확장하여 구현되어 있다. numpy의 기본적인 개념인 모든 dtype이 동일한 것과, fancy indexing, broadcasting 등을 모두 지원한다.



## Contents



1. pandas data structure
2. pandas data structure (2)
3. pandas data structure (3)
4. DataFrame method
5. DataFrame method (2)
6. DataFrame method (3)
7. DataFrame method (4)
8. DataFrame method (5)
9. sorting
10. indexing
11. indexing (2)
12. indexing (3)
13. indexing (4)
14. concat
15. concat (2)
16. read write panel data
17. read write panel data (2)
18. read write panel data (3)
19. missing values
20. missing values (2)
21. missing values (3)
22. missing values (4)
23. aggregating
24. aggregating (2)
25. aggregating (3)
26. pivot table



below is to update

## Numpy Data type

`numpy.bool` : `bool` Boolean (True or False) stored as a byte

`numpy.byte` : `signed char` Platform-defined

`numpy.ubyte` : `unsigned char` Platform-defined

`numpy.short` : `short` Platform-defined

`numpy.ushort` : `unsigned short` Platform-defined

`numpy.intc` : `int` Platform-defined

`numpy.uintc` : `unsigned int` Platform-defined

`numpy.int_` : `long` Platform-defined

`numpy.uint` : `unsigned long` Platform-defined

`numpy.longlong` : `long long` Platform-defined

`numpy.ulonglong` : `unsigned long long` Platform-defined

`numpy.half` / `numpy.float16` : Half precision float: sign bit, 5 bits exponent, 10 bits mantissa

`numpy.single` : `float` Platform-defined single precision float: typically sign bit, 8 bits exponent, 23 bits mantissa

`numpy.double` : `double` Platform-defined double precision float: typically sign bit, 11 bits exponent, 52 bits mantissa.

`numpy.longdouble` : `long double` Platform-defined extended-precision float

`numpy.csingle` : `float complex` Complex number, represented by two single-precision floats (real and imaginary components)

`numpy.cdouble` : `double complex` Complex number, represented by two double-precision floats (real and imaginary components)

`numpy.clongdouble` : `long double complex` Complex number, represented by two extended-precision floats (real and imaginary components).  

> **reference** [Numpy documentation](https://numpy.org/devdocs/user/basics.types.html#array-types-and-conversions-between-types)  


​    

platform에 따라 달라지는 data type을 제외하면 다음과 같다.

1. **Integer** 계열

   - `int8`, `int16`, `int32`, `int64`  
     모두 Integer를 나타내며 뒤에 따라오는 숫자에 따라 표현 범위가 정해짐.  

     > e.g. `int8`(8bytes) : -128 ~ 127

   - `uint8`, `uint16`, `uint32`, `uint64`    
     모두 unsigned integer를 나타내며 뒤에 따라오는 숫자에 따라 표현 범위가 정해짐.  

     > e.g. `uint16`(16bytes) : 0 ~ 65535



2. **Floating-point** 계열

   - `float32`, `float64`  
     모두 fixed-floating 타입을 나타내며 뒤에 따라오는 숫자에 따라 표현 범위가 정해짐.  
     (float16도 있으나, platform-dependent)  

     > e.g. `float32`(single precision, sign bit + 8 bits exponent + 23 bits mantissa)  

  



> **reference** [FutureSkill 김용담 creator](https://futureskill.io/content/79eba49a-178d-41be-8f88-137a5127742d/question/ced42779-2980-46d6-90a5-8d4d2f1e6c61)









---



#### Contents

- [Future Skill](https://futureskill.io/)

#### Course
- [[Python Data Analysis & Image Processing] - Dongbin Na](https://www.youtube.com/playlist?list=PLRx0vPvlEmdBx9X5xSgcEk4CEbzEiws8C)
- [Youtube Minsuk Heo 허민석](https://www.youtube.com/channel/UCxP77kNgVfiiG6CXZ5WMuAQ)
  - [[Pandas 강의\] 팬더스, 데이터프레임, 시리즈 알아보기](https://www.youtube.com/watch?list=PLVNY1HnUlO26Igldy2Q6Nb2LZbpQWTyle&v=pFXipjh0ghw&feature=emb_logo) 

#### Editor
- [**Colab**](https://colab.research.google.com/) / PyCharm