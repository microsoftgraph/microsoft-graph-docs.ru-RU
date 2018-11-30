---
title: Список androidWorkProfileCompliancePolicies
description: Свойства списка и связей объектов androidWorkProfileCompliancePolicy.
ms.openlocfilehash: 5eaa8d8b6bedcfc1e70fb851cd070491689fd583
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076200"
---
# <a name="list-androidworkprofilecompliancepolicies"></a><span data-ttu-id="ffb07-103">Список androidWorkProfileCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="ffb07-103">List androidWorkProfileCompliancePolicies</span></span>

> <span data-ttu-id="ffb07-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ffb07-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffb07-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffb07-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ffb07-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ffb07-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffb07-107">Свойства списка и связей объектов [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ffb07-107">List properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ffb07-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ffb07-108">Prerequisites</span></span>
<span data-ttu-id="ffb07-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffb07-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffb07-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffb07-111">Permission type</span></span>|<span data-ttu-id="ffb07-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffb07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffb07-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffb07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ffb07-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffb07-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ffb07-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffb07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffb07-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffb07-116">Not supported.</span></span>|
|<span data-ttu-id="ffb07-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffb07-117">Application</span></span>|<span data-ttu-id="ffb07-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffb07-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffb07-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffb07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="ffb07-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffb07-120">Request headers</span></span>
|<span data-ttu-id="ffb07-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffb07-121">Header</span></span>|<span data-ttu-id="ffb07-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ffb07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffb07-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffb07-123">Authorization</span></span>|<span data-ttu-id="ffb07-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ffb07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffb07-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ffb07-125">Accept</span></span>|<span data-ttu-id="ffb07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffb07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffb07-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffb07-127">Request body</span></span>
<span data-ttu-id="ffb07-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ffb07-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffb07-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ffb07-129">Response</span></span>
<span data-ttu-id="ffb07-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ffb07-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffb07-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ffb07-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ffb07-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffb07-132">Request</span></span>
<span data-ttu-id="ffb07-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffb07-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="ffb07-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ffb07-134">Response</span></span>
<span data-ttu-id="ffb07-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ffb07-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1561

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "4e385271-5271-4e38-7152-384e7152384e",
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





