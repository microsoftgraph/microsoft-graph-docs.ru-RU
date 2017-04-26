
# <a name="microsoft-graph-app-authentication-using-azure-ad"></a>Проверка подлинности в приложении Microsoft Graph с помощью Azure AD

В этой статье подробно рассматривается пример проверки подлинности и потока авторизации для приложения Microsoft Graph. В этом примере используется Azure Active Directory (Azure AD) как поставщик проверки подлинности, а также <a href="https://msdn.microsoft.com/en-us/library/azure/dn645542.aspx" target="_newtab">поток предоставления кода авторизации</a>. В этом примере показано, как использовать Azure AD в приложении Microsoft Graph для проверки подлинности пользователя, получения маркера доступа и обновления маркера доступа с помощью маркера обновления.

Процесс проверки подлинности для потоков предоставления кода состоит из двух основных этапов:

1. Запрос кода авторизации.
2. Запрос маркеров доступа и обновления с помощью кода авторизации. 

С помощью маркера обновления можно получить новый маркер доступа по истечении срока действия текущего маркера доступа.
 
##<a name="authenticate-a-user-and-get-app-authorized"></a>Проверка подлинности пользователя и авторизация приложения

Чтобы авторизовать приложение, необходимо сначала проверить подлинность пользователя. Для этого пользователь перенаправляется в конечную точку авторизации Azure Active Directory (Azure AD) вместе со сведениями о приложении для входа в рабочую или учебную учетную запись. Когда пользователь выполнит вход и предоставит необходимые разрешения (если он еще не сделал этого), приложение получит код авторизации, необходимый для получения маркера доступа OAuth.

