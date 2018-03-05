# <a name="get-devicecompliancepolicystate"></a><span data-ttu-id="e469c-101">Get deviceCompliancePolicyState</span><span class="sxs-lookup"><span data-stu-id="e469c-101">Get deviceCompliancePolicyState</span></span>

> <span data-ttu-id="e469c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e469c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e469c-103">Чтение свойств и связей объекта [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).</span><span class="sxs-lookup"><span data-stu-id="e469c-103">Read properties and relationships of [plannerProgressTaskBoardTaskFormat](../resources/intune_deviceconfig_devicecompliancepolicystate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e469c-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e469c-104">Prerequisites</span></span>
<span data-ttu-id="e469c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e469c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e469c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e469c-107">Permission type</span></span>|<span data-ttu-id="e469c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e469c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e469c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e469c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e469c-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e469c-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e469c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e469c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e469c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e469c-112">Not supported.</span></span>|
|<span data-ttu-id="e469c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e469c-113">Application</span></span>|<span data-ttu-id="e469c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e469c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e469c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e469c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /managedDevices/{managedDevicesId}/deviceCompliancePolicyStates/{deviceCompliancePolicyStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e469c-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e469c-116">Optional query parameters</span></span>
<span data-ttu-id="e469c-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e469c-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e469c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e469c-118">Request headers</span></span>
|<span data-ttu-id="e469c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e469c-119">Header</span></span>|<span data-ttu-id="e469c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e469c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e469c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e469c-121">Authorization</span></span>|<span data-ttu-id="e469c-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e469c-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e469c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e469c-123">Accept</span></span>|<span data-ttu-id="e469c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e469c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e469c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e469c-125">Request body</span></span>
<span data-ttu-id="e469c-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e469c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e469c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="e469c-127">Response</span></span>
<span data-ttu-id="e469c-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e469c-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_deviceconfig_devicecompliancepolicystate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e469c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="e469c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="e469c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e469c-130">Request</span></span>
<span data-ttu-id="e469c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e469c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/managedDevices/{managedDevicesId}/deviceCompliancePolicyStates/{deviceCompliancePolicyStateId}
```

### <a name="response"></a><span data-ttu-id="e469c-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="e469c-132">Response</span></span>
<span data-ttu-id="e469c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e469c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1101

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
    "id": "2999e387-e387-2999-87e3-992987e39929",
    "settingStates": [
      {
        "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
        "setting": "Setting value",
        "settingName": "Setting Name value",
        "instanceDisplayName": "Instance Display Name value",
        "state": "notApplicable",
        "errorCode": 9,
        "errorDescription": "Error Description value",
        "userId": "User Id value",
        "userName": "User Name value",
        "userEmail": "User Email value",
        "userPrincipalName": "User Principal Name value",
        "sources": [
          {
            "@odata.type": "microsoft.graph.settingSource",
            "id": "Id value",
            "displayName": "Display Name value"
          }
        ],
        "currentValue": "Current Value value"
      }
    ],
    "displayName": "Display Name value",
    "version": 7,
    "platformType": "iOS",
    "state": "notApplicable",
    "settingCount": 12
  }
}
```



