---
title: Перечисление объектов windows10CompliancePolicy
description: Список свойств и связей объектов windows10CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 31a8032c3be6874d35e35e422af065b2f38dd336
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129484"
---
# <a name="list-windows10compliancepolicies"></a><span data-ttu-id="74c75-103">Перечисление объектов windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="74c75-103">List windows10CompliancePolicies</span></span>

<span data-ttu-id="74c75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74c75-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74c75-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74c75-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74c75-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74c75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74c75-107">Список свойств и связей объектов [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="74c75-107">List properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74c75-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="74c75-108">Prerequisites</span></span>
<span data-ttu-id="74c75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74c75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74c75-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74c75-111">Permission type</span></span>|<span data-ttu-id="74c75-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74c75-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74c75-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74c75-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74c75-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74c75-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74c75-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74c75-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74c75-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74c75-116">Not supported.</span></span>|
|<span data-ttu-id="74c75-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="74c75-117">Application</span></span>|<span data-ttu-id="74c75-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74c75-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74c75-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74c75-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="74c75-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="74c75-120">Request headers</span></span>
|<span data-ttu-id="74c75-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74c75-121">Header</span></span>|<span data-ttu-id="74c75-122">Значение</span><span class="sxs-lookup"><span data-stu-id="74c75-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74c75-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74c75-123">Authorization</span></span>|<span data-ttu-id="74c75-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74c75-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74c75-125">Accept</span><span class="sxs-lookup"><span data-stu-id="74c75-125">Accept</span></span>|<span data-ttu-id="74c75-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74c75-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74c75-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74c75-127">Request body</span></span>
<span data-ttu-id="74c75-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="74c75-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74c75-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="74c75-129">Response</span></span>
<span data-ttu-id="74c75-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="74c75-130">If successful, this method returns a `200 OK` response code and a collection of [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74c75-131">Пример</span><span class="sxs-lookup"><span data-stu-id="74c75-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="74c75-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="74c75-132">Request</span></span>
<span data-ttu-id="74c75-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74c75-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="74c75-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="74c75-134">Response</span></span>
<span data-ttu-id="74c75-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74c75-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2328

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "2919ae62-ae62-2919-62ae-192962ae1929",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordRequiredToUnlockFromIdle": true,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "requireHealthyDeviceReport": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
      "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
      "earlyLaunchAntiMalwareDriverEnabled": true,
      "bitLockerEnabled": true,
      "secureBootEnabled": true,
      "codeIntegrityEnabled": true,
      "storageRequireEncryption": true,
      "activeFirewallRequired": true,
      "defenderEnabled": true,
      "defenderVersion": "Defender Version value",
      "signatureOutOfDate": true,
      "rtpEnabled": true,
      "antivirusRequired": true,
      "antiSpywareRequired": true,
      "validOperatingSystemBuildRanges": [
        {
          "@odata.type": "microsoft.graph.operatingSystemVersionRange",
          "description": "Description value",
          "lowestVersion": "Lowest Version value",
          "highestVersion": "Highest Version value"
        }
      ],
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "configurationManagerComplianceRequired": true,
      "tpmRequired": true,
      "deviceCompliancePolicyScript": {
        "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
        "deviceComplianceScriptId": "Device Compliance Script Id value",
        "rulesContent": "cnVsZXNDb250ZW50"
      }
    }
  ]
}
```




