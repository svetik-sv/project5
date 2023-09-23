# Сберстрахование. 1.Оформление. XPath-ы  

## Логотип «Сберстрахование»  
//div[@class='header_logo']

## Условия страхования  
-	Чек-бокс Залог Сбербанка  
//label[@for='mat-checkbox-3-input']//span[@class='mat-checkbox-inner-container']

## Данные страхователя  
-	Хедер Данные страхователя   
//h4[contains(text(),'Данные страхователя')]  
-	Кнопка Юридическое лицо   
//\*[@id="mat-button-toggle-1-button"]    
-	Кнопка Индивидуальный предприниматель   
//\*[@id="mat-button-toggle-2-button"]   
-	Чек-бокс Заполнить вручную   
//mat-checkbox[contains(@formcontrolname,'isManual')]//input[contains(@type,'checkbox')]    
-	Поле поиска Наименования(ФИО)/ИНН/ОГРН  
//input[contains(@placeholder,'ИНН/ОГРН')]   

## Юр. Лицо
-	Поле Страна регистрации   
//input[contains(@placeholder,'Страна')]  
-	Поле Полное наименование   
//input[contains(@data-placeholder,'Полное наименование')]  
-	Поле ИНН   
//input[contains(@data-placeholder,'ИНН')]  
-	Поле КПП   
//input[contains(@data-placeholder,'КПП')]  
-	Поле ОГРН   
//input[contains(@data-placeholder,'ОГРН')]  
-	Поле Регион   
//input[contains(@data-placeholder,'Регион') and contains(@formcontrolname,'registration')]    
-	Поле Город или населённый пункт   
//input[contains(@data-placeholder,'Город') and contains(@formcontrolname,'registration')]  
-	Поле Улица   
//input[contains(@data-placeholder,'Улица') and contains(@formcontrolname,'registration')]  
-	Чек-бокс Улица отсутствует   
//label[@for='mat-checkbox-2-input']//span[@class='mat-checkbox-inner-container']    
-	Поле Дом, литер, корпус   
//input[contains(@data-placeholder,'Дом') and contains(@formcontrolname,'registration')]  
-	Поле Офис, помещение   
//input[contains(@data-placeholder,'Офис') and contains(@formcontrolname,'registration')]  

## Индивидуальный предприниматель
- Кнопка Гражданин РФ   
//span[contains(text(),'Гражданин РФ')]/..  
- Кнопка Иностранный гражданин   
//span[contains(text(),'Иностранный гражданин')]/..  
- Фамилия   
//input[@data-placeholder='Фамилия']  
- Имя   
//input[@data-placeholder='Имя']  
- Отчество   
//input[@data-placeholder='Отчество']  
- Чек-бокс Отчество отсутствует   
//label[@for='mat-checkbox-22-input']//span[@class='mat-checkbox-inner-container']  
- Поле Дата рождения   
//input[@data-mat-calendar='mat-datepicker-4']  
- Датапикер Дата рождения   
//mat-datepicker-toggle[@class='mat-datepicker-toggle ng-tns-c65-183']//span[@class='mat-button-wrapper']  
- Кнопка Мужской   
//span[contains(text(),'Мужской')]/..    
- Кнопка Женский   
//span[contains(text(),'Женский')]/..    
- Поле ОГРНИП   
//input[contains(@data-placeholder,'ОРНИП')]

## Имущество, подлежащее страхованию  
## Территория страхования 
### Адрес имущества
-	Чек-бокс Андрес имущества совпадает с адресом регистрации   
//label[@for='mat-checkbox-3-input']//span[@class='mat-checkbox-inner-container']   
-	Поле Регион   
//input[contains(@data-placeholder,'Регион') and contains(@formcontrolname,'property')]  
-	Поле Город   
//input[contains(@data-placeholder,'Город') and contains(@formcontrolname,'property')]   
-	Поле Улица   
//input[contains(@data-placeholder,'Улица') and contains(@formcontrolname,'property')]   
-	Чек-бокс Улица отсутствует   
//label[@for='mat-checkbox-17-input']//span[@class='mat-checkbox-inner-container']   
-	Поле Дом   
//input[contains(@data-placeholder,'Дом') and contains(@formcontrolname,'property')]     
-	Поле Офис, помещение, кадастровый номер, территориальный ориентир  
//input[contains(@data-placeholder,'Офис') and contains(@formcontrolname,'property')]      

### Вид деятельности 
-	Поле Класс опасности   
//input[contains(@data-placeholder,'Класс опасности')]  
-	Поле Требование к АПС   
//input[contains(@data-placeholder,'АПС')]  

### Декларация страхователя

Является законсервированным, под реконструкцией, незавершенным строительством
- Кнопка «Да»  
//\*[@id="mat-button-toggle-10"]\
- Кнопка «Нет» -   
//\*[@id="mat-button-toggle-11"]\  

Является некапитальным зданием/сооружением без фундамента, воздухоопорной и/или надувной конструкцией
-	Кнопка «Да» -   
//\*[@id="mat-button-toggle-12-button"]  
-	Кнопка «Нет» -   
//\*[@id="mat-button-toggle-13-button"]  

