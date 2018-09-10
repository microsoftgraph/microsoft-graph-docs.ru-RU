# <a name="list-androidmanagedappprotections"></a><span data-ttu-id="c6a17-101">Перечисление объектов androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="c6a17-101">List androidManagedAppProtections</span></span>

> <span data-ttu-id="c6a17-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c6a17-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6a17-103">Перечисление свойств и связей объектов [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="c6a17-103">List properties and relationships of the [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c6a17-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c6a17-104">Prerequisites</span></span>
<span data-ttu-id="c6a17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c6a17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c6a17-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6a17-107">Permission type</span></span>|<span data-ttu-id="c6a17-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6a17-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6a17-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6a17-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c6a17-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6a17-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c6a17-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6a17-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6a17-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6a17-112">Not supported.</span></span>|
|<span data-ttu-id="c6a17-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6a17-113">Application</span></span>|<span data-ttu-id="c6a17-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6a17-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6a17-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6a17-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="c6a17-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6a17-116">Request headers</span></span>
|<span data-ttu-id="c6a17-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c6a17-117">Header</span></span>|<span data-ttu-id="c6a17-118">Значение</span><span class="sxs-lookup"><span data-stu-id="c6a17-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6a17-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6a17-119">Authorization</span></span>|<span data-ttu-id="c6a17-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="c6a17-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6a17-121">Принять</span><span class="sxs-lookup"><span data-stu-id="c6a17-121">Accept</span></span>|<span data-ttu-id="c6a17-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c6a17-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6a17-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6a17-123">Request body</span></span>
<span data-ttu-id="c6a17-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6a17-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6a17-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6a17-125">Response</span></span>
<span data-ttu-id="c6a17-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c6a17-126">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6a17-127">Пример</span><span class="sxs-lookup"><span data-stu-id="c6a17-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6a17-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6a17-128">Request</span></span>
<span data-ttu-id="c6a17-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6a17-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="c6a17-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6a17-130">Response</span></span>
<span data-ttu-id="c6a17-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6a17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2065

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "cf517ced-7ced-cf51-ed7c-51cfed7c51cf",
      "version": "Version value",
      "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
      "periodOnlineBeforeAccessCheck": "PT35.0018757S",
      "allowedInboundDataTransferSources": "managedApps",
      "allowedOutboundDataTransferDestinations": "managedApps",
      "organizationalCredentialsRequired": true,
      "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
      "dataBackupBlocked": true,
      "deviceComplianceRequired": true,
      "managedBrowserToOpenLinksRequired": true,
      "saveAsBlocked": true,
      "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
      "pinRequired": true,
      "maximumPinRetries": 1,
      "simplePinBlocked": true,
      "minimumPinLength": 0,
      "pinCharacterSet": "alphanumericAndSymbol",
      "periodBeforePinReset": "PT3M29.6631862S",
      "allowedDataStorageLocations": [
        "sharePoint"
      ],
      "contactSyncBlocked": true,
      "printBlocked": true,
      "fingerprintBlocked": true,
      "disableAppPinIfDevicePinIsSet": true,
      "minimumRequiredOsVersion": "Minimum Required Os Version value",
      "minimumWarningOsVersion": "Minimum Warning Os Version value",
      "minimumRequiredAppVersion": "Minimum Required App Version value",
      "minimumWarningAppVersion": "Minimum Warning App Version value",
      "isAssigned": true,
      "screenCaptureBlocked": true,
      "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
      "encryptAppData": true,
      "deployedAppCount": 0,
      "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
      "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
    }
  ]
}
```








