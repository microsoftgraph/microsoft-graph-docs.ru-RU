---
title: Список androidForWorkCompliancePolicies
description: Список свойств и связей объектов AndroidForWorkCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9bf12ff3b08b7f5a61bee9adae4b30ac740d1566
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130422"
---
# <a name="list-androidforworkcompliancepolicies"></a><span data-ttu-id="422e0-103">Список androidForWorkCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="422e0-103">List androidForWorkCompliancePolicies</span></span>

<span data-ttu-id="422e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="422e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="422e0-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="422e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="422e0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="422e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="422e0-107">Список свойств и связей объектов [AndroidForWorkCompliancePolicy.](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="422e0-107">List properties and relationships of the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="422e0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="422e0-108">Prerequisites</span></span>
<span data-ttu-id="422e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="422e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="422e0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="422e0-111">Permission type</span></span>|<span data-ttu-id="422e0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="422e0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="422e0-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="422e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="422e0-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422e0-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="422e0-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="422e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="422e0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="422e0-116">Not supported.</span></span>|
|<span data-ttu-id="422e0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="422e0-117">Application</span></span>|<span data-ttu-id="422e0-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422e0-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="422e0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="422e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="422e0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="422e0-120">Request headers</span></span>
|<span data-ttu-id="422e0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="422e0-121">Header</span></span>|<span data-ttu-id="422e0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="422e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="422e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="422e0-123">Authorization</span></span>|<span data-ttu-id="422e0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="422e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="422e0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="422e0-125">Accept</span></span>|<span data-ttu-id="422e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="422e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="422e0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="422e0-127">Request body</span></span>
<span data-ttu-id="422e0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="422e0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="422e0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="422e0-129">Response</span></span>
<span data-ttu-id="422e0-130">В случае успешного использования этот метод возвращает код отклика и коллекцию объектов `200 OK` [AndroidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="422e0-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="422e0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="422e0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="422e0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="422e0-132">Request</span></span>
<span data-ttu-id="422e0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="422e0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="422e0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="422e0-134">Response</span></span>
<span data-ttu-id="422e0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="422e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1616

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
      "securityRequireCompanyPortalAppIntegrity": true
    }
  ]
}
```