На объекте отсутствуют первичные средства пожаротушения (огнетушители / пожарный кран / пожарный водопровод) или их количество и состояние не соответствуют действующим нормам пожарной безопасности РФ 
-	Кнопка «Да» -   
//\*[@id="mat-button-toggle-14-button"]  
-	Кнопка «Нет» -   
//\*[@id="mat-button-toggle-15-button"]  

Имеет не исполненные предписания МЧС и/или Ростехнадзора на начало страхования
-	Кнопка «Да» -   
//\*[@id="mat-button-toggle-16-button"]  
-	Кнопка «Нет» -   
//*[@id="mat-button-toggle-17-button"]  

Расположено в зоне объявленной чрезвычайной ситуации 
- Кнопка «Да» -   
//\*[@id="mat-button-toggle-18-button"]  
-	Кнопка «Нет» -   
//*[@id="mat-button-toggle-19-button"]  

Является рынком (совокупность отдельно стоящих или примыкающих друг к другу строений, расположенных на одной территории); отдельностоящей баней/сауной/бассейном; памятником истории/культуры/архитектуры 
-	Кнопка «Да» -   
//\*[@id="mat-button-toggle-20-button"]  
-	Кнопка «Нет» -   
//*[@id="mat-button-toggle-21-button"]  

Имеется неузаконенная перепланировка / реконструкция объекта в части капитальной конструкции и инженерных систем 
-	Кнопка «Да» -   
//\*[@id="mat-button-toggle-22-button"]  
-	Кнопка «Нет» -   
//*[@id="mat-button-toggle-23-button"]  

## Информация по территории страхования

-	Поле Год постройки здания или последний кап ремонт -   
//*\[@id="mat-input-9"]  

### Объект 1  
- Поле Расшифровка названия объекта -   
//\*[@id="mat-input-22"]  
- Поле Офис/помещение -   
//\*[@id="mat-input-23"]  
- Поле Кадастровый номер -   
//\*[@id="mat-input-24"]  
- Поле Площадь объекта -   
//\*[@id="mat-input-25"]  
- Поле Страховая сумма -   
//\*[@id="mat-input-26"]  
Поле Страховая стоимость -   
//\*[@id="mat-input-27"]  

- кнопка "добавить обьект" 
//span[text()=' Добавить объект ']/..  
- кнопка "удалить обьект" 
//span[contains(text(),' Удалить объект')]/..  
- кнопка "удалить территорию"  
//span[contains(text(),' Удалить    территорию')]/..  
- кнопка "добавить территорию"    
//span[text()=' Добавить территорию ']/..

## Срок страхования:  
- Датапикер «Дата начала страхования» -   
//mat-datepicker-toggle[@class='mat-datepicker-toggle ng-tns-c65-0'] 
- Окно ввода даты -   
//input[@id='mat-input-0']  
- Слайдер «Количество месяцев» –   
//mat-slider[@role='slider']  
- Окно ввода количества месяцев -   
//input[@id='mat-input-6']

## Контактная информация:  
- Телефон –   
//mat-form-field[@type='phone']   
- Электронная почта –   
//input[@id='mat-input-2']
- Дополнительная электронная почта –   
//input[@id='mat-input-3']

## Дополнительные расходы и риски:  
- Чек-бокс «внезапные и непредвиденные расходы по расчистке территории от последствий возникновения ущерба» -   
//label[@for='mat-checkbox-10-input']/../..  
- чек-бокс «Внезапные и непредвиденные расходы по ограждению, укреплению, обшивке материалами, герметизации или поддержке зданий, сооружений или застрахованного имущества для обеспечения их безопасности»  
//label[@for='mat-checkbox-11-input']/../..
 - чек-бокс «расходы на перемещение и защиту»  
 //label[@for='mat-checkbox-12-input']/../..
- чек-бокс «расходы по благоустройству территории»  
//label[@for='mat-checkbox-13-input']/../..
- чек-бокс «расходы по замене ключей, замков, мастер-ключей и т.д.(в случае их хищения)»  
//label[@for='mat-checkbox-14-input']/../..  

## Дополнительные риски:
- Чек-бокс «покрытие по риску терроризм»  
//mat-checkbox[@id='mat-checkbox-5']    
//span[contains(text(),'Покрытие по риску терроризм')]/../..
- чек-бокс «покрытие по риску диверсия»  
//mat-checkbox[@id='mat-checkbox-6']/..
- чек-бокс «покрытие по риску народные волнения»  
//mat-checkbox[@id='mat-checkbox-7']/..
- чек-бокс «покрытие по риску бой стекол»  
//mat-checkbox[@id='mat-checkbox-8']/..
 - чек-бокс «покрытие по риску не капитальные ремонт»  
 //mat-checkbox[@id='mat-checkbox-9']/..  
- Кнопка «Рассчитать»   
//span[text()=' Рассчитать ']/..
- Поле «франшиза» -   
//input[@id=’mat-input-4’]/..  
- Кнопка «применить»  
//input[@id='mat-input-4']/../../../../../..//button 
- Поле «введите промокод» -   
//input[@id=’mat-input-5’]/..  
- Кнопка «применить»  
//input[@id='mat-input-5']/../../../../../..//button   
//input[@id='mat-input-5']//ancestor::div[@class='contact-form__contact-item']//button

## Стоимость и срок действия:  
- Кнопка «назад»  
//span[text()='Назад']/.. 
- Кнопка «оформить полис»  
//span[text()=' Оформить полис']/..
