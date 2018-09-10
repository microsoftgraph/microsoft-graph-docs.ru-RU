# <a name="get-windows10teamgeneralconfiguration"></a><span data-ttu-id="0f4bd-101">Get windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f4bd-101">Get windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="0f4bd-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0f4bd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f4bd-103">Чтение свойств и связей объекта [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f4bd-103">Read properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0f4bd-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0f4bd-104">Prerequisites</span></span>
<span data-ttu-id="0f4bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0f4bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0f4bd-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f4bd-107">Permission type</span></span>|<span data-ttu-id="0f4bd-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f4bd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f4bd-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f4bd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0f4bd-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f4bd-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0f4bd-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f4bd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f4bd-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f4bd-112">Not supported.</span></span>|
|<span data-ttu-id="0f4bd-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f4bd-113">Application</span></span>|<span data-ttu-id="0f4bd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f4bd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f4bd-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f4bd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0f4bd-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0f4bd-116">Optional query parameters</span></span>
<span data-ttu-id="0f4bd-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0f4bd-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0f4bd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f4bd-118">Request headers</span></span>
|<span data-ttu-id="0f4bd-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f4bd-119">Header</span></span>|<span data-ttu-id="0f4bd-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0f4bd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f4bd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f4bd-121">Authorization</span></span>|<span data-ttu-id="0f4bd-122">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="0f4bd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f4bd-123">Принять</span><span class="sxs-lookup"><span data-stu-id="0f4bd-123">Accept</span></span>|<span data-ttu-id="0f4bd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0f4bd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f4bd-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f4bd-125">Request body</span></span>
<span data-ttu-id="0f4bd-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f4bd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f4bd-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="0f4bd-127">Response</span></span>
<span data-ttu-id="0f4bd-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0f4bd-128">If successful, this method returns a `200 OK` response code and [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f4bd-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0f4bd-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f4bd-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f4bd-130">Request</span></span>
<span data-ttu-id="0f4bd-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f4bd-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="0f4bd-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="0f4bd-132">Response</span></span>
<span data-ttu-id="0f4bd-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f4bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1395

{
  "value": {
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
}
```








