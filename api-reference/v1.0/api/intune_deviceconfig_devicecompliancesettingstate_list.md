# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="d5940-101">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="d5940-101">List deviceComplianceSettingStates</span></span>

> <span data-ttu-id="d5940-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d5940-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5940-103">Перечисление свойств и связей объектов [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="d5940-103">List properties and relationships of the [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5940-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d5940-104">Prerequisites</span></span>
<span data-ttu-id="d5940-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d5940-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d5940-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5940-107">Permission type</span></span>|<span data-ttu-id="d5940-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5940-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5940-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5940-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d5940-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5940-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d5940-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5940-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5940-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5940-112">Not supported.</span></span>|
|<span data-ttu-id="d5940-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5940-113">Application</span></span>|<span data-ttu-id="d5940-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5940-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5940-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5940-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="d5940-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d5940-116">Request headers</span></span>
|<span data-ttu-id="d5940-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5940-117">Header</span></span>|<span data-ttu-id="d5940-118">Значение</span><span class="sxs-lookup"><span data-stu-id="d5940-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5940-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5940-119">Authorization</span></span>|<span data-ttu-id="d5940-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5940-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5940-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d5940-121">Accept</span></span>|<span data-ttu-id="d5940-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d5940-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5940-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5940-123">Request body</span></span>
<span data-ttu-id="d5940-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d5940-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5940-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="d5940-125">Response</span></span>
<span data-ttu-id="d5940-126">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d5940-126">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5940-127">Пример</span><span class="sxs-lookup"><span data-stu-id="d5940-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="d5940-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5940-128">Request</span></span>
<span data-ttu-id="d5940-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5940-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="d5940-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d5940-130">Response</span></span>
<span data-ttu-id="d5940-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d5940-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
      "id": "9905f955-f955-9905-55f9-059955f90599",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "userId": "User Id value",
      "userEmail": "User Email value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "deviceModel": "Device Model value",
      "state": "notApplicable",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
    }
  ]
}
```



