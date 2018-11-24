# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="e7af8-101">Перечисление объектов settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e7af8-101">List settingStateDeviceSummaries</span></span>

> <span data-ttu-id="e7af8-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e7af8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7af8-103">Список свойств и связей объектов [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e7af8-103">List properties and relationships of the [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7af8-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e7af8-104">Prerequisites</span></span>
<span data-ttu-id="e7af8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e7af8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e7af8-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7af8-107">Permission type</span></span>|<span data-ttu-id="e7af8-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7af8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7af8-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7af8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e7af8-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7af8-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e7af8-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7af8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7af8-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7af8-112">Not supported.</span></span>|
|<span data-ttu-id="e7af8-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7af8-113">Application</span></span>|<span data-ttu-id="e7af8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7af8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7af8-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7af8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="e7af8-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7af8-116">Request headers</span></span>
|<span data-ttu-id="e7af8-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7af8-117">Header</span></span>|<span data-ttu-id="e7af8-118">Значение</span><span class="sxs-lookup"><span data-stu-id="e7af8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7af8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7af8-119">Authorization</span></span>|<span data-ttu-id="e7af8-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7af8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7af8-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e7af8-121">Accept</span></span>|<span data-ttu-id="e7af8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e7af8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7af8-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7af8-123">Request body</span></span>
<span data-ttu-id="e7af8-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e7af8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7af8-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7af8-125">Response</span></span>
<span data-ttu-id="e7af8-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e7af8-126">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7af8-127">Пример</span><span class="sxs-lookup"><span data-stu-id="e7af8-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7af8-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7af8-128">Request</span></span>
<span data-ttu-id="e7af8-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7af8-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="e7af8-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7af8-130">Response</span></span>
<span data-ttu-id="e7af8-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e7af8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 486

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
      "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
      "settingName": "Setting Name value",
      "instancePath": "Instance Path value",
      "unknownDeviceCount": 2,
      "notApplicableDeviceCount": 8,
      "compliantDeviceCount": 4,
      "remediatedDeviceCount": 5,
      "nonCompliantDeviceCount": 7,
      "errorDeviceCount": 0,
      "conflictDeviceCount": 3
    }
  ]
}
```



