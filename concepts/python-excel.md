# <a name="use-microsoft-graph-to-access-excel-in-a-python-app"></a><span data-ttu-id="aef16-101">Использование Microsoft Graph для доступа к Excel в приложении на Python</span><span class="sxs-lookup"><span data-stu-id="aef16-101">Use Microsoft Graph to access Excel in a Python app</span></span>

<span data-ttu-id="aef16-102">С помощью API Microsoft Graph можно читать и обновлять книги в поддерживаемых интернет-хранилищах, в том числе OneDrive и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="aef16-102">You can use the Microsoft Graph API to read and update workbooks stored in supported online storage platforms including, OneDrive and SharePoint. The  (or Excel file) resource contains all the other Excel resources and your app can access them via simple navigations.</span></span> <span data-ttu-id="aef16-103">Ресурс `Workbook` (или файл Excel) содержит все другие ресурсы Excel, и ваше приложение может получать к ним доступ с помощью простых переходов.</span><span class="sxs-lookup"><span data-stu-id="aef16-103">You can use the Microsoft Graph API to read and update workbooks stored in supported online storage platforms including, OneDrive and SharePoint. The `Workbook` (or Excel file) resource contains all the other Excel resources and your app can access them via simple navigations.</span></span> 

<span data-ttu-id="aef16-104">Вы можете получить доступ к набору объектов Excel (например, Table, Range или Chart) с помощью стандартных REST API, чтобы выполнять с книгой операции CRUD (создание, чтение, обновление и удаление).</span><span class="sxs-lookup"><span data-stu-id="aef16-104">You can access a set of Excel objects (such as Table, Range, or Chart) by using standard REST APIs to perform  create, read, update, and delete (CRUD) operations on the workbook. For example, </span></span> <span data-ttu-id="aef16-105">Например, `https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`</span><span class="sxs-lookup"><span data-stu-id="aef16-105">For example:`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`</span></span>  
<span data-ttu-id="aef16-106">возвращает коллекцию объектов листа, включенных в книгу.</span><span class="sxs-lookup"><span data-stu-id="aef16-106">returns a collection of worksheet objects that are part of the workbook.</span></span>    

<span data-ttu-id="aef16-107">В этом пошаговом руководстве описано, как отправлять запросы в REST API для Excel из веб-приложения на Python.</span><span class="sxs-lookup"><span data-stu-id="aef16-107">This walkthrough describes how to make requests to the Excel REST API from a Python web app.</span></span> 

##  <a name="prerequisites"></a><span data-ttu-id="aef16-108">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="aef16-108">Prerequisites</span></span>

