# <a name="get-devicecomplianceuseroverview"></a><span data-ttu-id="4f261-101">Get deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="4f261-101">Get deviceComplianceUserOverview</span></span>

> <span data-ttu-id="4f261-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4f261-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f261-103">Чтение свойств и связей объекта [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="4f261-103">Read properties and relationships of [plannerProgressTaskBoardTaskFormat](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f261-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4f261-104">Prerequisites</span></span>
<span data-ttu-id="4f261-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4f261-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4f261-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f261-107">Permission type</span></span>|<span data-ttu-id="4f261-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f261-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f261-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f261-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4f261-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f261-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4f261-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f261-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f261-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f261-112">Not supported.</span></span>|
|<span data-ttu-id="4f261-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f261-113">Application</span></span>|<span data-ttu-id="4f261-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f261-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f261-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f261-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f261-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4f261-116">Optional query parameters</span></span>
<span data-ttu-id="4f261-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4f261-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4f261-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f261-118">Request headers</span></span>
|<span data-ttu-id="4f261-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f261-119">Header</span></span>|<span data-ttu-id="4f261-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4f261-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f261-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f261-121">Authorization</span></span>|<span data-ttu-id="4f261-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f261-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4f261-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4f261-123">Accept</span></span>|<span data-ttu-id="4f261-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4f261-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f261-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f261-125">Request body</span></span>
<span data-ttu-id="4f261-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f261-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f261-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f261-127">Response</span></span>
<span data-ttu-id="4f261-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4f261-128">If successful, this method returns a `200 OK` response code and a [section](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f261-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4f261-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f261-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f261-130">Request</span></span>
<span data-ttu-id="4f261-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f261-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="4f261-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f261-132">Response</span></span>
<span data-ttu-id="4f261-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4f261-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 365

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
    "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```



