# <a name="list-devicecomplianceuserstatuses"></a><span data-ttu-id="3924b-101">List deviceComplianceUserStatuses</span><span class="sxs-lookup"><span data-stu-id="3924b-101">List deviceComplianceUserStatuses</span></span>

> <span data-ttu-id="3924b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3924b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3924b-103">Перечисление свойств и связей объектов [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="3924b-103">List properties and relationships of the [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3924b-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3924b-104">Prerequisites</span></span>
<span data-ttu-id="3924b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3924b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3924b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3924b-107">Permission type</span></span>|<span data-ttu-id="3924b-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3924b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3924b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3924b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3924b-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3924b-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3924b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3924b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3924b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3924b-112">Not supported.</span></span>|
|<span data-ttu-id="3924b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3924b-113">Application</span></span>|<span data-ttu-id="3924b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3924b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3924b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3924b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="3924b-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3924b-116">Request headers</span></span>
|<span data-ttu-id="3924b-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3924b-117">Header</span></span>|<span data-ttu-id="3924b-118">Значение</span><span class="sxs-lookup"><span data-stu-id="3924b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3924b-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3924b-119">Authorization</span></span>|<span data-ttu-id="3924b-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="3924b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3924b-121">Принять</span><span class="sxs-lookup"><span data-stu-id="3924b-121">Accept</span></span>|<span data-ttu-id="3924b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3924b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3924b-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3924b-123">Request body</span></span>
<span data-ttu-id="3924b-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3924b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3924b-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="3924b-125">Response</span></span>
<span data-ttu-id="3924b-126">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3924b-126">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3924b-127">Пример</span><span class="sxs-lookup"><span data-stu-id="3924b-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="3924b-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="3924b-128">Request</span></span>
<span data-ttu-id="3924b-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3924b-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="3924b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3924b-130">Response</span></span>
<span data-ttu-id="3924b-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3924b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








