# <a name="get-auditevent"></a><span data-ttu-id="ab846-101">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="ab846-101">Get auditEvent</span></span>

> <span data-ttu-id="ab846-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ab846-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab846-103">Чтение свойств и связей объекта [auditEvent](../resources/intune_auditing_auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="ab846-103">Read properties and relationships of the [auditEvent](../resources/intune_auditing_auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab846-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ab846-104">Prerequisites</span></span>
<span data-ttu-id="ab846-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ab846-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ab846-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab846-107">Permission type</span></span>|<span data-ttu-id="ab846-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab846-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab846-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab846-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ab846-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab846-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ab846-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab846-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab846-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab846-112">Not supported.</span></span>|
|<span data-ttu-id="ab846-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab846-113">Application</span></span>|<span data-ttu-id="ab846-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab846-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab846-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab846-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab846-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ab846-116">Optional query parameters</span></span>
<span data-ttu-id="ab846-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ab846-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ab846-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab846-118">Request headers</span></span>
|<span data-ttu-id="ab846-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab846-119">Header</span></span>|<span data-ttu-id="ab846-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ab846-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab846-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab846-121">Authorization</span></span>|<span data-ttu-id="ab846-122">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="ab846-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab846-123">Принять</span><span class="sxs-lookup"><span data-stu-id="ab846-123">Accept</span></span>|<span data-ttu-id="ab846-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ab846-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab846-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab846-125">Request body</span></span>
<span data-ttu-id="ab846-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab846-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab846-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab846-127">Response</span></span>
<span data-ttu-id="ab846-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [auditEvent](../resources/intune_auditing_auditevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ab846-128">If successful, this method returns a `200 OK` response code and [auditEvent](../resources/intune_auditing_auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab846-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ab846-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab846-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab846-130">Request</span></span>
<span data-ttu-id="ab846-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab846-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="ab846-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab846-132">Response</span></span>
<span data-ttu-id="ab846-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab846-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1535

{
  "value": {
    "@odata.type": "#microsoft.graph.auditEvent",
    "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
    "displayName": "Display Name value",
    "componentName": "Component Name value",
    "actor": {
      "@odata.type": "microsoft.graph.auditActor",
      "type": "Type value",
      "userPermissions": [
        "User Permissions value"
      ],
      "applicationId": "Application Id value",
      "applicationDisplayName": "Application Display Name value",
      "userPrincipalName": "User Principal Name value",
      "servicePrincipalName": "Service Principal Name value",
      "ipAddress": "Ip Address value",
      "userId": "User Id value"
    },
    "activity": "Activity value",
    "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
    "activityType": "Activity Type value",
    "activityOperationType": "Activity Operation Type value",
    "activityResult": "Activity Result value",
    "correlationId": "<Unknown Primitive Type Edm.Guid>",
    "resources": [
      {
        "@odata.type": "microsoft.graph.auditResource",
        "displayName": "Display Name value",
        "modifiedProperties": [
          {
            "@odata.type": "microsoft.graph.auditProperty",
            "displayName": "Display Name value",
            "oldValue": "Old Value value",
            "newValue": "New Value value"
          }
        ],
        "type": "Type value",
        "resourceId": "Resource Id value"
      }
    ],
    "category": "Category value"
  }
}
```








