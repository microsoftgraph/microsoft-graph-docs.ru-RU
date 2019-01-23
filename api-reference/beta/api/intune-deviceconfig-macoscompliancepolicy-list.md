---
title: Перечисление объектов macOSCompliancePolicy
description: Список свойств и связей объектов macOSCompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 374c65b1b219be31bd591ac485ec3b0fec2ec1ca
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411759"
---
# <a name="list-macoscompliancepolicies"></a><span data-ttu-id="cb90d-103">Перечисление объектов macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="cb90d-103">List macOSCompliancePolicies</span></span>

> <span data-ttu-id="cb90d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cb90d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cb90d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb90d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb90d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb90d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb90d-107">Список свойств и связей объектов [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cb90d-107">List properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb90d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cb90d-108">Prerequisites</span></span>
<span data-ttu-id="cb90d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cb90d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cb90d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb90d-111">Permission type</span></span>|<span data-ttu-id="cb90d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb90d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb90d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb90d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb90d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb90d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cb90d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb90d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb90d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb90d-116">Not supported.</span></span>|
|<span data-ttu-id="cb90d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb90d-117">Application</span></span>|<span data-ttu-id="cb90d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb90d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb90d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb90d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="cb90d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb90d-120">Request headers</span></span>
|<span data-ttu-id="cb90d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb90d-121">Header</span></span>|<span data-ttu-id="cb90d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cb90d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb90d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb90d-123">Authorization</span></span>|<span data-ttu-id="cb90d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cb90d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb90d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cb90d-125">Accept</span></span>|<span data-ttu-id="cb90d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb90d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb90d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb90d-127">Request body</span></span>
<span data-ttu-id="cb90d-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb90d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb90d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb90d-129">Response</span></span>
<span data-ttu-id="cb90d-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cb90d-130">If successful, this method returns a `200 OK` response code and a collection of [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb90d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cb90d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb90d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb90d-132">Request</span></span>
<span data-ttu-id="cb90d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb90d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="cb90d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb90d-134">Response</span></span>
<span data-ttu-id="cb90d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cb90d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1408

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
      "osMinimumBuildVersion": "Os Minimum Build Version value",
      "osMaximumBuildVersion": "Os Maximum Build Version value",
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




