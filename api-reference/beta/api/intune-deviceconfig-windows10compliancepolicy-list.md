---
title: Перечисление объектов windows10CompliancePolicy
description: Список свойств и связей объектов windows10CompliancePolicy.
author: tfitzmac
ms.openlocfilehash: e4c385464c758aed782b7dd1ea8f5d6d51f92c1b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308101"
---
# <a name="list-windows10compliancepolicies"></a><span data-ttu-id="63185-103">Перечисление объектов windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="63185-103">List windows10CompliancePolicies</span></span>

> <span data-ttu-id="63185-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="63185-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63185-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63185-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63185-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="63185-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63185-107">Список свойств и связей объектов [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="63185-107">List properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="63185-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="63185-108">Prerequisites</span></span>
<span data-ttu-id="63185-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63185-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63185-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63185-111">Permission type</span></span>|<span data-ttu-id="63185-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="63185-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63185-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63185-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63185-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63185-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="63185-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63185-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63185-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63185-116">Not supported.</span></span>|
|<span data-ttu-id="63185-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63185-117">Application</span></span>|<span data-ttu-id="63185-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63185-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63185-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63185-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="63185-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63185-120">Request headers</span></span>
|<span data-ttu-id="63185-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63185-121">Header</span></span>|<span data-ttu-id="63185-122">Значение</span><span class="sxs-lookup"><span data-stu-id="63185-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63185-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63185-123">Authorization</span></span>|<span data-ttu-id="63185-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="63185-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63185-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63185-125">Accept</span></span>|<span data-ttu-id="63185-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63185-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63185-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63185-127">Request body</span></span>
<span data-ttu-id="63185-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63185-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63185-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="63185-129">Response</span></span>
<span data-ttu-id="63185-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="63185-130">If successful, this method returns a `200 OK` response code and a collection of [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63185-131">Пример</span><span class="sxs-lookup"><span data-stu-id="63185-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="63185-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="63185-132">Request</span></span>
<span data-ttu-id="63185-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63185-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="63185-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="63185-134">Response</span></span>
<span data-ttu-id="63185-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="63185-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2059

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
      "configurationManagerComplianceRequired": true
    }
  ]
}
```





