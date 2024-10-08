# Требования к проекту
---

# Содержание
1 [Введение](#introduction)  
1.1 [Назначение](#purpose)  
1.2 [Бизнес-требования](#business_requirements)  
1.2.1 [Исходные данные](#initial_data)  
1.2.2 [Возможности бизнеса](#business_opportunities)  
1.2.3 [Границы проекта](#project_boundary)  
1.3 [Аналоги](#analogues)  
2 [Требования пользователя](#user_requirements)  
2.1 [Программные интерфейсы](#software_interfaces)  
2.2 [Интерфейс пользователя](#user_interface)  
2.3 [Характеристики пользователей](#user_specifications)  
2.3.1 [Классы пользователей](#user_classes)  
2.3.2 [Аудитория приложения](#application_audience)  
2.3.2.1 [Целевая аудитория](#target_audience)  
2.3.2.1 [Побочная аудитория](#collateral_audience)  
2.4 [Предположения и зависимости](#assumptions_and_dependencies)  
3 [Системные требования](#system_requirements)  
3.1 [Функциональные требования](#functional_requirements)  
3.1.1 [Основные функции](#main_functions)  
3.1.1.1 [Вход пользователя в приложение](#user_logon_to_the_application)  
3.1.1.2 [Настройка профиля активного пользователя](#setting_up_the_profile_of_the_active_user)  
3.1.1.3 [Загрузка объявлений](#download_news)  
3.1.1.4 [Просмотр объявления](#view_information_about_an_individual_newsletter)  
3.1.1.5 [Сохранение объявлений](#view_favorite_and_history_about_an_individual_newsletter)  
3.1.1.6 [Выход пользователя из учётной записи](#active_user_change)  
3.1.2 [Ограничения и исключения](#restrictions_and_exclusions)  
3.2 [Нефункциональные требования](#non-functional_requirements)  
3.2.1 [Атрибуты качества](#quality_attributes)  
3.2.1.1 [Требования к удобству использования](#requirements_for_ease_of_use)    
3.2.1.2 [Требования к безопасности](#security_requirements)  
3.2.1.3 [Требования к доступности](#access_requirements)  
3.2.2 [Внешние интерфейсы](#external_interfaces)  
3.2.3 [Ограничения](#restrictions)  

<a name="intro"/>

# 1 Введение

<a name="purpose"/>

## 1.1 Назначение
В данном документе описаны основные функциональные требования к приложению «Realty Market» для ОС Android. Этот документ предназначен для разработчика или команды разработчиков, которая будет реализовывать и проверять корректность работы приложения.

<a name="business_requirements"/>

## 1.2 Бизнес-требования

<a name="initial_data"/>

### 1.2.1 Исходные данные
Нередко у людей возникает потребность покупки различной недвижимости, и они начинают задваться вопросом, где можно найти каталог актуальных объявлений с информацией о покупаемой недвижимости. Необходим ресурс, где будет собрана вся необходимая информация с возможнотью связи с продавцом. 

<a name="business_opportunities"/>

### 1.2.2 Возможности бизнеса
Многие люди оценят приложение, которое предлагает подробную информацию о покупке, продаже и аренде недвижимости в их регионе. Удобный интерфейс и функциональность, позволяющая отображать доступные объекты на карте, сделают процесс поиска жилья более простым и эффективным. Пользователи смогут легко находить подходящие варианты, основываясь на своих предпочтениях и геолокации. Это приложение будет ориентировано на всех, кто хочет быстро и удобно найти идеальную недвижимость для покупки или аренды, благодаря интуитивно понятному дизайну и полезным фильтрам.

<a name="project_boundary"/>

### 1.2.3 Границы проекта
Приложение "Realty Market" предоставит пользователям возможность удобно просматривать объекты недвижимости с помощью карты. После регистрации откроется расширенный функционал, который позволит добавлять свои предложения о продаже или аренде, а также просмотры других объектов. Пользователи смогут легко находить подходящие варианты, взаимодействовать с другими участниками рынка и получать актуальную информацию о недвижимости в своем регионе. Интуитивно понятный интерфейс сделает использование приложения доступным для всех желающих.

<a name="analogues"/>

## 1.3 Аналоги
Аналогами приложения "Realty Market" являются такие платформы, как Avito и Realtor.com. Основной особенностью этих аналогов является то, что они позволяют пользователям находить и размещать объявления о продаже, покупке и аренде недвижимости. Оба приложения предоставляют подробную информацию о каждом объекте, включая фотографии, цены и описание, а также возможность связаться с продавцом или арендодателем.

<a name="user_requirements"/>

# 2 Требования пользователя

<a name="software_interfaces"/>

## 2.1 Программные интерфейсы
Данные будут храниться в базе данных на собственном сервере.
Для просмотра адреса по картам будет использоваться API. 

<a name="user_interface"/>

## 2.2 Интерфейс пользователя
Вход в приложение.  

![Вход в приложение](https://github.com/Tonitruc/Realty-Market/blob/master/docks/Mockups/Enter.png)  

Окно регистрации нового пользователя.  

![Окно регистрации нового пользователя](https://github.com/Tonitruc/Realty-Market/blob/master/docks/Mockups/Registration.png) 

Окно каталога объявлений о недвижимости.

![Окно каталога объявлений о недвижимости](https://github.com/Tonitruc/Realty-Market/blob/master/docks/Mockups/Catalog.png)  

Окно добавления нового объявления.  

![Окно добавления нового объявления](https://github.com/Tonitruc/Realty-Market/blob/master/docks/Mockups/Add%20Advertisement.png).

Окно просмотра информации о недвижимости.  

![Окно просмотра информации о недвижимости](https://github.com/Tonitruc/Realty-Market/blob/master/docks/Mockups/Advertisement%20Preview.png).

Окно избранных объявлений.  

![Окно избранных объявлений](https://github.com/Tonitruc/Realty-Market/blob/master/docks/Mockups/Favourites.png).
                                  
Окно пользователя.  

![Окно пользователя](https://github.com/Tonitruc/Realty-Market/blob/master/docks/Mockups/User.png).

Окно выбора местопложения недвижимости.  

![Окно выбора местопложения недвижимости](https://github.com/Tonitruc/Realty-Market/blob/master/docks/Mockups/ChooseLocation.png).

Окно фильтра для поиска недвижимости.  

![Окно фильтра для поиска недвижимости](https://github.com/Tonitruc/Realty-Market/blob/master/docks/Mockups/Filter.png).

<a name="user_specifications"/>

## 2.3 Характеристики пользователей

<a name="user_classes"/>

### 2.3.1 Классы пользователей

| Класс пользователей | Описание |
|:---|:---|
| Гости | Пользователи, которые не прошли регистрацию и имеют ограниченную функциональность |
| Зарегистрированные пользователи | Пользователи, которые прошли регистрацию и имеют полную функциональность |

<a name="application_audience"/>

### 2.3.2 Аудитория приложения

<a name="target_audience"/>

#### 2.3.2.1 Целевая аудитория
Люди, которым необходимо купить, продать или арендовать недвижимость.

<a name="collateral_audience"/>

#### 2.3.2.2 Побочная аудитория
Люди, которые интересуется рынком недвижимости или планируют покупку в будущем. 

<a name="assumptions_and_dependencies"/>

## 2.4 Предположения и зависимости
1. Пользователь не может пользоваться какой-либо функциональностью приложения без интернета. 

<a name="system_requirements"/>

# 3 Системные требования

<a name="functional_requirements"/>

## 3.1 Функциональные требования

<a name="main_functions"/>

### 3.1.1 Основные функции

<a name="user_logon_to_the_application"/>

#### 3.1.1.1 Вход пользователя в приложение
**Описание.** Работа в приложении возможна без создания профиля или же с авторизацией.

| Функция | Требования | 
|:---|:---|
| Вход без создания профиля | Приложение должно предоставить пользователю возможность войти в приложение в качестве гостя |
| Регистрация нового пользователя | Приложение запрашивает логин, пароль и номер пользователя. Ввод электронной почты не обязателен. Пользователь вводит данные и регистрируется |
| Вход с авторизацией | Приложение запрашивает логин и пароль, после чего пользователь входит в профиль |

<a name="setting_up_the_profile_of_the_active_user"/>

#### 3.1.1.2 Просмотр информации о недвижимости
**Описание.** Все пользователи могут просмотреть каталог продаваемой недвижимости.
 
| Функция | Требования | 
|:---|:---|
| Просмотр подробной информации | Выбрав объявление, можно посмотреть всю информацию о недвижимсоти, например, адреса, площади, местопложения и т.д. |
| Просмотр местоположения на карте | Предоставляется возможность просмотра выбранного объявления на карте |
| Связь с продавцом | В выбранном объявлении, также будет указана контактная информация для связи с продавцом |

<a name="download_news"/>

#### 3.1.1.3 Добавление нового объявления
**Описание.** Авторизированные пользователи могут добавить свои объявления, чтобы другие их тоже видели.

| Функция | Требования | 
|:---|:---|
| Добавление нового объявления | Приложение запрашивает информацию о местоположении недпижимости с выбором на карте. Требует указать площадь, цену, категорию недвижимости и другую дополнительную информацию. |

<a name="view_information_about_an_individual_newsletter"/>

#### 3.1.1.4 Удаление объявлений
**Описание.** Авторизированные пользователи могут удалять свои собственные объявления

| Функция | Требования | 
|:---|:---|
| Удаление объявления | Пользователь имеет возможноть удалить свое объявление |
| Закрытие объявления | Объявление будет удалено из каталога при продаже или потере актуальности статуса недвижимости |

<a name="view_favorite_and_history_about_an_individual_newsletter"/>

#### 3.1.1.5 Сохранение объявлений
**Описание.** Авторизированные пользователи могут сохранять объявления в избранное, а также будет сохранена информация о проданной недвижимости

| Функция | Требования | 
|:---|:---|
| Добавление объявлений в избранное | Пользователь имеет возможноть добавлять свое объявление в избранное |
| Сохранение в истории | Объявление, которые было закрыто по причине продажи недвижимости будет сохранено в истории |

<a name="active_user_change"/>

#### 3.1.1.6 Выход из профиля
**Описание.** Зарегистрированный пользователь имеет возможность выйти из профиля.

| Функция | Требования | 
|:---|:---|
| Выход из учётной записи | Нажав на кнопку выхода из профиля, пользователь становится анонимным |  

<a name="restrictions_and_exclusions"/>

### 3.1.2 Ограничения и исключения
1. Приложение отображает информацию только при подключении к интернету.

<a name="non-functional_requirements"/>

## 3.2 Нефункциональные требования

<a name="quality_attributes"/>

### 3.2.1 Атрибуты качества

<a name="requirements_for_ease_of_use"/>

#### 3.2.1.1 Требования к удобству использования
1. Приложение реализует все основные функции;
2. Все функциональные элементы пользовательского интерфейса имеют названия, описывающие действие, которое произойдет при выборе элемента.
3. Интерфейс не содержит лишних элементов.

<a name="security_requirements"/>

#### 3.2.1.2 Требования к безопасности
1. Приложение не дает возможности удалять чужие объявления.
2. Приложение допускает создание объявлений только у авторизированных пользователей.

<a name="access_requirements"/>

#### 3.2.1.3 Требования к доступности
Время реакции на действия пользователя минимально.

<a name="external_interfaces"/>

### 3.2.2 Внешние интерфейсы
Окна приложения удобны для использования пользователями.

<a name="restrictions"/>

### 3.2.3 Ограничения
1. Приложение реализовано для ОС Android;
2. Язык, на котором реализована программа, - С#.