# <a name="sovereign-cloud-deployments"></a>Независимые облачные развертывания


В этой статье приведены сведения о различных независимых облачных экземплярах Microsoft Graph и возможностях, доступных разработчикам. 


## <a name="microsoft-graph-operated-by-21vianet-in-china"></a>Служба Microsoft Graph, предоставляемая 21Vianet в Китае

В этом разделе приведены сведения о службе Microsoft Graph под управлением 21Vianet и возможностях, доступных разработчикам. 

### <a name="microsoft-graph-service-root-endpoints"></a>Конечные точки корневого каталога для обслуживания Microsoft Graph
| Microsoft Graph под управлением 21Vianet | Microsoft Graph|
|---------------------------|----------------|
| https://microsoftgraph.chinacloudapi.cn | https://graph.microsoft.com|

### <a name="microsoft-graph-explorer"></a>Песочница Microsoft Graph
| Песочница Microsoft Graph в Китае | Песочница Microsoft Graph|
|---------------------------|----------------|
|https://graph.microsoft.io/zh-cn/graph-explorer| https://graph.microsoft.io/en-us/graph-explorer|

### <a name="azure-openid-connect-and-oauth20"></a>Azure OpenID Connect и OAuth2.0
Конечные точки, которые используются для получения маркеров для входа или для вызова службы Microsoft Graph, предоставляемой 21Vianet, отличаются от конечных точек других предложений. 

| Служба Microsoft Graph, предоставляемая 21Vianet | Microsoft Graph|
|---------------------------|----------------|
| https://login.chinacloudapi.cn | https://login.microsoftonline.com|
 
Используйте https://login.chinacloudapi.cn/common/oauth2/authorize, чтобы проверить подлинность пользователя, и https://login.chinacloudapi.cn/common/oauth2/token, чтобы получить маркер для вызова службы Microsoft Graph, которую предоставляет оператор 21Vianet.

> **Примечание.** Самые новые [конечные точки маркера и авторизации 2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-appmodel-v2-overview/) НЕ ДОСТУПНЫ для использования со службой Microsoft Graph, которую предоставляет 21Vianet. 

>С помощью конечной точки **https://microsoftgraph.chinacloudapi.cn** приложения могут получать доступ только к данным организации (не данным пользователей). Приложения должны использовать конечную точку **https://graph.microsoft.com** для доступа к пользовательским данным.

### <a name="service-capabilities-offered-by-microsoft-graph-operated-by-21vianet"></a>Возможности службы Microsoft Graph, предоставляемой 21Vianet
Следующие функции Microsoft Graph общедоступны (в конечной точке `/v1.0`):

* Пользователи
* Группы
* Файлы
* Почта
* Календарь
* Личные контакты 
* Операции CRUD (создание, чтение, обновление, удаление)
* Поддержка общего доступа к ресурсам независимо от источника (CORS)

Следующие функции Microsoft Graph также доступны в предварительной версии (в конечной точке `/beta`):

* Контакты организации
* Приложения
* Субъекты-службы
* Расширения схемы каталога
* Веб-перехватчики
