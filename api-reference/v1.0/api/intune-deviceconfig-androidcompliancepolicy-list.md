---
title: Перечисление объектов androidCompliancePolicy
description: Список свойств и связей объектов androidCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cca1a2fa5257713e1e7e3016d24029eed5e199c5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759380"
---
# <a name="list-androidcompliancepolicies"></a><span data-ttu-id="527b0-103">Перечисление объектов androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="527b0-103">List androidCompliancePolicies</span></span>

<span data-ttu-id="527b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="527b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="527b0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="527b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="527b0-106">Список свойств и связей объектов [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="527b0-106">List properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="527b0-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="527b0-107">Prerequisites</span></span>
<span data-ttu-id="527b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="527b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="527b0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="527b0-110">Permission type</span></span>|<span data-ttu-id="527b0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="527b0-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="527b0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="527b0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="527b0-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="527b0-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="527b0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="527b0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="527b0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="527b0-115">Not supported.</span></span>|
|<span data-ttu-id="527b0-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="527b0-116">Application</span></span>|<span data-ttu-id="527b0-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="527b0-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="527b0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="527b0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="527b0-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="527b0-119">Request headers</span></span>
|<span data-ttu-id="527b0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="527b0-120">Header</span></span>|<span data-ttu-id="527b0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="527b0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="527b0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="527b0-122">Authorization</span></span>|<span data-ttu-id="527b0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="527b0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="527b0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="527b0-124">Accept</span></span>|<span data-ttu-id="527b0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="527b0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="527b0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="527b0-126">Request body</span></span>
<span data-ttu-id="527b0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="527b0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="527b0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="527b0-128">Response</span></span>
<span data-ttu-id="527b0-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="527b0-129">If successful, this method returns a `200 OK` response code and a collection of [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="527b0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="527b0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="527b0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="527b0-131">Request</span></span>
<span data-ttu-id="527b0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="527b0-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="527b0-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="527b0-133">Response</span></span>
<span data-ttu-id="527b0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="527b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




