---
title: Get windows10CompliancePolicy
description: Чтение свойств и связей объекта windows10CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 667bb37b3b0b8dd9723e507717b4514b148b923a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129512"
---
# <a name="get-windows10compliancepolicy"></a><span data-ttu-id="4f6f0-103">Get windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4f6f0-103">Get windows10CompliancePolicy</span></span>

<span data-ttu-id="4f6f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f6f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f6f0-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f6f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f6f0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f6f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f6f0-107">Чтение свойств и связей объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4f6f0-107">Read properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f6f0-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4f6f0-108">Prerequisites</span></span>
<span data-ttu-id="4f6f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f6f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f6f0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f6f0-111">Permission type</span></span>|<span data-ttu-id="4f6f0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f6f0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f6f0-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f6f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f6f0-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f6f0-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f6f0-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f6f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f6f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f6f0-116">Not supported.</span></span>|
|<span data-ttu-id="4f6f0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4f6f0-117">Application</span></span>|<span data-ttu-id="4f6f0-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f6f0-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f6f0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f6f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f6f0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4f6f0-120">Optional query parameters</span></span>
<span data-ttu-id="4f6f0-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4f6f0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f6f0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f6f0-122">Request headers</span></span>
|<span data-ttu-id="4f6f0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f6f0-123">Header</span></span>|<span data-ttu-id="4f6f0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4f6f0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f6f0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f6f0-125">Authorization</span></span>|<span data-ttu-id="4f6f0-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f6f0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f6f0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4f6f0-127">Accept</span></span>|<span data-ttu-id="4f6f0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4f6f0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f6f0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f6f0-129">Request body</span></span>
<span data-ttu-id="4f6f0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f6f0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f6f0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6f0-131">Response</span></span>
<span data-ttu-id="4f6f0-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4f6f0-132">If successful, this method returns a `200 OK` response code and [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f6f0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4f6f0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f6f0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6f0-134">Request</span></span>
<span data-ttu-id="4f6f0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f6f0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="4f6f0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6f0-136">Response</span></span>
<span data-ttu-id="4f6f0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f6f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2208

{
  "value": {
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
}
```




