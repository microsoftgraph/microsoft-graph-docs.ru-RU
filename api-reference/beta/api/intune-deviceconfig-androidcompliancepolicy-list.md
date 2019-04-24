---
title: Перечисление объектов androidCompliancePolicy
description: Список свойств и связей объектов androidCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbf4d7483ee4ed7ff114fce957cf57b2cb92d9ca
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32481243"
---
# <a name="list-androidcompliancepolicies"></a><span data-ttu-id="64f1c-103">Перечисление объектов androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="64f1c-103">List androidCompliancePolicies</span></span>

> <span data-ttu-id="64f1c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64f1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64f1c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64f1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64f1c-106">Список свойств и связей объектов [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="64f1c-106">List properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64f1c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="64f1c-107">Prerequisites</span></span>
<span data-ttu-id="64f1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64f1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64f1c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64f1c-110">Permission type</span></span>|<span data-ttu-id="64f1c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64f1c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64f1c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64f1c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64f1c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="64f1c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="64f1c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64f1c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64f1c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64f1c-115">Not supported.</span></span>|
|<span data-ttu-id="64f1c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64f1c-116">Application</span></span>|<span data-ttu-id="64f1c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64f1c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64f1c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64f1c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="64f1c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64f1c-119">Request headers</span></span>
|<span data-ttu-id="64f1c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64f1c-120">Header</span></span>|<span data-ttu-id="64f1c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="64f1c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64f1c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64f1c-122">Authorization</span></span>|<span data-ttu-id="64f1c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64f1c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64f1c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="64f1c-124">Accept</span></span>|<span data-ttu-id="64f1c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64f1c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64f1c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64f1c-126">Request body</span></span>
<span data-ttu-id="64f1c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64f1c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64f1c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="64f1c-128">Response</span></span>
<span data-ttu-id="64f1c-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64f1c-129">If successful, this method returns a `200 OK` response code and a collection of [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64f1c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="64f1c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="64f1c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="64f1c-131">Request</span></span>
<span data-ttu-id="64f1c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64f1c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="64f1c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="64f1c-133">Response</span></span>
<span data-ttu-id="64f1c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64f1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1961

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





