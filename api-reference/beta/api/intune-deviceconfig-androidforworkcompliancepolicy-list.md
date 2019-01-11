---
title: Список androidForWorkCompliancePolicies
description: Свойства списка и связей объектов androidForWorkCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 87785352165a46a502fb79a35acaacb6dbb38133
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869120"
---
# <a name="list-androidforworkcompliancepolicies"></a><span data-ttu-id="a3cad-103">Список androidForWorkCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="a3cad-103">List androidForWorkCompliancePolicies</span></span>

> <span data-ttu-id="a3cad-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a3cad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3cad-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3cad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3cad-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a3cad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3cad-107">Свойства списка и связей объектов [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="a3cad-107">List properties and relationships of the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a3cad-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a3cad-108">Prerequisites</span></span>
<span data-ttu-id="a3cad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3cad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3cad-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3cad-111">Permission type</span></span>|<span data-ttu-id="a3cad-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3cad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3cad-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3cad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3cad-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3cad-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a3cad-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3cad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3cad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3cad-116">Not supported.</span></span>|
|<span data-ttu-id="a3cad-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3cad-117">Application</span></span>|<span data-ttu-id="a3cad-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3cad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3cad-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3cad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="a3cad-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3cad-120">Request headers</span></span>
|<span data-ttu-id="a3cad-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3cad-121">Header</span></span>|<span data-ttu-id="a3cad-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a3cad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3cad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3cad-123">Authorization</span></span>|<span data-ttu-id="a3cad-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a3cad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3cad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a3cad-125">Accept</span></span>|<span data-ttu-id="a3cad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3cad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3cad-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a3cad-127">Request body</span></span>
<span data-ttu-id="a3cad-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3cad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3cad-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3cad-129">Response</span></span>
<span data-ttu-id="a3cad-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a3cad-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3cad-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a3cad-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3cad-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3cad-132">Request</span></span>
<span data-ttu-id="a3cad-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3cad-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="a3cad-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3cad-134">Response</span></span>
<span data-ttu-id="a3cad-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a3cad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1557

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "a8d667bd-67bd-a8d6-bd67-d6a8bd67d6a8",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordMinimumLength": 5,
      "passwordRequiredType": "alphabetic",
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordPreviousPasswordBlockCount": 2,
      "securityPreventInstallAppsFromUnknownSources": true,
      "securityDisableUsbDebugging": true,
      "securityRequireVerifyApps": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "securityBlockJailbrokenDevices": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
      "storageRequireEncryption": true,
      "securityRequireSafetyNetAttestationBasicIntegrity": true,
      "securityRequireSafetyNetAttestationCertifiedDevice": true,
      "securityRequireGooglePlayServices": true,
      "securityRequireUpToDateSecurityProviders": true,
      "securityRequireCompanyPortalAppIntegrity": true
    }
  ]
}
```





