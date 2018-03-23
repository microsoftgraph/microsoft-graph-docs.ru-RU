# <a name="list-managedappprotections"></a><span data-ttu-id="d2f51-101">Перечисление объектов managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="d2f51-101">List managedAppProtections</span></span>

> <span data-ttu-id="d2f51-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d2f51-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2f51-103">Список свойств и связей объектов [managedAppProtection](../resources/intune_mam_managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d2f51-103">List properties and relationships of the [managedAppProtection](../resources/intune_mam_managedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2f51-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d2f51-104">Prerequisites</span></span>
<span data-ttu-id="d2f51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d2f51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d2f51-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2f51-107">Permission type</span></span>|<span data-ttu-id="d2f51-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2f51-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2f51-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2f51-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d2f51-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2f51-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d2f51-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2f51-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2f51-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f51-112">Not supported.</span></span>|
|<span data-ttu-id="d2f51-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2f51-113">Application</span></span>|<span data-ttu-id="d2f51-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f51-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2f51-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2f51-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="d2f51-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2f51-116">Request headers</span></span>
|<span data-ttu-id="d2f51-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2f51-117">Header</span></span>|<span data-ttu-id="d2f51-118">Значение</span><span class="sxs-lookup"><span data-stu-id="d2f51-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2f51-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2f51-119">Authorization</span></span>|<span data-ttu-id="d2f51-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2f51-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d2f51-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d2f51-121">Accept</span></span>|<span data-ttu-id="d2f51-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d2f51-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2f51-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2f51-123">Request body</span></span>
<span data-ttu-id="d2f51-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2f51-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2f51-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2f51-125">Response</span></span>
<span data-ttu-id="d2f51-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppProtection](../resources/intune_mam_managedappprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d2f51-126">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/intune_mam_managedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2f51-127">Пример</span><span class="sxs-lookup"><span data-stu-id="d2f51-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2f51-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2f51-128">Request</span></span>
<span data-ttu-id="d2f51-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2f51-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="d2f51-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2f51-130">Response</span></span>
<span data-ttu-id="d2f51-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d2f51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1715

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "a6c064ce-64ce-a6c0-ce64-c0a6ce64c0a6",
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
      "minimumWarningAppVersion": "Minimum Warning App Version value"
    }
  ]
}
```



