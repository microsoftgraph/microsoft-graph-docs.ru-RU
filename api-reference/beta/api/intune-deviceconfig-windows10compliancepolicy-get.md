---
title: Get windows10CompliancePolicy
description: Чтение свойств и связей объекта windows10CompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ee2e169775187ce7fd3354e51286bbd014e10b0d
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38082838"
---
# <a name="get-windows10compliancepolicy"></a><span data-ttu-id="1dd28-103">Get windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="1dd28-103">Get windows10CompliancePolicy</span></span>

> <span data-ttu-id="1dd28-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dd28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dd28-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1dd28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dd28-106">Чтение свойств и связей объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1dd28-106">Read properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dd28-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1dd28-107">Prerequisites</span></span>
<span data-ttu-id="1dd28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dd28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dd28-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dd28-110">Permission type</span></span>|<span data-ttu-id="1dd28-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dd28-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dd28-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dd28-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1dd28-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dd28-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1dd28-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dd28-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dd28-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dd28-115">Not supported.</span></span>|
|<span data-ttu-id="1dd28-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1dd28-116">Application</span></span>|<span data-ttu-id="1dd28-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dd28-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dd28-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dd28-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1dd28-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1dd28-119">Optional query parameters</span></span>
<span data-ttu-id="1dd28-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1dd28-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1dd28-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1dd28-121">Request headers</span></span>
|<span data-ttu-id="1dd28-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1dd28-122">Header</span></span>|<span data-ttu-id="1dd28-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1dd28-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dd28-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1dd28-124">Authorization</span></span>|<span data-ttu-id="1dd28-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1dd28-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dd28-126">Accept</span><span class="sxs-lookup"><span data-stu-id="1dd28-126">Accept</span></span>|<span data-ttu-id="1dd28-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1dd28-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dd28-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1dd28-128">Request body</span></span>
<span data-ttu-id="1dd28-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1dd28-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dd28-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="1dd28-130">Response</span></span>
<span data-ttu-id="1dd28-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1dd28-131">If successful, this method returns a `200 OK` response code and [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dd28-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1dd28-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dd28-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dd28-133">Request</span></span>
<span data-ttu-id="1dd28-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1dd28-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="1dd28-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dd28-135">Response</span></span>
<span data-ttu-id="1dd28-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1dd28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1977

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
    "tpmRequired": true
  }
}
```






