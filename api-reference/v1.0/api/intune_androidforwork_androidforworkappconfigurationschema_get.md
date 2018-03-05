# <a name="get-androidforworkappconfigurationschema"></a><span data-ttu-id="fcd08-101">Get androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="fcd08-101">Get androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="fcd08-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fcd08-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcd08-103">Чтение свойств и связей объекта [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="fcd08-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fcd08-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fcd08-104">Prerequisites</span></span>
<span data-ttu-id="fcd08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fcd08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fcd08-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcd08-107">Permission type</span></span>|<span data-ttu-id="fcd08-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcd08-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcd08-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcd08-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fcd08-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd08-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fcd08-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcd08-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcd08-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcd08-112">Not supported.</span></span>|
|<span data-ttu-id="fcd08-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcd08-113">Application</span></span>|<span data-ttu-id="fcd08-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcd08-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcd08-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcd08-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fcd08-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fcd08-116">Optional query parameters</span></span>
<span data-ttu-id="fcd08-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fcd08-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fcd08-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcd08-118">Request headers</span></span>
|<span data-ttu-id="fcd08-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcd08-119">Header</span></span>|<span data-ttu-id="fcd08-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fcd08-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcd08-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcd08-121">Authorization</span></span>|<span data-ttu-id="fcd08-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcd08-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fcd08-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fcd08-123">Accept</span></span>|<span data-ttu-id="fcd08-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fcd08-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcd08-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcd08-125">Request body</span></span>
<span data-ttu-id="fcd08-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fcd08-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcd08-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcd08-127">Response</span></span>
<span data-ttu-id="fcd08-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fcd08-128">If successful, this method returns a `200 OK` response code and [plannerAssignedToTaskBoardTaskFormat](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcd08-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fcd08-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="fcd08-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcd08-130">Request</span></span>
<span data-ttu-id="fcd08-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcd08-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="fcd08-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcd08-132">Response</span></span>
<span data-ttu-id="fcd08-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fcd08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 913

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
    "id": "c1230dc6-0dc6-c123-c60d-23c1c60d23c1",
    "exampleJson": "ZXhhbXBsZUpzb24=",
    "schemaItems": [
      {
        "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
        "schemaItemKey": "Schema Item Key value",
        "displayName": "Display Name value",
        "description": "Description value",
        "defaultBoolValue": true,
        "defaultIntValue": 15,
        "defaultStringValue": "Default String Value value",
        "defaultStringArrayValue": [
          "Default String Array Value value"
        ],
        "dataType": "integer",
        "selections": [
          {
            "@odata.type": "microsoft.graph.keyValuePair",
            "name": "Name value",
            "value": "Value value"
          }
        ]
      }
    ]
  }
}
```



