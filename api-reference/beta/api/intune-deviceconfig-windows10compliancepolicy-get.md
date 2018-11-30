---
title: Get windows10CompliancePolicy
description: Чтение свойств и связей объекта windows10CompliancePolicy.
ms.openlocfilehash: 1e9f6910265e9ee89c9f22ab1876408214858dab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076774"
---
# <a name="get-windows10compliancepolicy"></a><span data-ttu-id="12e4a-103">Get windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="12e4a-103">Get windows10CompliancePolicy</span></span>

> <span data-ttu-id="12e4a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="12e4a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12e4a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12e4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12e4a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="12e4a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12e4a-107">Чтение свойств и связей объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="12e4a-107">Read properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12e4a-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="12e4a-108">Prerequisites</span></span>
<span data-ttu-id="12e4a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12e4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12e4a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12e4a-111">Permission type</span></span>|<span data-ttu-id="12e4a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12e4a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12e4a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12e4a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12e4a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="12e4a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="12e4a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12e4a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12e4a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12e4a-116">Not supported.</span></span>|
|<span data-ttu-id="12e4a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12e4a-117">Application</span></span>|<span data-ttu-id="12e4a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12e4a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12e4a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12e4a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12e4a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="12e4a-120">Optional query parameters</span></span>
<span data-ttu-id="12e4a-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="12e4a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="12e4a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12e4a-122">Request headers</span></span>
|<span data-ttu-id="12e4a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12e4a-123">Header</span></span>|<span data-ttu-id="12e4a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="12e4a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12e4a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="12e4a-125">Authorization</span></span>|<span data-ttu-id="12e4a-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="12e4a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12e4a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="12e4a-127">Accept</span></span>|<span data-ttu-id="12e4a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="12e4a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12e4a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12e4a-129">Request body</span></span>
<span data-ttu-id="12e4a-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12e4a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12e4a-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="12e4a-131">Response</span></span>
<span data-ttu-id="12e4a-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="12e4a-132">If successful, this method returns a `200 OK` response code and [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12e4a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="12e4a-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="12e4a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="12e4a-134">Request</span></span>
<span data-ttu-id="12e4a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12e4a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="12e4a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="12e4a-136">Response</span></span>
<span data-ttu-id="12e4a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="12e4a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1951

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
    "configurationManagerComplianceRequired": true
  }
}
```





