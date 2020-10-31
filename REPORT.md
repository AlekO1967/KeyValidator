# Отчёт о тестировании OpenJDK 11
## Установка OpenJDK 11 на операционную систему Windows 10

30.10.2020 г. - 30.10.2020 г. было проведено тестирование установки приложения JDK.

На тестирование затрачено: 0,5 часа

В результате тестирования дефекты не выявлены

## Описание процесса тестирования

В качестве тестовых данных использовались данные из [Инструкции по установке OpenJDK 11](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/openjdk11-manual.md):
* Открыть браузер Google Chrom, ожидаемый результат открывается бразуер Google Chrom;

* Ввести в поисковую строку адрес сайта https://adoptopenjdk.net/, ожидаемый результат - открывается страница AdoptopenJDK;

* Выбрать опции, как на скриншоте и нажать кнопку "Latest release", 
ожидаемый результат - запускается скачивание MCI-файла; 
![](https://raw.githubusercontent.com/netology-code/javaqa-homeworks/master/intro/pic/win-adoptopenjdk.png) 


* Запустить на установку скачанный MSI-файл и нажать кнопку "Next", ожидаемый результат - окрывается окно; ![](https://raw.githubusercontent.com/netology-code/javaqa-homeworks/master/intro/pic/win-step1.png)

* Нажать кнопку "Next", ожидаемый результат - открывается окно; ![](https://raw.githubusercontent.com/netology-code/javaqa-homeworks/master/intro/pic/win-step2.png)

* Прочитать, согласиться с условиями лицензии и нажать кнопку "Next", ожтдаемый результат открывается окно; ![](https://raw.githubusercontent.com/netology-code/javaqa-homeworks/master/intro/pic/win-step3.png)

* Выбрать опции, как на экране (удостовериться, что установка происходит в Program Files и опция Add to PATH выбрана), нажать кнопку "Next", ожидаемый результат - откроется окно;

![](https://raw.githubusercontent.com/netology-code/javaqa-homeworks/master/intro/pic/win-step4.png)

* Нажать кнопку "Install" и дождаться окончания установки, ожидаемый результат откроется окно;
![](https://raw.githubusercontent.com/netology-code/javaqa-homeworks/master/intro/pic/win-step5.png)

* нажать кнопку "Finish", ожидаемый результат - установка завершена, окно погаснет;

* перегрузить компьютер;

* открыть терминал и запустить команду
  java -version, 
  
  ожидаемый результат - 
  
  openjdk version "11.0.5" 2019-10-15
  
  OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.5+10)
  
  OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.5+10, mixed mode);

  фактический результат -

  openjdk version "11.0.9" 2020-10-20

  OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.9+11)

  OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.9+11, mixed mode)

Тестирование производилось в следующем окружении:
* Windows 10, 64-разрядная операционная система
* версия JDK "11.0.9" 2020-10-20
* Google Chrom Версия 86.0.4240.111 (Официальная сборка), (64 бит)