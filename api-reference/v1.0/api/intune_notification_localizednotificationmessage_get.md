# <a name="get-localizednotificationmessage"></a><span data-ttu-id="653b5-101">Получение объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="653b5-101">Get localizedNotificationMessage</span></span>

> <span data-ttu-id="653b5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="653b5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="653b5-103">Чтение свойств и связей объекта [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="653b5-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_notification_localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="653b5-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="653b5-104">Prerequisites</span></span>
<span data-ttu-id="653b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="653b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="653b5-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="653b5-107">Permission type</span></span>|<span data-ttu-id="653b5-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="653b5-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="653b5-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="653b5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="653b5-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="653b5-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="653b5-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="653b5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="653b5-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="653b5-112">Not supported.</span></span>|
|<span data-ttu-id="653b5-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="653b5-113">Application</span></span>|<span data-ttu-id="653b5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="653b5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="653b5-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="653b5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="653b5-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="653b5-116">Optional query parameters</span></span>
<span data-ttu-id="653b5-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="653b5-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="653b5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="653b5-118">Request headers</span></span>
|<span data-ttu-id="653b5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="653b5-119">Header</span></span>|<span data-ttu-id="653b5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="653b5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="653b5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="653b5-121">Authorization</span></span>|<span data-ttu-id="653b5-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="653b5-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="653b5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="653b5-123">Accept</span></span>|<span data-ttu-id="653b5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="653b5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="653b5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="653b5-125">Request body</span></span>
<span data-ttu-id="653b5-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="653b5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="653b5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="653b5-127">Response</span></span>
<span data-ttu-id="653b5-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="653b5-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_notification_localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="653b5-129">Пример</span><span class="sxs-lookup"><span data-stu-id="653b5-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="653b5-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="653b5-130">Request</span></span>
<span data-ttu-id="653b5-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="653b5-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="653b5-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="653b5-132">Response</span></span>
<span data-ttu-id="653b5-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="653b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.localizedNotificationMessage",
    "id": "7a777708-7708-7a77-0877-777a0877777a",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "locale": "Locale value",
    "subject": "Subject value",
    "messageTemplate": "Message Template value",
    "isDefault": true
  }
}
```



