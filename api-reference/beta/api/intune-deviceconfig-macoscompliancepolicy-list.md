---
title: Перечисление объектов macOSCompliancePolicy
description: Список свойств и связей объектов macOSCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d76cf48d6ef3d305046b1e5a1171e2128ec7efce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913291"
---
# <a name="list-macoscompliancepolicies"></a><span data-ttu-id="0fe37-103">Перечисление объектов macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0fe37-103">List macOSCompliancePolicies</span></span>

> <span data-ttu-id="0fe37-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0fe37-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0fe37-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fe37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0fe37-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0fe37-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0fe37-107">Список свойств и связей объектов [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0fe37-107">List properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0fe37-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0fe37-108">Prerequisites</span></span>
<span data-ttu-id="0fe37-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fe37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fe37-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fe37-111">Permission type</span></span>|<span data-ttu-id="0fe37-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fe37-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fe37-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fe37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0fe37-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fe37-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0fe37-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fe37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fe37-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fe37-116">Not supported.</span></span>|
|<span data-ttu-id="0fe37-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fe37-117">Application</span></span>|<span data-ttu-id="0fe37-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fe37-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fe37-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fe37-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0fe37-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fe37-120">Request headers</span></span>
|<span data-ttu-id="0fe37-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0fe37-121">Header</span></span>|<span data-ttu-id="0fe37-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0fe37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fe37-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fe37-123">Authorization</span></span>|<span data-ttu-id="0fe37-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0fe37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fe37-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0fe37-125">Accept</span></span>|<span data-ttu-id="0fe37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0fe37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fe37-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0fe37-127">Request body</span></span>
<span data-ttu-id="0fe37-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0fe37-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fe37-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fe37-129">Response</span></span>
<span data-ttu-id="0fe37-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0fe37-130">If successful, this method returns a `200 OK` response code and a collection of [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fe37-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0fe37-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0fe37-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fe37-132">Request</span></span>
<span data-ttu-id="0fe37-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fe37-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="0fe37-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="0fe37-134">Response</span></span>
<span data-ttu-id="0fe37-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0fe37-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





