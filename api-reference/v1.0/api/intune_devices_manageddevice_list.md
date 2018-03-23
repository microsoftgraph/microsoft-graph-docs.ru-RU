# <a name="list-manageddevices"></a><span data-ttu-id="ffdeb-101">Перечисление объектов managedDevice</span><span class="sxs-lookup"><span data-stu-id="ffdeb-101">List managedDevices</span></span>

> <span data-ttu-id="ffdeb-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ffdeb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffdeb-103">Перечисление свойств и связей объектов [managedDevice](../resources/intune_devices_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ffdeb-103">List properties and relationships of the [managedDevice](../resources/intune_devices_manageddevice.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ffdeb-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ffdeb-104">Prerequisites</span></span>
<span data-ttu-id="ffdeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ffdeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ffdeb-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffdeb-107">Permission type</span></span>|<span data-ttu-id="ffdeb-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffdeb-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffdeb-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffdeb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ffdeb-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffdeb-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ffdeb-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffdeb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffdeb-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffdeb-112">Not supported.</span></span>|
|<span data-ttu-id="ffdeb-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffdeb-113">Application</span></span>|<span data-ttu-id="ffdeb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffdeb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffdeb-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffdeb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/managedDevices
GET /deviceManagement/managedDevices
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="ffdeb-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffdeb-116">Request headers</span></span>
|<span data-ttu-id="ffdeb-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffdeb-117">Header</span></span>|<span data-ttu-id="ffdeb-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ffdeb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffdeb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffdeb-119">Authorization</span></span>|<span data-ttu-id="ffdeb-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffdeb-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ffdeb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ffdeb-121">Accept</span></span>|<span data-ttu-id="ffdeb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ffdeb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffdeb-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffdeb-123">Request body</span></span>
<span data-ttu-id="ffdeb-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ffdeb-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffdeb-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffdeb-125">Response</span></span>
<span data-ttu-id="ffdeb-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDevice](../resources/intune_devices_manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ffdeb-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_devices_manageddevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffdeb-127">Пример</span><span class="sxs-lookup"><span data-stu-id="ffdeb-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="ffdeb-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffdeb-128">Request</span></span>
<span data-ttu-id="ffdeb-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffdeb-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
```

### <a name="response"></a><span data-ttu-id="ffdeb-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ffdeb-130">Response</span></span>
<span data-ttu-id="ffdeb-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ffdeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5086

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDevice",
      "id": "705c034c-034c-705c-4c03-5c704c035c70",
      "userId": "User Id value",
      "deviceName": "Device Name value",
      "deviceActionResults": [
        {
          "@odata.type": "microsoft.graph.deviceActionResult",
          "actionName": "Action Name value",
          "actionState": "pending",
          "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
          "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
        }
      ],
      "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "operatingSystem": "Operating System value",
      "complianceState": "compliant",
      "jailBroken": "Jail Broken value",
      "managementAgent": "mdm",
      "osVersion": "Os Version value",
      "easActivated": true,
      "easDeviceId": "Eas Device Id value",
      "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
      "azureADRegistered": true,
      "deviceEnrollmentType": "userEnrollment",
      "activationLockBypassCode": "Activation Lock Bypass Code value",
      "emailAddress": "Email Address value",
      "azureADDeviceId": "Azure ADDevice Id value",
      "deviceRegistrationState": "registered",
      "deviceCategoryDisplayName": "Device Category Display Name value",
      "isSupervised": true,
      "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
      "exchangeAccessState": "unknown",
      "exchangeAccessStateReason": "unknown",
      "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
      "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
      "isEncrypted": true,
      "userPrincipalName": "User Principal Name value",
      "model": "Model value",
      "manufacturer": "Manufacturer value",
      "imei": "Imei value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "serialNumber": "Serial Number value",
      "phoneNumber": "Phone Number value",
      "androidSecurityPatchLevel": "Android Security Patch Level value",
      "userDisplayName": "User Display Name value",
      "configurationManagerClientEnabledFeatures": {
        "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
        "inventory": true,
        "modernApps": true,
        "resourceAccess": true,
        "deviceConfiguration": true,
        "compliancePolicy": true,
        "windowsUpdateForBusiness": true
      },
      "wiFiMacAddress": "Wi Fi Mac Address value",
      "deviceHealthAttestationState": {
        "@odata.type": "microsoft.graph.deviceHealthAttestationState",
        "lastUpdateDateTime": "Last Update Date Time value",
        "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
        "deviceHealthAttestationStatus": "Device Health Attestation Status value",
        "contentVersion": "Content Version value",
        "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
        "attestationIdentityKey": "Attestation Identity Key value",
        "resetCount": 10,
        "restartCount": 12,
        "dataExcutionPolicy": "Data Excution Policy value",
        "bitLockerStatus": "Bit Locker Status value",
        "bootManagerVersion": "Boot Manager Version value",
        "codeIntegrityCheckVersion": "Code Integrity Check Version value",
        "secureBoot": "Secure Boot value",
        "bootDebugging": "Boot Debugging value",
        "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
        "codeIntegrity": "Code Integrity value",
        "testSigning": "Test Signing value",
        "safeMode": "Safe Mode value",
        "windowsPE": "Windows PE value",
        "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
        "virtualSecureMode": "Virtual Secure Mode value",
        "pcrHashAlgorithm": "Pcr Hash Algorithm value",
        "bootAppSecurityVersion": "Boot App Security Version value",
        "bootManagerSecurityVersion": "Boot Manager Security Version value",
        "tpmVersion": "Tpm Version value",
        "pcr0": "Pcr0 value",
        "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
        "codeIntegrityPolicy": "Code Integrity Policy value",
        "bootRevisionListInfo": "Boot Revision List Info value",
        "operatingSystemRevListInfo": "Operating System Rev List Info value",
        "healthStatusMismatchInfo": "Health Status Mismatch Info value",
        "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
      },
      "subscriberCarrier": "Subscriber Carrier value",
      "meid": "Meid value",
      "totalStorageSpaceInBytes": 8,
      "freeStorageSpaceInBytes": 7,
      "managedDeviceName": "Managed Device Name value",
      "partnerReportedThreatState": "activated"
    }
  ]
}
```



