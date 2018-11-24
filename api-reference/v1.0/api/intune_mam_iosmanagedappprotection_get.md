# <a name="get-iosmanagedappprotection"></a><span data-ttu-id="4dfab-101">Получение объекта iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="4dfab-101">Get iosManagedAppProtection</span></span>

> <span data-ttu-id="4dfab-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4dfab-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4dfab-103">Чтение свойств и связей объекта [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4dfab-103">Read properties and relationships of the [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4dfab-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4dfab-104">Prerequisites</span></span>
<span data-ttu-id="4dfab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4dfab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4dfab-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4dfab-107">Permission type</span></span>|<span data-ttu-id="4dfab-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4dfab-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dfab-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4dfab-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4dfab-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4dfab-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4dfab-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4dfab-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dfab-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dfab-112">Not supported.</span></span>|
|<span data-ttu-id="4dfab-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4dfab-113">Application</span></span>|<span data-ttu-id="4dfab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dfab-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dfab-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4dfab-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4dfab-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4dfab-116">Optional query parameters</span></span>
<span data-ttu-id="4dfab-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4dfab-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4dfab-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4dfab-118">Request headers</span></span>
|<span data-ttu-id="4dfab-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4dfab-119">Header</span></span>|<span data-ttu-id="4dfab-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4dfab-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dfab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dfab-121">Authorization</span></span>|<span data-ttu-id="4dfab-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4dfab-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dfab-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4dfab-123">Accept</span></span>|<span data-ttu-id="4dfab-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4dfab-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dfab-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4dfab-125">Request body</span></span>
<span data-ttu-id="4dfab-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4dfab-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4dfab-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dfab-127">Response</span></span>
<span data-ttu-id="4dfab-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4dfab-128">If successful, this method returns a `200 OK` response code and [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dfab-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4dfab-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4dfab-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dfab-130">Request</span></span>
<span data-ttu-id="4dfab-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dfab-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="4dfab-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="4dfab-132">Response</span></span>
<span data-ttu-id="4dfab-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4dfab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1839

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "5bc789cb-89cb-5bc7-cb89-c75bcb89c75b",
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
    "appDataEncryptionType": "afterDeviceRestart",
    "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
    "deployedAppCount": 0,
    "faceIdBlocked": true
  }
}
```



