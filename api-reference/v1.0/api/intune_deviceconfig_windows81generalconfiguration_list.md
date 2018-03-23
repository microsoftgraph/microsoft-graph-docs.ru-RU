# <a name="list-windows81generalconfigurations"></a><span data-ttu-id="4d314-101">Перечисление объектов windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="4d314-101">List windows81GeneralConfigurations</span></span>

> <span data-ttu-id="4d314-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4d314-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d314-103">Перечисление свойств и связей объектов [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4d314-103">List properties and relationships of the [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d314-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4d314-104">Prerequisites</span></span>
<span data-ttu-id="4d314-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4d314-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4d314-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d314-107">Permission type</span></span>|<span data-ttu-id="4d314-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d314-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d314-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d314-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4d314-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d314-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4d314-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d314-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d314-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d314-112">Not supported.</span></span>|
|<span data-ttu-id="4d314-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d314-113">Application</span></span>|<span data-ttu-id="4d314-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d314-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d314-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d314-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4d314-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d314-116">Request headers</span></span>
|<span data-ttu-id="4d314-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d314-117">Header</span></span>|<span data-ttu-id="4d314-118">Значение</span><span class="sxs-lookup"><span data-stu-id="4d314-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d314-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d314-119">Authorization</span></span>|<span data-ttu-id="4d314-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d314-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4d314-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4d314-121">Accept</span></span>|<span data-ttu-id="4d314-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4d314-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d314-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d314-123">Request body</span></span>
<span data-ttu-id="4d314-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d314-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d314-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d314-125">Response</span></span>
<span data-ttu-id="4d314-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4d314-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_deviceconfig_windows81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d314-127">Пример</span><span class="sxs-lookup"><span data-stu-id="4d314-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d314-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d314-128">Request</span></span>
<span data-ttu-id="4d314-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d314-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="4d314-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d314-130">Response</span></span>
<span data-ttu-id="4d314-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4d314-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2058

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
      "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "accountsBlockAddingNonMicrosoftAccountEmail": true,
      "applyOnlyToWindows81": true,
      "browserBlockAutofill": true,
      "browserBlockAutomaticDetectionOfIntranetSites": true,
      "browserBlockEnterpriseModeAccess": true,
      "browserBlockJavaScript": true,
      "browserBlockPlugins": true,
      "browserBlockPopups": true,
      "browserBlockSendingDoNotTrackHeader": true,
      "browserBlockSingleWordEntryOnIntranetSites": true,
      "browserRequireSmartScreen": true,
      "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
      "browserInternetSecurityLevel": "medium",
      "browserIntranetSecurityLevel": "low",
      "browserLoggingReportLocation": "Browser Logging Report Location value",
      "browserRequireHighSecurityForRestrictedSites": true,
      "browserRequireFirewall": true,
      "browserRequireFraudWarning": true,
      "browserTrustedSitesSecurityLevel": "low",
      "cellularBlockDataRoaming": true,
      "diagnosticsBlockDataSubmission": true,
      "passwordBlockPicturePasswordAndPin": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordMinimumCharacterSetCount": 0,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequiredType": "alphanumeric",
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "storageRequireDeviceEncryption": true,
      "updatesRequireAutomaticUpdates": true,
      "userAccountControlSettings": "alwaysNotify",
      "workFoldersUrl": "https://example.com/workFoldersUrl/"
    }
  ]
}
```



