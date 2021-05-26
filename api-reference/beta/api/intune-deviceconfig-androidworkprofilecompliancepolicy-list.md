---
title: Список androidWorkProfileCompliancePolicies
description: Список свойств и связей объектов AndroidWorkProfileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b4e7b3cadf24f1581aba02f1d3a292ce650fa4d4
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665478"
---
# <a name="list-androidworkprofilecompliancepolicies"></a><span data-ttu-id="cb990-103">Список androidWorkProfileCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="cb990-103">List androidWorkProfileCompliancePolicies</span></span>

<span data-ttu-id="cb990-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb990-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb990-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb990-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb990-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb990-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb990-107">Список свойств и связей объектов [AndroidWorkProfileCompliancePolicy.](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cb990-107">List properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb990-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cb990-108">Prerequisites</span></span>
<span data-ttu-id="cb990-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb990-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb990-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb990-111">Permission type</span></span>|<span data-ttu-id="cb990-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb990-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb990-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb990-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb990-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb990-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cb990-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb990-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb990-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb990-116">Not supported.</span></span>|
|<span data-ttu-id="cb990-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cb990-117">Application</span></span>|<span data-ttu-id="cb990-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb990-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb990-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb990-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="cb990-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cb990-120">Request headers</span></span>
|<span data-ttu-id="cb990-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb990-121">Header</span></span>|<span data-ttu-id="cb990-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cb990-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb990-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb990-123">Authorization</span></span>|<span data-ttu-id="cb990-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb990-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb990-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cb990-125">Accept</span></span>|<span data-ttu-id="cb990-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb990-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb990-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb990-127">Request body</span></span>
<span data-ttu-id="cb990-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb990-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb990-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb990-129">Response</span></span>
<span data-ttu-id="cb990-130">В случае успешного использования этот метод возвращает код отклика и коллекцию объектов `200 OK` [AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cb990-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb990-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cb990-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb990-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb990-132">Request</span></span>
<span data-ttu-id="cb990-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb990-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="cb990-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb990-134">Response</span></span>
<span data-ttu-id="cb990-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb990-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1762

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
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "securityPreventInstallAppsFromUnknownSources": true,
      "securityDisableUsbDebugging": true,
      "securityRequireVerifyApps": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "advancedThreatProtectionRequiredSecurityLevel": "secured",
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
      "securityRequiredAndroidSafetyNetEvaluationType": "hardwareBacked"
    }
  ]
}
```




