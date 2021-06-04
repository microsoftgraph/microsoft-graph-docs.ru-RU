---
title: Перечисление объектов managedDevice
description: Перечисление свойств и связей объектов managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: de9b927b3dde1b265c5ab71402d97e75487ec1aa
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753682"
---
# <a name="list-manageddevices"></a><span data-ttu-id="1bdb4-103">Перечисление объектов managedDevice</span><span class="sxs-lookup"><span data-stu-id="1bdb4-103">List managedDevices</span></span>

<span data-ttu-id="1bdb4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bdb4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bdb4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1bdb4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bdb4-106">Перечисление свойств и связей объектов [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1bdb4-106">List properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bdb4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1bdb4-107">Prerequisites</span></span>
<span data-ttu-id="1bdb4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bdb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bdb4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bdb4-110">Permission type</span></span>|<span data-ttu-id="1bdb4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bdb4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bdb4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bdb4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1bdb4-113">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bdb4-113">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1bdb4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bdb4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bdb4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bdb4-115">Not supported.</span></span>|
|<span data-ttu-id="1bdb4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1bdb4-116">Application</span></span>|<span data-ttu-id="1bdb4-117">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bdb4-117">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bdb4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bdb4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/managedDevices
GET /deviceManagement/managedDevices
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="1bdb4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1bdb4-119">Request headers</span></span>
|<span data-ttu-id="1bdb4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1bdb4-120">Header</span></span>|<span data-ttu-id="1bdb4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1bdb4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bdb4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bdb4-122">Authorization</span></span>|<span data-ttu-id="1bdb4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bdb4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bdb4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1bdb4-124">Accept</span></span>|<span data-ttu-id="1bdb4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1bdb4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bdb4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1bdb4-126">Request body</span></span>
<span data-ttu-id="1bdb4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1bdb4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bdb4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bdb4-128">Response</span></span>
<span data-ttu-id="1bdb4-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDevice](../resources/intune-devices-manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1bdb4-129">If successful, this method returns a `200 OK` response code and a collection of [managedDevice](../resources/intune-devices-manageddevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bdb4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1bdb4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bdb4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bdb4-131">Request</span></span>
<span data-ttu-id="1bdb4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bdb4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
```

### <a name="response"></a><span data-ttu-id="1bdb4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bdb4-133">Response</span></span>
<span data-ttu-id="1bdb4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1bdb4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5315

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDevice",
      "id": "705c034c-034c-705c-4c03-5c704c035c70",
      "userId": "User Id value",
      "deviceName": "Device Name value",
      "managedDeviceOwnerType": "company",
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
      "partnerReportedThreatState": "activated",
      "iccid": "Iccid value",
      "udid": "Udid value",
      "notes": "Notes value",
      "ethernetMacAddress": "Ethernet Mac Address value",
      "physicalMemoryInBytes": 5
    }
  ]
}
```




