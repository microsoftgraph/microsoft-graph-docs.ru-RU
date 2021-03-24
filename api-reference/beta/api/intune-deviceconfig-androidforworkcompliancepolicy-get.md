---
title: Get AndroidForWorkCompliancePolicy
description: Чтение свойств и связей объекта AndroidForWorkCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1122b1a64d433ee943d1fd028bd2a28cfcd4206e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130429"
---
# <a name="get-androidforworkcompliancepolicy"></a><span data-ttu-id="9f8ac-103">Get AndroidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9f8ac-103">Get androidForWorkCompliancePolicy</span></span>

<span data-ttu-id="9f8ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f8ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f8ac-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f8ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f8ac-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f8ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f8ac-107">Чтение свойств и связей объекта [AndroidForWorkCompliancePolicy.](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9f8ac-107">Read properties and relationships of the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f8ac-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f8ac-108">Prerequisites</span></span>
<span data-ttu-id="9f8ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f8ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f8ac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f8ac-111">Permission type</span></span>|<span data-ttu-id="9f8ac-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f8ac-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f8ac-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f8ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f8ac-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f8ac-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f8ac-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f8ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f8ac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f8ac-116">Not supported.</span></span>|
|<span data-ttu-id="9f8ac-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9f8ac-117">Application</span></span>|<span data-ttu-id="9f8ac-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f8ac-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f8ac-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f8ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f8ac-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9f8ac-120">Optional query parameters</span></span>
<span data-ttu-id="9f8ac-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9f8ac-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f8ac-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f8ac-122">Request headers</span></span>
|<span data-ttu-id="9f8ac-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f8ac-123">Header</span></span>|<span data-ttu-id="9f8ac-124">Значение</span><span class="sxs-lookup"><span data-stu-id="9f8ac-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f8ac-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f8ac-125">Authorization</span></span>|<span data-ttu-id="9f8ac-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f8ac-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f8ac-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9f8ac-127">Accept</span></span>|<span data-ttu-id="9f8ac-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9f8ac-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f8ac-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f8ac-129">Request body</span></span>
<span data-ttu-id="9f8ac-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f8ac-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f8ac-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f8ac-131">Response</span></span>
<span data-ttu-id="9f8ac-132">В случае успешного использования этот метод возвращает код отклика и `200 OK` [объект AndroidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9f8ac-132">If successful, this method returns a `200 OK` response code and [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f8ac-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9f8ac-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f8ac-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f8ac-134">Request</span></span>
<span data-ttu-id="9f8ac-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f8ac-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="9f8ac-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f8ac-136">Response</span></span>
<span data-ttu-id="9f8ac-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f8ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1538

{
  "value": {
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
}
```




