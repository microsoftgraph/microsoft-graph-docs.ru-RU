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

Первые несколько строк кода предназначены для [импорта](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L4-L32) модулей и пакетов Python, используемых в примере:

* Модуль **base64** из стандартной библиотеки используется для кодирования вложений электронной почты.
* Модуль **mimetypes** позволяет определить тип MIME для вложенных файлов.
* Модуль **os** обеспечивает общую функциональность файловой системы.
* Модуль **pprint** из стандартной библиотеки используется для структурированного вывода сообщений об ошибках, которые возвращает Graph, например при попытке отправить сообщение на недействительный электронный адрес.
* Модуль **uuid** из стандартной библиотеки используется для создания случайной строки длиной 36 символов, однозначно определяющей каждый запрос Graph. Это может быть полезно для отладки.
* Пакет **flask** — это веб-платформа для примера.
* Класс **OAuth** в файле **flask_oauthlib.client** — это оболочка для приложения Flask, в котором реализуется рабочий процесс аутентификации OAuth 2.0.
* Модуль **config** содержит параметры регистрации приложения, настроенные в описанном выше процессе установки.

После этого мы [создаем приложение Flask](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L15-L17) и [клиентский объект Graph](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L19-L28) под названием **MSGRAPH**.

За этими начальными этапами настройки следуют три функции обработчика маршрута Flask, реализующие рабочий процесс аутентификации: [homepage()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L30-L33), [login()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L35-L39) и [authorized()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L41-L48). Дополнительные сведения о рабочем процессе аутентификации см. в разделе [Пример архитектуры](https://github.com/microsoftgraph/python-sample-auth#sample-architecture) репозитория примеров аутентификации на Python.

Следующий обработчик маршрута, [mailform()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L50-L83), — это форма для указания получателей, темы и текста сообщения. Обратите внимание на то, что эта функция также включает наши первые вызовы Graph (в том числе получает профиль пользователя и фотографию профиля, отправляет ее в OneDrive и создает ссылку для доступа). Данные [передаются в шаблон mailform.html](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L77-L83), в котором получателя, тему и текст сообщения можно изменить перед отправкой. 

За ним следует функция [send_mail()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L85-L107), которая отправляет сообщение и показывает ответ API Graph. Она использует вспомогательную функцию sendmail(), передавая в нее параметры строки запроса, опубликованные из формы:

```python
response = sendmail(client=MSGRAPH,
                    subject=flask.request.args['subject'],
                    recipients=flask.request.args['email'].split(';'),
                    body=flask.request.args['body'],
                    attachments=[profile_pic])
```

Функция [get_token()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L109-L123) используется экземпляром клиента Flask-OAuthlib (```MSGRAPH```) для получения маркера доступа при каждом вызове Graph. Маркер доступа передается в заголовке HTTP **Authorization**, но в данном случае нам не нужно его использовать. Вы можете просто вызывать Graph с помощью методов HTTP клиента, например get() или post(), а экземпляр клиента будет вызывать ```get_token()``` для получения маркера, так как функция [содержит](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L109-L109) ```tokengetter```.

Остальная часть примера состоит из вспомогательных функций, упрощающих основные действия Graph:

* [request_headers()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L114-L123) возвращает словарь HTTP-заголовков, отправляемых с каждым вызовом Graph.
* [profile_photo()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L125-L154) возвращает фотографию профиля пользователя и при необходимости сохраняет копию в локальном файле.
* [sendmail()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L156-L202) отправляет сообщение, используя конечную точку ```me/microsoft.graph.sendMail```.
* [sharing_link()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L204-L221) создает ссылку для доступа к указанному элементу OneDrive.
* [upload_file()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L223-L255) отправляет файл в OneDrive.

Эти вспомогательные функции могут пригодиться вам в других приложениях.

## <a name="other-python-rest-samples"></a>Другие примеры кода на Python REST

Вот некоторые примеры кода на Python, демонстрирующие работу с различными аспектами Microsoft Graph:

* [Примеры кода аутентификации на Python для Microsoft Graph](https://github.com/microsoftgraph/python-sample-auth)
* [Работа с разбитыми на страницы ответами Microsoft Graph в Python](https://github.com/microsoftgraph/python-sample-pagination)
* [Работа с открытыми расширениями Graph в Python](https://github.com/microsoftgraph/python-sample-open-extensions)
* [Подключение веб-приложения Python к API безопасности](https://github.com/microsoftgraph/python-security-rest-sample)

Если вы бы хотели увидеть конкретный пример, [отправьте нам заявку](https://github.com/microsoftgraph/python-sample-auth/issues). Мы будем рады узнать, какие сценарии Microsoft Graph вы хотели бы реализовать на Python!

API Microsoft Graph — единый мощный API, с помощью которого можно взаимодействовать со всеми типами данных Майкрософт. Чтобы узнать больше о возможностях Microsoft Graph, ознакомьтесь с [документацией для разработчиков](https://developer.microsoft.com/ru-RU/graph/docs/concepts/overview) или опробуйте [песочницу Graph](https://developer.microsoft.com/ru-RU/graph/graph-explorer).
