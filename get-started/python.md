# <a name="get-started-with-microsoft-graph-in-a-python-app"></a>Начало работы с Microsoft Graph в приложении Python 

В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из Azure AD и вызвать Microsoft Graph. В ней описывается создание [примера Microsoft Graph Connect для Python](https://github.com/microsoftgraph/python3-connect-rest-sample), и рассматриваются основные понятия, которые необходимо реализовать для использования API Microsoft Graph. В этой статье рассказывается, как получить доступ к Microsoft Graph с помощью прямых вызовов REST.

![Снимок экрана приложения Python Connect для Office 365](./images/web-screenshot.png)

##  <a name="prerequisites"></a>Необходимые условия

* [Python 3.5.2](https://www.python.org/downloads/)
* [Flask-OAuthlib](https://github.com/lepture/flask-oauthlib)
* [Flask-Script 0.4](http://flask-script.readthedocs.io/en/latest/)
* [Учетная запись Майкрософт](https://www.outlook.com/) или [учетная запись Office 365 для бизнеса](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account).
* [Пример Microsoft Graph Connect для Python](https://github.com/microsoftgraph/python3-connect-rest-sample)

## <a name="register-the-application-in-azure-active-directory"></a>Регистрация приложения в Azure Active Directory

Для начала необходимо зарегистрировать приложение и задать разрешения на использование Microsoft Graph. Это позволяет пользователям входить в приложение с помощью рабочих или учебных учетных записей.

## <a name="register-the-application"></a>Регистрация приложения

Зарегистрируйте приложение на портале регистрации приложений Майкрософт. При этом будут созданы пароль и идентификатор приложения, с помощью которых вы настроите приложение для проверки подлинности.

1. Войдите на [портал регистрации приложений Майкрософт](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.

2. Нажмите кнопку **Добавить приложение**.

3. Введите имя приложения и нажмите кнопку **Создать приложение**.

    Откроется страница регистрации со свойствами приложения.

4. Скопируйте идентификатор приложения. Это уникальный идентификатор приложения.

5. В разделе **Секреты приложения** нажмите кнопку **Создать новый пароль**. Скопируйте секрет приложения из диалогового окна **Новый пароль создан**.

    Идентификатор и секрет приложения используются для его настройки.

6. В разделе **Платформы** выберите **Добавление платформы** > **Интернет**.

7. Убедитесь, что установлен флажок **Разрешить неявный поток** и введите URI перенаправления *http://localhost:5000/login/authorized*.

    Параметр **Разрешить неявный поток** включает гибридный поток OpenID Connect. Благодаря этому при проверке подлинности приложение может получить данные для входа (**id_token**) и артефакты (в данном случае — код авторизации), с помощью которых оно может получить маркер доступа.

    URI перенаправления *http://localhost:5000/login/authorized* — это значение, которое ПО промежуточного слоя OmniAuth использует после обработки запроса аутентификации.

8. Нажмите кнопку **Сохранить**.

## <a name="create-oauth-client"></a>Создание клиента OAuth

Приложение должно зарегистрировать экземпляр клиента Flask-OAuth, который будет использоваться для запуска потока OAuth и получения маркера доступа. 

В примере Connect приведенный ниже код (расположенный в файле [*connect/__init__.py*](https://github.com/microsoftgraph/python3-connect-rest-sample/blob/master/connect/__init__.py)) регистрирует клиент с использованием всех обязательных значений, в том числе идентификатора приложения (client_id), секрета приложения (client_secret) URL-адреса авторизации, используемого для аутентификации пользователя.

```python
    # Put your consumer key and consumer secret into a config file
    # and don't check it into github!!
    microsoft = oauth.remote_app(
        'microsoft',
        consumer_key=client_id,
        consumer_secret=client_secret,
        request_token_params={'scope': 'User.Read Mail.Send'},
        base_url='https://graph.microsoft.com/v1.0/',
        request_token_url=None,
        access_token_method='POST',
        access_token_url='https://login.microsoftonline.com/common/oauth2/v2.0/token',
        authorize_url='https://login.microsoftonline.com/common/oauth2/v2.0/authorize'
    )
```

<!--<a name="authCode"></a>-->
## <a name="receive-an-authorization-code-in-your-reply-url-page"></a>Получение кода авторизации на странице URL-адреса ответа

После входа пользователя в браузере открывается URL-адрес ответа, маршрут ```login/authorized``` в файле [*connect/__init__.py*](https://github.com/microsoftgraph/python3-connect-rest-sample/blob/master/connect/__init__.py), с маркером доступа в ответе. Приложение сохраняет маркер в переменной сеанса.

```python
    @app.route('/login/authorized')
    def authorized():
        response = microsoft.authorized_response()
    
        if response is None:
            return "Access Denied: Reason=%s\nError=%s" % (
                request.args['error'], 
                request.args['error_description']
            )
    
        # Check response for state
        if str(session['state']) != str(request.args['state']):
            raise Exception('State has been messed with, end authentication')
        # Remove state session variable to prevent reuse.
        session['state'] = ""
            
        # Okay to store this in a local variable, encrypt if it's going to client
        # machine or database. Treat as a password. 
        session['microsoft_token'] = (response['access_token'], '')
        # Store the token in another session variable for easy access
        session['access_token'] = response['access_token']
        meResponse = microsoft.get('me')
        meData = json.dumps(meResponse.data)
        me = json.loads(meData)
        userName = me['displayName']
        userEmailAddress = me['userPrincipalName']
        session['alias'] = userName
        session['userEmailAddress'] = userEmailAddress
        return redirect('main')
```

<!--<a name="request"></a>-->
## <a name="use-the-access-token-in-a-request-to-the-microsoft-graph-api"></a>Использование маркера доступа в запросе к API Microsoft Graph

Используя токен доступа, приложение может отправлять проверенные запросы в API Microsoft Graph. Приложение должно добавлять токен доступа в заголовок **Authorization** каждого запроса.

Приложение Connect отправляет электронную почту, используя конечную точку ```me/microsoft.graph.sendMail``` в API Microsoft Graph. Код содержится в функции ```call_sendMail_endpoint``` в файле [*connect/graph_service.py*](https://github.com/microsoftgraph/python3-connect-rest-sample/blob/master/connect/graph_service.py). Этот код показывает, как добавить код доступа в заголовок "Authorization".

```python
    # Set request headers.
    headers = { 
      'User-Agent' : 'python_tutorial/1.0',
      'Authorization' : 'Bearer {0}'.format(access_token),
      'Accept' : 'application/json',
      'Content-Type' : 'application/json'
    }
```

> **Примечание**. В запросе необходимо также отправлять заголовок **Content-Type** со значением, принимаемым API Graph, например `application/json`.

API Microsoft Graph — это мощный единый API, с помощью которого можно взаимодействовать со всеми типами данных корпорации Майкрософт. Сведения о других возможностях API Microsoft Graph см. в справочнике по API.