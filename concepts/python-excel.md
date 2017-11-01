# <a name="use-microsoft-graph-to-access-excel-in-a-python-app"></a>Использование Microsoft Graph для доступа к Excel в приложении на Python

С помощью API Microsoft Graph можно читать и обновлять книги в поддерживаемых интернет-хранилищах, в том числе OneDrive и SharePoint. Ресурс `Workbook` (или файл Excel) содержит все другие ресурсы Excel, и ваше приложение может получать к ним доступ с помощью простых переходов. 

Вы можете получить доступ к набору объектов Excel (например, Table, Range или Chart) с помощью стандартных REST API, чтобы выполнять с книгой операции CRUD (создание, чтение, обновление и удаление). Например, `https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`  
возвращает коллекцию объектов листа, включенных в книгу.    

В этом пошаговом руководстве описано, как отправлять запросы в REST API для Excel из веб-приложения на Python. 

##  <a name="prerequisites"></a>Необходимые условия

* [Python 3.5.2](https://www.python.org/downloads/)
* [Flask-OAuthlib](https://github.com/lepture/flask-oauthlib)
* [Рабочая или учебная учетная запись](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account)<!-- This link target doesn't match the link title. Please verify that this is what you want to link to and update the text, or update the URL as appropriate. -->


## <a name="authorization-and-scopes"></a>Авторизация и области
Для аутентификации вызовов REST API для Excel можно использовать [конечную точку Azure AD 2.0](https://graph.microsoft.io/en-us/docs/concepts/converged_auth). Для всех API требуется заголовок HTTP `Authorization: Bearer {access-token}`.   
  
Для использования ресурса Excel требуется одна из следующих [областей разрешений](https://graph.microsoft.io/en-us/docs/concepts/permissions_reference):

* Files.Read; 
* Files.ReadWrite.

## <a name="sessions-and-persistence"></a>Сеансы и сохраняемость

Интерфейсы API Excel можно вызвать в одном из двух режимов. 

1. Постоянный сеанс — все изменения, внесенные в книгу, сохраняются (сохраненные). Это обычный режим работы. 
2. Временный сеанс — изменения, внесенные интерфейсом API, не сохраняются в исходном расположении. Вместо этого внутренний сервер Excel сохраняет временную копию файла, в которой отражены изменения, внесенные во время конкретного сеанса API. Когда истечет срок действия сеанса Excel, изменения будут потеряны. Этот режим удобен для приложений, которым нужно выполнять анализ или получать результаты вычислений или изображение диаграммы, не изменяя состояние документа.   

Чтобы представить сеанс в API, воспользуйтесь заголовком `workbook-session-id: {session-id}`. 

## <a name="register-the-application-in-azure-active-directory"></a>Регистрация приложения в Azure Active Directory

Для начала необходимо зарегистрировать приложение и задать разрешения на использование Microsoft Graph. Это позволяет пользователям входить в приложение с помощью рабочих или учебных учетных записей.

### <a name="register-the-application"></a>Регистрация приложения

Зарегистрируйте приложение на портале регистрации приложений Майкрософт. При этом будут созданы пароль и идентификатор приложения, с помощью которых вы настроите приложение для проверки подлинности.

1. Войдите на [портал регистрации приложений Майкрософт](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи. 

2. Нажмите кнопку **Добавить приложение**.

3. Введите имя приложения и нажмите кнопку **Создать приложение**.

    Откроется страница регистрации со свойствами приложения.

4. Скопируйте идентификатор приложения. Это уникальный идентификатор приложения.

5. В разделе **Секреты приложения** нажмите кнопку **Создать новый пароль**. Скопируйте секрет приложения из диалогового окна **Новый пароль создан**.

    Идентификатор и секрет приложения используются для его настройки.

6. В разделе **Платформы** выберите **Добавление платформы** > **Веб**.

7. Установите флажок **Разрешить неявный поток** и введите URI перенаправления приложения.

    Параметр **Разрешить неявный поток** включает гибридный поток OpenID Connect. Благодаря этому при аутентификации приложение может получить данные для входа (**id_token**) и артефакты (в данном случае — код авторизации), с помощью которых оно может получить маркер доступа.

8. Нажмите кнопку **Сохранить**.

### <a name="create-oauth-client"></a>Создание клиента OAuth

Приложение должно зарегистрировать экземпляр клиента Flask-OAuth, который будет использоваться для запуска потока OAuth и получения маркера доступа. Обратите внимание, что для получения сеанса Excel, который поддерживает сохраняемые изменения, необходима область *Files.ReadWrite*.

```python
    # Put your consumer key and consumer secret into a config file
    # and don't check it into github!
    microsoft = oauth.remote_app(
        'microsoft',
        consumer_key = client_id,
        consumer_secret = client_secret,
        request_token_params = {'scope': 'User.Read Files.ReadWrite'},
        base_url = 'https://graph.microsoft.com/v1.0/',
        request_token_url = None,
        access_token_method = 'POST',
        access_token_url = 'https://login.microsoftonline.com/common/oauth2/v2.0/token',
        authorize_url = 'https://login.microsoftonline.com/common/oauth2/v2.0/authorize'
    )
```

### <a name="receive-an-authorization-code-in-your-reply-url-page"></a>Получение кода авторизации на странице URL-адреса ответа

После входа пользователя браузер перенаправляется на URL-адрес отклика. После успешной авторизации в теле отклика возвращается маркер доступа (он будет использоваться для авторизации дополнительных запросов). 

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
```

## <a name="make-requests-to-the-excel-api"></a>Отправка запросов к API Excel

### <a name="request-headers"></a>Заголовки запросов 
Используя токен доступа, приложение может отправлять проверенные запросы в API Microsoft Graph. Приложение должно добавлять токен доступа в заголовок **Authorization** каждого запроса.

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

### <a name="getting-an-excel-session"></a>Получение сеанса Excel
#### <a name="request"></a>Запрос 

Передайте объект JSON, задав `persistChanges` значение `true` или `false`. Если для параметра `persistChanges` установлено значение `false`, возвращается идентификатор непостоянного сеанса. В этом примере используется библиотека HTTP [Requests](http://docs.python-requests.org/en/latest/user/quickstart). 

```python
    # Replace the id with your Excel workbook's drive id
    url = 'https://graph.microsoft.com/v1.0/me/drive/items/01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE/workbook/createSession'
    # Set request headers
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
        'Accept' : 'application/json',
        'Content-Type' : 'application/json'
    }
    # Specify type of session
    body = {
        'persistChanges': True
    }
    
    response = requests.post(url, headers = headers, json = body)
```

#### <a name="response"></a>Отклик

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/{version}/$metadata#microsoft.graph.sessionInfo",
    "id": "{session-id}",
    "persistChanges": true
}
```

#### <a name="usage"></a>Использование 

Идентификатор сеанса, возвращенный при предыдущем вызове, передается в качестве заголовка при последующих запросах API в HTTP-заголовке **Workbook-Session-Id**. Например, для перечисления листов в книге Excel.

```python
    # Replace the id with your Excel workbook's drive id
    url = 'https://graph.microsoft.com/v1.0/me/drive/items/01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE/workbook/worksheets'
    # Set request headers - note the session header 
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
        'Accept' : 'application/json',
        'Workbook-Session-Id': 'cluster=PP1&session=12.a04039942e021.A272...'
    }
    
    response = requests.get(url, headers = headers)
```

#### <a name="response"></a>Отклик

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('8473b867-3e4e-4e44-8d09-8c6da362080f')/drive/items('01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE')/workbook/worksheets",
    "value": [
    {
        "@odata.id": "/users('8473b867-3e4e-4e44-8d09-8c6da362080f')/drive/items('01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)",
        "id": "{00000000-0001-0000-0000-000000000000}",
        "name": "Session 1",
        "position": 0,
        "visibility": "Visible"
    },
    {
        "@odata.id": "/users('8473b867-3e4e-4e44-8d09-8c6da362080f')/drive/items('01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
        "id": "{00000000-0001-0000-0100-000000000000}",
        "name": "Session 2",
        "position": 1,
        "visibility": "Visible"
    }]
}
```

## <a name="next-steps"></a>Дальнейшие действия

С помощью HTTP-заголовка **Workbook-Session-Id** можно отправлять запросы на получение данных, создание диаграмм и многие другие. 

* [Обычные сценарии использования API Excel](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel#common-excel-scenarios)
* [Работа с Excel в Microsoft Graph](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel)

REST API для Excel в Microsoft Graph — это эффективный способ доступа к данным в книгах Excel и работы с ними. Узнайте о других возможностях Microsoft Graph.

* [Обзор Microsoft Graph](https://developer.microsoft.com/graph/docs)
* [Начало работы с Microsoft Graph в приложении на Python](https://developer.microsoft.com/graph/docs/get-started/python)
