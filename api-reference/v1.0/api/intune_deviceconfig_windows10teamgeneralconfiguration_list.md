# <a name="list-windows10teamgeneralconfigurations"></a><span data-ttu-id="85830-101">Перечисление объектов windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="85830-101">List windows10TeamGeneralConfigurations</span></span>

> <span data-ttu-id="85830-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="85830-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85830-103">Перечисление свойств и связей объектов [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85830-103">List properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85830-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="85830-104">Prerequisites</span></span>
<span data-ttu-id="85830-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="85830-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="85830-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85830-107">Permission type</span></span>|<span data-ttu-id="85830-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85830-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85830-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85830-109">Delegated (work or school account)</span></span>|<span data-ttu-id="85830-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="85830-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="85830-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85830-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85830-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85830-112">Not supported.</span></span>|
|<span data-ttu-id="85830-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85830-113">Application</span></span>|<span data-ttu-id="85830-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85830-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85830-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85830-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="85830-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85830-116">Request headers</span></span>
|<span data-ttu-id="85830-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85830-117">Header</span></span>|<span data-ttu-id="85830-118">Значение</span><span class="sxs-lookup"><span data-stu-id="85830-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85830-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="85830-119">Authorization</span></span>|<span data-ttu-id="85830-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85830-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="85830-121">Accept</span><span class="sxs-lookup"><span data-stu-id="85830-121">Accept</span></span>|<span data-ttu-id="85830-122">application/json</span><span class="sxs-lookup"><span data-stu-id="85830-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85830-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85830-123">Request body</span></span>
<span data-ttu-id="85830-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85830-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85830-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="85830-125">Response</span></span>
<span data-ttu-id="85830-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="85830-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85830-127">Пример</span><span class="sxs-lookup"><span data-stu-id="85830-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="85830-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="85830-128">Request</span></span>
<span data-ttu-id="85830-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85830-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="85830-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="85830-130">Response</span></span>
<span data-ttu-id="85830-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="85830-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1463

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
      "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "azureOperationalInsightsBlockTelemetry": true,
      "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
      "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
      "connectAppBlockAutoLaunch": true,
      "maintenanceWindowBlocked": true,
      "maintenanceWindowDurationInHours": 0,
      "maintenanceWindowStartTime": "11:59:09.3130000",
      "miracastChannel": "one",
      "miracastBlocked": true,
      "miracastRequirePin": true,
      "settingsBlockMyMeetingsAndFiles": true,
      "settingsBlockSessionResume": true,
      "settingsBlockSigninSuggestions": true,
      "settingsDefaultVolume": 5,
      "settingsScreenTimeoutInMinutes": 14,
      "settingsSessionTimeoutInMinutes": 15,
      "settingsSleepTimeoutInMinutes": 13,
      "welcomeScreenBlockAutomaticWakeUp": true,
      "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
      "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
    }
  ]
}
```



