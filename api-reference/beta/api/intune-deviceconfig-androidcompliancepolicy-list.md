---
title: Перечисление объектов androidCompliancePolicy
description: Список свойств и связей объектов androidCompliancePolicy.
ms.openlocfilehash: 32953967a7ea84f9e769ee415b79f28ce95e8f4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082257"
---
# <a name="list-androidcompliancepolicies"></a><span data-ttu-id="84d29-103">Перечисление объектов androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="84d29-103">List androidCompliancePolicies</span></span>

> <span data-ttu-id="84d29-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="84d29-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84d29-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84d29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84d29-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="84d29-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84d29-107">Список свойств и связей объектов [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="84d29-107">List properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84d29-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="84d29-108">Prerequisites</span></span>
<span data-ttu-id="84d29-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84d29-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84d29-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84d29-111">Permission type</span></span>|<span data-ttu-id="84d29-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84d29-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84d29-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84d29-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84d29-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="84d29-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="84d29-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84d29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84d29-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84d29-116">Not supported.</span></span>|
|<span data-ttu-id="84d29-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84d29-117">Application</span></span>|<span data-ttu-id="84d29-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84d29-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84d29-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84d29-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="84d29-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84d29-120">Request headers</span></span>
|<span data-ttu-id="84d29-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84d29-121">Header</span></span>|<span data-ttu-id="84d29-122">Значение</span><span class="sxs-lookup"><span data-stu-id="84d29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84d29-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84d29-123">Authorization</span></span>|<span data-ttu-id="84d29-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="84d29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84d29-125">Accept</span><span class="sxs-lookup"><span data-stu-id="84d29-125">Accept</span></span>|<span data-ttu-id="84d29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84d29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84d29-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84d29-127">Request body</span></span>
<span data-ttu-id="84d29-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84d29-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84d29-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="84d29-129">Response</span></span>
<span data-ttu-id="84d29-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84d29-130">If successful, this method returns a `200 OK` response code and a collection of [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84d29-131">Пример</span><span class="sxs-lookup"><span data-stu-id="84d29-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="84d29-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="84d29-132">Request</span></span>
<span data-ttu-id="84d29-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84d29-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="84d29-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="84d29-134">Response</span></span>
<span data-ttu-id="84d29-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="84d29-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1902

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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
      "securityRequireCompanyPortalAppIntegrity": true,
      "conditionStatementId": "Condition Statement Id value",
      "restrictedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ]
    }
  ]
}
```





