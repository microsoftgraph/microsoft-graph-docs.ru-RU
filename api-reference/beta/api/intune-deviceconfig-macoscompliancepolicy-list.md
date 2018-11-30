---
title: Перечисление объектов macOSCompliancePolicy
description: Список свойств и связей объектов macOSCompliancePolicy.
ms.openlocfilehash: 3164297670b0402bd51428928577f3c3ad4134d9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076478"
---
# <a name="list-macoscompliancepolicies"></a><span data-ttu-id="fc6a8-103">Перечисление объектов macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="fc6a8-103">List macOSCompliancePolicies</span></span>

> <span data-ttu-id="fc6a8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fc6a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc6a8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc6a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc6a8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fc6a8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc6a8-107">Список свойств и связей объектов [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fc6a8-107">List properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fc6a8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fc6a8-108">Prerequisites</span></span>
<span data-ttu-id="fc6a8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc6a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc6a8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc6a8-111">Permission type</span></span>|<span data-ttu-id="fc6a8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc6a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc6a8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc6a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc6a8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc6a8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fc6a8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc6a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc6a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc6a8-116">Not supported.</span></span>|
|<span data-ttu-id="fc6a8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc6a8-117">Application</span></span>|<span data-ttu-id="fc6a8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc6a8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc6a8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc6a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="fc6a8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc6a8-120">Request headers</span></span>
|<span data-ttu-id="fc6a8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc6a8-121">Header</span></span>|<span data-ttu-id="fc6a8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fc6a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc6a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc6a8-123">Authorization</span></span>|<span data-ttu-id="fc6a8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fc6a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc6a8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fc6a8-125">Accept</span></span>|<span data-ttu-id="fc6a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc6a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc6a8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc6a8-127">Request body</span></span>
<span data-ttu-id="fc6a8-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc6a8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc6a8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc6a8-129">Response</span></span>
<span data-ttu-id="fc6a8-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc6a8-130">If successful, this method returns a `200 OK` response code and a collection of [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc6a8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fc6a8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fc6a8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc6a8-132">Request</span></span>
<span data-ttu-id="fc6a8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc6a8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="fc6a8-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc6a8-134">Response</span></span>
<span data-ttu-id="fc6a8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="fc6a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1276

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "systemIntegrityProtectionEnabled": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "storageRequireEncryption": true,
      "gatekeeperAllowedAppSource": "macAppStore",
      "firewallEnabled": true,
      "firewallBlockAllIncoming": true,
      "firewallEnableStealthMode": true
    }
  ]
}
```