* [<span data-ttu-id="aef16-109">Python 3.5.2</span><span class="sxs-lookup"><span data-stu-id="aef16-109">Python 3.5.2</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="aef16-110">Flask-OAuthlib</span><span class="sxs-lookup"><span data-stu-id="aef16-110">Flask-OAuthlib</span></span>](https://github.com/lepture/flask-oauthlib)
* <span data-ttu-id="aef16-111">[Рабочая или учебная учетная запись](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account)<!-- This link target doesn't match the link title. Please verify that this is what you want to link to and update the text, or update the URL as appropriate. --></span><span class="sxs-lookup"><span data-stu-id="aef16-111">A [work or school account](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account)<!-- This link target doesn't match the link title. Please verify that this is what you want to link to and update the text, or update the URL as appropriate. --></span></span>


## <a name="authorization-and-scopes"></a><span data-ttu-id="aef16-112">Авторизация и области</span><span class="sxs-lookup"><span data-stu-id="aef16-112">Authorization and scopes</span></span>
<span data-ttu-id="aef16-113">Для аутентификации вызовов REST API для Excel можно использовать [конечную точку Azure AD 2.0](https://graph.microsoft.io/en-us/docs/concepts/converged_auth).</span><span class="sxs-lookup"><span data-stu-id="aef16-113">You can use the [Azure AD v2.0 endpoint](https://graph.microsoft.io/en-us/docs/concepts/converged_auth) to authenticate Excel REST API calls. All APIs require the  HTTP header.</span></span> <span data-ttu-id="aef16-114">Для всех API требуется заголовок HTTP `Authorization: Bearer {access-token}`.</span><span class="sxs-lookup"><span data-stu-id="aef16-114">All APIs require the `Authorization: Bearer {access-token}` HTTP header.</span></span>   
  
<span data-ttu-id="aef16-115">Для использования ресурса Excel требуется одна из следующих [областей разрешений](https://graph.microsoft.io/en-us/docs/concepts/permissions_reference):</span><span class="sxs-lookup"><span data-stu-id="aef16-115">One of the following [permission scopes](https://graph.microsoft.io/en-us/docs/concepts/permissions_reference) is required to use the Excel resource:</span></span>

* <span data-ttu-id="aef16-116">Files.Read;</span><span class="sxs-lookup"><span data-stu-id="aef16-116">Files.Read</span></span> 
* <span data-ttu-id="aef16-117">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="aef16-117">Files.ReadWrite</span></span>

## <a name="sessions-and-persistence"></a><span data-ttu-id="aef16-118">Сеансы и сохраняемость</span><span class="sxs-lookup"><span data-stu-id="aef16-118">Sessions and persistence</span></span>

<span data-ttu-id="aef16-119">Интерфейсы API Excel можно вызвать в одном из двух режимов.</span><span class="sxs-lookup"><span data-stu-id="aef16-119">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="aef16-p104">Постоянный сеанс — все изменения, внесенные в книгу, сохраняются (сохраненные). Это обычный режим работы.</span><span class="sxs-lookup"><span data-stu-id="aef16-p104">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="aef16-p105">Временный сеанс — изменения, внесенные интерфейсом API, не сохраняются в исходном расположении. Вместо этого внутренний сервер Excel сохраняет временную копию файла, в которой отражены изменения, внесенные во время конкретного сеанса API. Когда истечет срок действия сеанса Excel, изменения будут потеряны. Этот режим удобен для приложений, которым нужно выполнять анализ или получать результаты вычислений или изображение диаграммы, не изменяя состояние документа.</span><span class="sxs-lookup"><span data-stu-id="aef16-p105">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="aef16-126">Чтобы представить сеанс в API, воспользуйтесь заголовком `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="aef16-126">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

## <a name="register-the-application-in-azure-active-directory"></a><span data-ttu-id="aef16-127">Регистрация приложения в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="aef16-127">Register the application in Azure Active Directory</span></span>

<span data-ttu-id="aef16-p106">Для начала необходимо зарегистрировать приложение и задать разрешения на использование Microsoft Graph. Это позволяет пользователям входить в приложение с помощью рабочих или учебных учетных записей.</span><span class="sxs-lookup"><span data-stu-id="aef16-p106">First, you need to register your application and set permissions to use Microsoft Graph. This lets users sign in to the application with work or school accounts.</span></span>

### <a name="register-the-application"></a><span data-ttu-id="aef16-130">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="aef16-130">Register the application</span></span>

<span data-ttu-id="aef16-p107">Зарегистрируйте приложение на портале регистрации приложений Майкрософт. При этом будут созданы пароль и идентификатор приложения, с помощью которых вы настроите приложение для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="aef16-p107">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app for authentication.</span></span>

1. <span data-ttu-id="aef16-133">Войдите на [портал регистрации приложений Майкрософт](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи. </span><span class="sxs-lookup"><span data-stu-id="aef16-133">Sign in to the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="aef16-134">Нажмите кнопку **Добавить приложение**.</span><span class="sxs-lookup"><span data-stu-id="aef16-134">Choose **Add an app**.</span></span>

3. <span data-ttu-id="aef16-135">Введите имя приложения и нажмите кнопку **Создать приложение**.</span><span class="sxs-lookup"><span data-stu-id="aef16-135">Enter a name for the app, and choose **Create application**.</span></span>

    <span data-ttu-id="aef16-136">Откроется страница регистрации со свойствами приложения.</span><span class="sxs-lookup"><span data-stu-id="aef16-136">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="aef16-p108">Скопируйте идентификатор приложения. Это уникальный идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="aef16-p108">Copy the application ID. This is the unique identifier for your app.</span></span>

5. <span data-ttu-id="aef16-p109">В разделе **Секреты приложения** нажмите кнопку **Создать новый пароль**. Скопируйте секрет приложения из диалогового окна **Новый пароль создан**.</span><span class="sxs-lookup"><span data-stu-id="aef16-p109">Under **Application Secrets**, choose **Generate New Password**. Copy the app secret from the **New password generated** dialog box.</span></span>

    <span data-ttu-id="aef16-141">Идентификатор и секрет приложения используются для его настройки.</span><span class="sxs-lookup"><span data-stu-id="aef16-141">You'll use the application ID and app secret to configure the app.</span></span>

6. <span data-ttu-id="aef16-142">В разделе **Платформы** выберите **Добавление платформы** > **Веб**.</span><span class="sxs-lookup"><span data-stu-id="aef16-142">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="aef16-143">Установите флажок **Разрешить неявный поток** и введите URI перенаправления приложения.</span><span class="sxs-lookup"><span data-stu-id="aef16-143">Make sure the **Allow Implicit Flow** check box is selected, and enter your app's Redirect URI.</span></span>

    <span data-ttu-id="aef16-144">Параметр **Разрешить неявный поток** включает гибридный поток OpenID Connect.</span><span class="sxs-lookup"><span data-stu-id="aef16-144">The **Allow Implicit Flow** option enables the OpenID Connect hybrid flow.</span></span> <span data-ttu-id="aef16-145">Благодаря этому при аутентификации приложение может получить данные для входа (**id_token**) и артефакты (в данном случае — код авторизации), с помощью которых оно может получить маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="aef16-145">During authentication, this enables the app to receive both sign-in info (the id_token) and artifacts (in this case, an authorization code) that the app can use to obtain an access token.</span></span>

8. <span data-ttu-id="aef16-146">Нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="aef16-146">Choose **Save**.</span></span>

### <a name="create-oauth-client"></a><span data-ttu-id="aef16-147">Создание клиента OAuth</span><span class="sxs-lookup"><span data-stu-id="aef16-147">Create OAuth client</span></span>

<span data-ttu-id="aef16-148">Приложение должно зарегистрировать экземпляр клиента Flask-OAuth, который будет использоваться для запуска потока OAuth и получения маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="aef16-148">Your app needs to register an instance of the Flask-OAuth client that you'll use to start the OAuth flow and get an access token.</span></span> <span data-ttu-id="aef16-149">Обратите внимание, что для получения сеанса Excel, который поддерживает сохраняемые изменения, необходима область *Files.ReadWrite*.</span><span class="sxs-lookup"><span data-stu-id="aef16-149">Note that the *Files.ReadWrite* scope is required to obtain an Excel session that supports persisted changes.</span></span>

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

### <a name="receive-an-authorization-code-in-your-reply-url-page"></a><span data-ttu-id="aef16-150">Получение кода авторизации на странице URL-адреса ответа</span><span class="sxs-lookup"><span data-stu-id="aef16-150">Receive an authorization code in your reply URL page</span></span>

<span data-ttu-id="aef16-p112">После входа пользователя браузер перенаправляется на URL-адрес отклика. После успешной авторизации в теле отклика возвращается маркер доступа (он будет использоваться для авторизации дополнительных запросов).</span><span class="sxs-lookup"><span data-stu-id="aef16-p112">After the user signs in, the browser is redirected to your reply URL. Upon successful authorization, the access token (which will be used to authorize additional requests) will be returned in the response body.</span></span> 

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

## <a name="make-requests-to-the-excel-api"></a><span data-ttu-id="aef16-153">Отправка запросов к API Excel</span><span class="sxs-lookup"><span data-stu-id="aef16-153">Make requests to the Excel API</span></span>

### <a name="request-headers"></a><span data-ttu-id="aef16-154">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aef16-154">Request headers</span></span> 
<span data-ttu-id="aef16-p113">Используя токен доступа, приложение может отправлять проверенные запросы в API Microsoft Graph. Приложение должно добавлять токен доступа в заголовок **Authorization** каждого запроса.</span><span class="sxs-lookup"><span data-stu-id="aef16-p113">With an access token, your app can make authenticated requests to the Microsoft Graph API. Your app must append the access token to the **Authorization** header of each request.</span></span>

```python
    # Set request headers.
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
        'Accept' : 'application/json',
        'Content-Type' : 'application/json'
    }
```
> <span data-ttu-id="aef16-157">**Примечание**. В запросе необходимо также отправлять заголовок **Content-Type** со значением, принимаемым API Graph, например `application/json`.</span><span class="sxs-lookup"><span data-stu-id="aef16-157">**Note** The request must also send a **Content-Type** header with a value accepted by the Graph API, for example, `application/json`.</span></span>

### <a name="getting-an-excel-session"></a><span data-ttu-id="aef16-158">Получение сеанса Excel</span><span class="sxs-lookup"><span data-stu-id="aef16-158">Getting an Excel Session</span></span>
#### <a name="request"></a><span data-ttu-id="aef16-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="aef16-159">Request</span></span> 

<span data-ttu-id="aef16-160">Передайте объект JSON, задав `persistChanges` значение `true` или `false`.</span><span class="sxs-lookup"><span data-stu-id="aef16-160">Pass a JSON object by setting the `persistChanges` value to `true` or `false`.</span></span> <span data-ttu-id="aef16-161">Если для параметра `persistChanges` установлено значение `false`, возвращается идентификатор непостоянного сеанса.</span><span class="sxs-lookup"><span data-stu-id="aef16-161">When the value of `persistChanges` is set to `false`, a non-persistent session id is returned.</span></span> <span data-ttu-id="aef16-162">В этом примере используется библиотека HTTP [Requests](http://docs.python-requests.org/en/latest/user/quickstart).</span><span class="sxs-lookup"><span data-stu-id="aef16-162">This example uses the [Requests](http://docs.python-requests.org/en/latest/user/quickstart) HTTP library</span></span> 

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

#### <a name="response"></a><span data-ttu-id="aef16-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="aef16-163">Response</span></span>

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

#### <a name="usage"></a><span data-ttu-id="aef16-164">Использование</span><span class="sxs-lookup"><span data-stu-id="aef16-164">Usage</span></span> 

<span data-ttu-id="aef16-165">Идентификатор сеанса, возвращенный при предыдущем вызове, передается в качестве заголовка при последующих запросах API в HTTP-заголовке **Workbook-Session-Id**.</span><span class="sxs-lookup"><span data-stu-id="aef16-165">The session ID returned from the previous call is passed as a header on subsequent API requests in the **Workbook-Session-Id** HTTP header. For instance, to list worksheets in that Excel workbook.</span></span> <span data-ttu-id="aef16-166">Например, для перечисления листов в книге Excel.</span><span class="sxs-lookup"><span data-stu-id="aef16-166">For instance, to list worksheets in that Excel workbook.</span></span>

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

#### <a name="response"></a><span data-ttu-id="aef16-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="aef16-167">Response</span></span>

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

## <a name="next-steps"></a><span data-ttu-id="aef16-168">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="aef16-168">Next steps</span></span>

<span data-ttu-id="aef16-169">С помощью HTTP-заголовка **Workbook-Session-Id** можно отправлять запросы на получение данных, создание диаграмм и многие другие.</span><span class="sxs-lookup"><span data-stu-id="aef16-169">With the **Workbook-Session-Id** HTTP header, you can begin issuing requests to fetch data, create charts, and much more.</span></span> 

* [<span data-ttu-id="aef16-170">Обычные сценарии использования API Excel</span><span class="sxs-lookup"><span data-stu-id="aef16-170">Common Excel API scenarios</span></span>](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel#common-excel-scenarios)
* [<span data-ttu-id="aef16-171">Работа с Excel в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="aef16-171">Working with Excel in Microsoft Graph</span></span>](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel)

<span data-ttu-id="aef16-p116">REST API для Excel в Microsoft Graph — это эффективный способ доступа к данным в книгах Excel и работы с ними. Узнайте о других возможностях Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="aef16-p116">The Excel REST API in Microsoft Graph provides a powerful way to access and interact with data in Excel workbooks. Explore what else is possible with Microsoft Graph.</span></span>

* [<span data-ttu-id="aef16-174">Обзор Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="aef16-174">Overview of Microsoft Graph</span></span>](https://developer.microsoft.com/graph/docs)
* [<span data-ttu-id="aef16-175">Начало работы с Microsoft Graph в приложении на Python</span><span class="sxs-lookup"><span data-stu-id="aef16-175">Get started with Microsoft Graph in a Python app</span></span>](https://developer.microsoft.com/graph/docs/get-started/python)
