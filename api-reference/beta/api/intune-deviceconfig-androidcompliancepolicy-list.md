---
title: Перечисление объектов androidCompliancePolicy
description: Список свойств и связей объектов androidCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 77bdbde21a6baf723c2e691d4c2622104cc12201
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450127"
---
# <a name="list-androidcompliancepolicies"></a><span data-ttu-id="df7cd-103">Перечисление объектов androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="df7cd-103">List androidCompliancePolicies</span></span>

<span data-ttu-id="df7cd-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="df7cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df7cd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df7cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df7cd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="df7cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df7cd-107">Список свойств и связей объектов [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="df7cd-107">List properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df7cd-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="df7cd-108">Prerequisites</span></span>
<span data-ttu-id="df7cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df7cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df7cd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df7cd-111">Permission type</span></span>|<span data-ttu-id="df7cd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="df7cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df7cd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df7cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df7cd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="df7cd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="df7cd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df7cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df7cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df7cd-116">Not supported.</span></span>|
|<span data-ttu-id="df7cd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df7cd-117">Application</span></span>|<span data-ttu-id="df7cd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="df7cd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df7cd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df7cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="df7cd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="df7cd-120">Request headers</span></span>
|<span data-ttu-id="df7cd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="df7cd-121">Header</span></span>|<span data-ttu-id="df7cd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="df7cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df7cd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df7cd-123">Authorization</span></span>|<span data-ttu-id="df7cd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df7cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df7cd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="df7cd-125">Accept</span></span>|<span data-ttu-id="df7cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df7cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df7cd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df7cd-127">Request body</span></span>
<span data-ttu-id="df7cd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="df7cd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df7cd-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="df7cd-129">Response</span></span>
<span data-ttu-id="df7cd-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="df7cd-130">If successful, this method returns a `200 OK` response code and a collection of [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df7cd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="df7cd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="df7cd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="df7cd-132">Request</span></span>
<span data-ttu-id="df7cd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df7cd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="df7cd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="df7cd-134">Response</span></span>
<span data-ttu-id="df7cd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df7cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2091

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
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "securityPreventInstallAppsFromUnknownSources": true,
      "securityDisableUsbDebugging": true,
      "securityRequireVerifyApps": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "advancedThreatProtectionRequiredSecurityLevel": "secured",
      "securityBlockJailbrokenDevices": true,
      "securityBlockDeviceAdministratorManagedDevices": true,
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





