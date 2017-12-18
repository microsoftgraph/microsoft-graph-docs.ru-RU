# <a name="get-started-with-microsoft-graph-in-a-python-app"></a>Начало работы с Microsoft Graph в приложении Python 

В этой статье описано, как получить маркер доступа из Azure AD и вызвать Microsoft Graph. Из нее вы узнаете, как [отправить почту через Microsoft Graph из приложения Python](https://github.com/microsoftgraph/python-sample-send-mail), и что необходимо для использования API Microsoft Graph. В этой статье описано, как получить доступ к Microsoft Graph, используя прямые вызовы REST.

![Форма отправки почты](https://raw.githubusercontent.com/microsoftgraph/python-sample-send-mail/master/static/images/sendmail.png)

## <a name="choosing-an-authentication-library"></a>Выбор библиотеки аутентификации

Для вызова Microsoft Graph приложение должно получить действительный маркер доступа из Azure Active Directory (Azure AD) — облачной службы идентификации Майкрософт. Маркер необходимо передавать в заголовке HTTP каждого вызова REST API Microsoft Graph. Подход к аутентификацию, реализованный в Graph, основан на стандартах OAuth 2.0 и Open ID Connect, поэтому доступен широкий выбор [библиотек аутентификации](https://docs.microsoft.com/ru-RU/azure/active-directory/develop/active-directory-v2-libraries).

В приведенном ниже примере используется библиотека [Flask-OAuthlib](https://flask-oauthlib.readthedocs.io/en/latest/) для реализации рабочего процесса OAuth 2.0 с [предоставлением кода авторизации](https://tools.ietf.org/html/rfc6749#section-4.1), который рекомендуется использовать для веб-приложений, написанных на Python. Информацию о других способах аутентификации см. в [примерах аутентификации на Python для Microsoft Graph](https://github.com/microsoftgraph/python-sample-auth).

## <a name="installing-and-running-the-send-mail-sample"></a>Установка и запуск примера приложения для отправки почты

Чтобы установить и настроить пример приложения, выполните действия, описанные в статье [Установка примеров Python REST](https://github.com/microsoftgraph/python-sample-auth/blob/master/installation.md). Чтобы использовать рассматриваемый ниже пример, клонируйте репозиторий с помощью следующей команды:

    ```git clone https://github.com/microsoftgraph/python-sample-send-mail.git```

Регистрируя приложение, как описано в [инструкциях по установке](https://github.com/microsoftgraph/python-sample-auth/blob/master/installation.md), обязательно включите разрешения **User.Read** и **Mail.Send**, которые необходимы для этого примера.

После установки и настройки вы можете запустить пример приложения, следуя [этим инструкциям](https://github.com/microsoftgraph/python-sample-send-mail#running-the-sample).

## <a name="code-walkthrough"></a>Разбор кода

Ниже приведен обзор [исходного кода](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py) примера приложения.

Первые несколько строк кода предназначены для [импорта](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L4-L11) модулей и пакетов Python, используемых в примере.

* Модуль **base64** из стандартной библиотеки используется для кодирования вложений электронной почты.
* Модуль **pprint** из стандартной библиотеки используется для структурированного вывода сообщений об ошибках, которые возвращает Graph, например при попытке отправить сообщение на недействительный электронный адрес.
* Модуль **uuid** из стандартной библиотеки используется для создания случайной строки длиной 36 символов, однозначно определяющей каждый запрос Graph. Это может быть полезно для отладки.
* Пакет **flask** — это веб-платформа для примера.
* Класс **OAuth** в файле **flask_oauthlib.client** — это оболочка для приложения Flask, в котором реализуется рабочий процесс аутентификации OAuth 2.0.
* Модуль **config** содержит параметры регистрации приложения, настроенные в описанном выше процессе установки.

После этого мы [создаем приложение Flask](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L13-L15) и [объект клиента Graph](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L17-L26) под названием **MSGRAPH**.

За этими операциями для первоначальной настройки следуют три функции обработчика маршрута Flask, реализующие рабочий процесс аутентификации: [homepage()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L28-L31), [login()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L33-L37) и [authorized()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L39-L46). Дополнительные сведения о рабочем процессе аутентификации см. в разделе [Пример архитектуры](https://github.com/microsoftgraph/python-sample-auth#sample-architecture) репозитория примеров аутентификации на Python.

Следующий обработчик маршрута, [mailform()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L48-L54), — это форма для указания получателей, темы и текста сообщения. Обратите внимание, что эта функция также включает наш первый вызов Graph: [получение профиля пользователя](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L51-L51) для получения отображаемого имени и электронного адреса текущего пользователя, которые [передаются в шаблон mailform.html](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L52-L54).

За ним следует функция [send_mail()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L56-L73), которая отправляет сообщение и показывает ответ от API Graph. Она использует вспомогательную функцию sendmail(), передавая в нее параметры строки запроса, опубликованные из формы:

```python
response = sendmail(MSGRAPH,
                    subject=flask.request.args['subject'],
                    recipients=flask.request.args['email'].split(';'),
                    html=flask.request.args['body'])
```

Функция [get_token()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L75-L78) используется экземпляром клиента Flask-OAuthlib (```MSGRAPH```) для получения маркера доступа при каждом вызове Graph. Маркер доступа передается в заголовке HTTP **Authorization**, но в данном случае нам не нужно его использовать. Вы можете просто вызывать Graph с помощью методов HTTP, например get() или post(), а экземпляр клиента будет вызывать метод ```get_token()``` для получения маркера, так как функция [содержит](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L75-L75) атрибут ```tokengetter```.

За ним следует метод [request_headers()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L80-L85), возвращающий словарь заголовков HTTP, отправляемых с каждым вызовом Graph.

Наконец, у нас есть [sendmail()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L87-L129) — вспомогательная функция для отправки сообщения. Она отправляет сообщение с помощью конечной точки ```me/microsoft.graph.sendMail``` в API Microsoft Graph. Вы можете использовать эту функцию в своем коде, чтобы отправить сообщение с помощью Microsoft Graph. Сведения о том, как вызывать эту функцию, см. [здесь](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L88-L97).

## <a name="other-python-rest-samples"></a>Другие примеры Python REST

Приведенные ниже примеры демонстрируют, как работать с другими функциями Microsoft Graph из Python:

* [Примеры аутентификации на Python для Microsoft Graph](https://github.com/microsoftgraph/python-sample-auth)
* [Работа с разбитыми на страницы ответами Microsoft Graph в Python](https://github.com/microsoftgraph/python-sample-pagination)
* [Работа с открытыми расширениями Graph в Python](https://github.com/microsoftgraph/python-sample-open-extensions)

Разместить заявку на пример можно [здесь](https://github.com/microsoftgraph/python-sample-auth/issues). Мы будем рады узнать, какие сценарии Microsoft Graph вы хотели бы реализовать на Python!

API Microsoft Graph — единый мощный API, с помощью которого можно взаимодействовать со всеми типами данных Майкрософт. Чтобы узнать больше о возможностях Microsoft Graph, ознакомьтесь с [документацией для разработчиков](https://developer.microsoft.com/ru-RU/graph/docs/concepts/overview) или опробуйте [песочницу Graph](https://developer.microsoft.com/ru-RU/graph/graph-explorer).
