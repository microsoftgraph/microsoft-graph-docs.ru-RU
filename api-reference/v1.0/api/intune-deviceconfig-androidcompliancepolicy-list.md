---
title: Перечисление объектов androidCompliancePolicy
description: Список свойств и связей объектов androidCompliancePolicy.
ms.openlocfilehash: 289529aaa56e55b5a6c66fd1335ceaa8e8e565df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025428"
---
# <a name="list-androidcompliancepolicies"></a><span data-ttu-id="1151e-103">Перечисление объектов androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="1151e-103">List androidCompliancePolicies</span></span>

> <span data-ttu-id="1151e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1151e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1151e-105">Список свойств и связей объектов [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1151e-105">List properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1151e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1151e-106">Prerequisites</span></span>
<span data-ttu-id="1151e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1151e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1151e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1151e-109">Permission type</span></span>|<span data-ttu-id="1151e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1151e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1151e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1151e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1151e-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1151e-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1151e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1151e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1151e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1151e-114">Not supported.</span></span>|
|<span data-ttu-id="1151e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1151e-115">Application</span></span>|<span data-ttu-id="1151e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1151e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1151e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1151e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="1151e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1151e-118">Request headers</span></span>
|<span data-ttu-id="1151e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1151e-119">Header</span></span>|<span data-ttu-id="1151e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1151e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1151e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1151e-121">Authorization</span></span>|<span data-ttu-id="1151e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1151e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1151e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1151e-123">Accept</span></span>|<span data-ttu-id="1151e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1151e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1151e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1151e-125">Request body</span></span>
<span data-ttu-id="1151e-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1151e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1151e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1151e-127">Response</span></span>
<span data-ttu-id="1151e-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1151e-128">If successful, this method returns a `200 OK` response code and a collection of [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1151e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1151e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="1151e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1151e-130">Request</span></span>
<span data-ttu-id="1151e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1151e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="1151e-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="1151e-132">Response</span></span>
<span data-ttu-id="1151e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1151e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1476

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidCompliancePolicy",
      "id": "752c820f-820f-752c-0f82-2c750f822c75",
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



