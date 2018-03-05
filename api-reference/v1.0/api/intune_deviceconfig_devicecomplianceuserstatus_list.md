# <a name="list-devicecomplianceuserstatuses"></a><span data-ttu-id="03961-101">List deviceComplianceUserStatuses</span><span class="sxs-lookup"><span data-stu-id="03961-101">List deviceComplianceUserStatuses</span></span>

> <span data-ttu-id="03961-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="03961-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03961-103">Перечисление свойств и связей объектов [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="03961-103">List properties and relationships of the [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="03961-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="03961-104">Prerequisites</span></span>
<span data-ttu-id="03961-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="03961-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="03961-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03961-107">Permission type</span></span>|<span data-ttu-id="03961-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03961-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03961-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03961-109">Delegated (work or school account)</span></span>|<span data-ttu-id="03961-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="03961-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="03961-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03961-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03961-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03961-112">Not supported.</span></span>|
|<span data-ttu-id="03961-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03961-113">Application</span></span>|<span data-ttu-id="03961-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03961-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03961-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03961-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="03961-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="03961-116">Request headers</span></span>
|<span data-ttu-id="03961-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03961-117">Header</span></span>|<span data-ttu-id="03961-118">Значение</span><span class="sxs-lookup"><span data-stu-id="03961-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03961-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="03961-119">Authorization</span></span>|<span data-ttu-id="03961-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03961-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="03961-121">Accept</span><span class="sxs-lookup"><span data-stu-id="03961-121">Accept</span></span>|<span data-ttu-id="03961-122">application/json</span><span class="sxs-lookup"><span data-stu-id="03961-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03961-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03961-123">Request body</span></span>
<span data-ttu-id="03961-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03961-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03961-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="03961-125">Response</span></span>
<span data-ttu-id="03961-126">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="03961-126">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03961-127">Пример</span><span class="sxs-lookup"><span data-stu-id="03961-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="03961-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="03961-128">Request</span></span>
<span data-ttu-id="03961-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03961-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="03961-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="03961-130">Response</span></span>
<span data-ttu-id="03961-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="03961-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 397

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
      "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