> **Примечание**.  Для этого необходимо вызвать методы в [библиотеке Azure AD Authentication Library (ADAL)](https://msdn.microsoft.com/en-us/library/azure/jj573266.aspx). Дополнительные сведения об авторизации см. в статье [Предоставление кода авторизации](https://msdn.microsoft.com/en-us/library/azure/dn645542.aspx).

Прежде чем авторизовать приложение, нужно отправить запрос HTTPS GET, используя следующий URL-адрес:
 
```GET https://login.microsoftonline.com/common/oauth2/authorize?response_type=code&redirect_uri=<uri>&client_id=<id>```

**Обязательные параметры строки запроса**

| Имя параметра  | Значение  | Описание                                                                                            |
|:----------------|:-------|:-------------------------------------------------------------------------------------------------------|
| *client_id*     | строка | Идентификатор клиента, созданный для приложения. Это значение **идентификатора клиента** вашего приложения, указанное в реестре приложений клиента Azure.                                                                  |
| *response_type* | строка | Указывает нужный тип ответа. В запросе на предоставление кода авторизации значение должно быть кодом. |
| *redirect_uri*  | строка | URL-адрес, на который перенаправляется браузер после проверки подлинности.  Это значение должно соответствовать предварительно настроенному значению **URL-адреса ответа**.                        |
 


Ниже приведен пример такого запроса, выполняемого во время работы приложения:


```GET https://login.microsoftonline.com/common/oauth2/authorize?response_type=code&redirect_uri=http%3a%2f%2flocalhost:1339/auth/azureoauth/callback&client_id=8b8539cd-7b75-427f-bef1-4a6264fd4940``` 

Этот запрос возвращает ответ `200 OK` и представляет страницу входа в учетную запись Azure AD. 

Когда пользователь выполняет вход с помощью действительных учетных данных и подтверждает предоставленные разрешения, страница входа отправляет запрос `POST` в Azure. Если этот запрос выполнен успешно, Azure отправит в ответ сообщение `302 Found` для переадресации вызова на URI перенаправления, чтобы приложение смогло получить необходимый маркер доступа. Переадресованный URI, указанный в заголовке `Location` ответа, соответствует URL-адресу ответа приложения с двумя параметрами запроса: `code=...` и `session_state=...`. В следующем примере приведен фрагмент такого ответа: 

```no-highlight 
HTTP/1.1 302 Found
Cache-Control: no-cache, no-store
Pragma: no-cache
Content-Type: text/html; charset=utf-8
Expires: -1
Location: http://localhost:1339/auth/azureoauth/callback?code=AAABAAAAvPM...&session_state=a9556cd3-cae6-4bc9-bf51-672f7b79b7c6
Server: Microsoft-IIS/8.5
P3P: CP="DSP CUR OTPi IND OTRi ONL FIN"

..... 
```

В этом примере URL-адрес ответа приложения — `http://localhost:1339/auth/azureoauth/callback`. При обработке этого ответа необходимо извлечь значение параметра `code` и использовать его, чтобы получить первые токены доступа и обновления OAuth 2.0 (см. следующий раздел).

> **Примечание.** Приведенный выше ответ `302 Found` отличается от ответа `302 Found`, который вы бы получили, если бы начали процесс входа с URL-адреса `https://login.windows.net/{tenantId}/oauth2/authorize?...`. В последнем случае ответ `302 Found` перенаправляет ваш запрос на сайт `login.microsoftonline.com`.
 
<!---<a name="msg_get_app_authenticated"> </a> -->

##<a name="acquire-an-access-token"></a>Получение маркера доступа
Для доступа к ресурсам Microsoft Graph приложение должно добавлять действительный маркер доступа OAuth 2.0 в каждый HTTP-запрос. Вы можете получить маркер доступа с помощью следующего запроса POST:

```no-highlight 
POST https://login.microsoftonline.com/common/oauth2/token HTTP/1.1
content-type : application/x-www-form-urlencoded
content-length : 144
```
 
Для этого запроса требуются полезные данные в кодировке URL в следующем формате:
 
```no-highlight 
grant_type=authorization_code
&redirect_uri=<uri>
&client_id=<id>
&client_secret=<secret_key>
&code=<code>
&resource=https%3A%2F%2Fgraph.microsoft.com%2F
```

**Обязательные параметры строки запроса**

| Имя параметра  | Значение  | Описание                                                                                            |
|:----------------|:-------|:-------------------------------------------------------------------------------------------------------|
| *client_id*     | string | Идентификатор клиента, созданный для приложения.  |
| *client_secret*  | string | Ключ, созданный для приложения. Это значение совпадает со значением в разделе **Ключи** на странице настройки приложения на портале управления Azure.|
| *redirect_uri*  | string | URL-адрес, на который перенаправляется браузер после проверки подлинности.  |
| *code*  | строка | Код авторизации. Значение параметра запроса `code`, возвращенное из ответа на запрос авторизации. |
| *resource*   | string | Ресурс, к которому нужно получить доступ. Чтобы вызвать API Microsoft Graph, задайте для этого параметра значение "https://graph.microsoft.com/".|

Во фрагменте кода ниже приведен пример полезных данных запроса, используемых для получения первого токена доступа OAuth 2.0.

```no-highlight  
grant_type=authorization_code&
redirect_uri=http%3A%2F%2Flocalhost%3A1339%2Fauth%2Fazureoauth%2Fcallback&
client_id=8b8539cd-7b75-427f-bef1-4a6264fd4940&client_secret=PJW3dznGfyNSm3rM9aHeXWGKsTMepKXT1Eqy45XXdU4%3D&
code=AAABAAAAvPM1KaPlrEqdFSBzjqfTGBLRVQc6BtQmJ_9DQZUg8Tb7TJgTmbTE7AHM93qB5EKc4Bf-bOgzt3mebAywK-09X1uBHwOluuqSWfd9LU2HHgZtxcZFIYI5UL7L1UEvhrJRvX2iHhfz9ZSRMZMVL55n_K79gCOxtSATeCUw52zPk5ZaQ87Y42SCLsRZN4Y_zddhD3mMpkObiHVT8HzfhBUiT0oX0e-Q439vkbZoKiq1HaqMR3IPHiCXDbPPH5u7a4NTe5xAhh-o2MUIe6s4Xqql86sv1-IwyroOJJMueGUarkfbgwqmYL9Tm-jWab8o-BAK_plVsN73GU8cXO8ts30wa2YmNR5ZxSkw8oiB4mSZwGzGQlch55DRnucDs0SZBgj5etGi3SeXv5jhKlDU2S0bAPnGxF3QAH0N_zBpfakETVlcsHKi714u-tn9da6aTPQsE0IYKTAYgxjTMei6zfRFvCZi-tKdFR6X9TvvmF2iPdGQGWKeLw8CMWUzU8VmOhiHc0aBKG6RaXAOTM067J_9WKYPxMopcytD2z8HVkL1QhggAA&
resource=https%3A%2F%2Fgraph.microsoft.com%2F
```

После успешной отправки запроса будет возвращен ответ `200 OK`. Пример:

```no-highlight  
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8
Expires: -1
Content-Length: 2978
Access-Control-Allow-Origin: *

{
    "token_type":"Bearer",
    "expires_in":"3599",
    "expires_on":"1426551729",
    "not_before":"1426547829",
    "resource":"https://graph.microsoft.com/",
    "access_token":"eyJ0eXAiOiJKV1QiLCJhb...",
    "refresh_token":"AAABAAAAvPM1KaPlrEqd...",
    "scope": "Calendar.ReadWrite Directory.Read.All Files.ReadWrite Group.ReadWrite.All Mail.ReadWrite Mail.Send User.ReadBasic.All",
    "id_token":"eyJ0eXAiOiJKV1QiLCJhbGci..."
}
```

 
Ответ — это строка в формате JSON, содержащая маркер доступа (`access_token`). Для доступа к ресурсам Microsoft Graph этот маркер необходимо добавлять во все дальнейшие HTTP-запросы. 

Значение свойства `scope` должно соответствовать разрешениям, предоставленным приложению во время регистрации.

Токен доступа действует в течение заданного периода времени (`3599` в приведенном выше примере) в секундах (или 1 час) с момента выдачи, как указано в свойстве `expires_in`. Результат также содержит токен обновления (`refresh_token`), который необходимо использовать для обновления токена доступа с истекающим или истекшим сроком действия. 

В любом рабочем коде приложение должно отслеживать срок действия этих токенов и обновлять их до окончания срока действия токена обновления. 
-->

<!---<a name="msg_renew_access_token using refresh token"> </a> -->

##<a name="renew-expiring-access-token-using-refresh-token"></a>Обновление токена доступа с истекающим сроком действия с помощью токена обновления
Чтобы обновить маркер доступа с истекшим сроком действия, используйте запрос POST, приведенный в примере ниже (если срок действия маркера обновления не истек).

```no-highlight  
POST https://login.microsoftonline.com/common/oauth2/token HTTP/1.1
Host: login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded
Content-Length: 897


grant_type=refresh_token
&redirect_uri=http%3A%2F%2Flocalhost%3A1339%2Fauth%2Fazureoauth%2Fcallback
&client_id=8b8539cd-7b75-427f-bef1-4a6264fd4940
&client_secret=PJW3dznGfyNSm3rM9aHeXWGKsTMepKXT1Eqy45XXdU4%3D
&refresh_token=AAABAAAAvPM1KaPlrEqdFSBzjqfTGM74--...
&resource=https%3A%2F%2Fgraph.microsoft.com%2F
```

**Обязательные параметры строки запроса**

| Имя параметра  | Значение  | Описание                                                                                                                                         |
|:----------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| *client_id*     | string | Идентификатор клиента, созданный для приложения.  |
| *redirect_uri*  | string | URL-адрес, на который перенаправляется браузер после проверки подлинности. Это значение должно соответствовать значению *redirect_uri*, использованному в первом запросе. |
| *client_secret* | string | Одно из значений ключей, созданных для приложения.                                                                                                     |
| *refresh_token* | string | Маркер обновления, полученный ранее.    |
| *resource*      | string | Ресурс, к которому нужно получить доступ.|

Обратите внимание, что этот запрос практически не отличается от запроса на получение первого токена. В полезных данных запроса есть два различия, а именно: параметр `grant_type` теперь имеет значение `refresh_token` (а не `code`).
 
Успешный ответ возвращает полезные данные строки JSON в следующем формате:

```no-highlight 
{
    "token_type":"Bearer",
    "expires_in":"3600",
    "expires_on":"1426561346",
    "not_before":"1426557446",
    "resource":"https://graph.microsoft.com/",
    "access_token":"eyJ0eXAiOiJKV1QiLCJhbGciOi...", 
    "refresh_token":"AAABAAAAvPM1KaPlrEqdFSBzj...",
   "scope":"Graph.Read",
    "pwd_exp":"6553342",
    "pwd_url":"https://portal.microsoftonline.com/ChangePassword.aspx"
}
```
 
По синтаксису и семантике этот ответ не отличается от ответа на запрос на получение первого маркера (отсутствует только свойство `id_token`). Жизненный цикл новых значений `access_token` и `refresh_token` увеличивается. Новый срок действия маркера доступа — это количество секунд, указанное в значении `expires_in`, с момента успешной отправки запроса на обновление маркера. 
 
Когда срок действия токена обновления истечет, вы не сможете обновлять токены доступа с истекшим сроком действия, используя описанный запрос POST. Необходимо будет перезапустить процесс авторизации приложения и проверки подлинности.



