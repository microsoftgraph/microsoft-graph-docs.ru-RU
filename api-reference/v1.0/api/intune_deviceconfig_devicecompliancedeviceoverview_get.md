# <a name="get-devicecompliancedeviceoverview"></a><span data-ttu-id="43900-101">Get deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="43900-101">Get deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="43900-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="43900-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43900-103">Чтение свойств и связей объекта [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="43900-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43900-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="43900-104">Prerequisites</span></span>
<span data-ttu-id="43900-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="43900-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="43900-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43900-107">Permission type</span></span>|<span data-ttu-id="43900-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43900-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43900-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43900-109">Delegated (work or school account)</span></span>|<span data-ttu-id="43900-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="43900-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="43900-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43900-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43900-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43900-112">Not supported.</span></span>|
|<span data-ttu-id="43900-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43900-113">Application</span></span>|<span data-ttu-id="43900-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43900-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43900-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43900-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43900-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="43900-116">Optional query parameters</span></span>
<span data-ttu-id="43900-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="43900-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="43900-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43900-118">Request headers</span></span>
|<span data-ttu-id="43900-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43900-119">Header</span></span>|<span data-ttu-id="43900-120">Значение</span><span class="sxs-lookup"><span data-stu-id="43900-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43900-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="43900-121">Authorization</span></span>|<span data-ttu-id="43900-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43900-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="43900-123">Accept</span><span class="sxs-lookup"><span data-stu-id="43900-123">Accept</span></span>|<span data-ttu-id="43900-124">application/json</span><span class="sxs-lookup"><span data-stu-id="43900-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43900-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43900-125">Request body</span></span>
<span data-ttu-id="43900-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43900-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43900-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="43900-127">Response</span></span>
<span data-ttu-id="43900-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="43900-128">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43900-129">Пример</span><span class="sxs-lookup"><span data-stu-id="43900-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="43900-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="43900-130">Request</span></span>
<span data-ttu-id="43900-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43900-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="43900-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="43900-132">Response</span></span>
<span data-ttu-id="43900-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="43900-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 367

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
    "id": "886f167b-167b-886f-7b16-6f887b166f88",
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



