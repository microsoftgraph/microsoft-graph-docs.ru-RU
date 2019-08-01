---
title: Получение managedDevice
description: Чтение свойств и связей объекта managedDevice.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 778b01e5b03cbcc49cebe21890634aa43be0797e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020985"
---
# <a name="get-manageddevice"></a><span data-ttu-id="bb197-103">Получение managedDevice</span><span class="sxs-lookup"><span data-stu-id="bb197-103">Get managedDevice</span></span>

> <span data-ttu-id="bb197-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb197-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb197-105">Чтение свойств и связей объекта [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="bb197-105">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb197-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bb197-106">Prerequisites</span></span>
<span data-ttu-id="bb197-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb197-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb197-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb197-109">Permission type</span></span>|<span data-ttu-id="bb197-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb197-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb197-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb197-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb197-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb197-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="bb197-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb197-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb197-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb197-114">Not supported.</span></span>|
|<span data-ttu-id="bb197-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb197-115">Application</span></span>|<span data-ttu-id="bb197-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb197-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb197-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb197-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/managedDevices/{managedDeviceId}
GET /deviceManagement/managedDevices/{managedDeviceId}
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb197-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bb197-118">Optional query parameters</span></span>
<span data-ttu-id="bb197-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bb197-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb197-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb197-120">Request headers</span></span>
|<span data-ttu-id="bb197-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb197-121">Header</span></span>|<span data-ttu-id="bb197-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bb197-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb197-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb197-123">Authorization</span></span>|<span data-ttu-id="bb197-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb197-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb197-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bb197-125">Accept</span></span>|<span data-ttu-id="bb197-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb197-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb197-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bb197-127">Request body</span></span>
<span data-ttu-id="bb197-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb197-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb197-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb197-129">Response</span></span>
<span data-ttu-id="bb197-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [managedDevice](../resources/intune-devices-manageddevice.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bb197-130">If successful, this method returns a `200 OK` response code and [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb197-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bb197-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb197-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb197-132">Request</span></span>
<span data-ttu-id="bb197-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb197-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}
```

### <a name="response"></a><span data-ttu-id="bb197-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb197-134">Response</span></span>
<span data-ttu-id="bb197-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb197-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4920

{
  "value": {
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
    "partnerReportedThreatState": "activated"
  }
}
```



