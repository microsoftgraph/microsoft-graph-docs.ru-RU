---
title: Get AndroidWorkProfileCompliancePolicy
description: Чтение свойств и связей объекта AndroidWorkProfileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f314f32f2217c9b9da7e2dbf842b4f42349f8bde
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665485"
---
# <a name="get-androidworkprofilecompliancepolicy"></a><span data-ttu-id="e2724-103">Get AndroidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e2724-103">Get androidWorkProfileCompliancePolicy</span></span>

<span data-ttu-id="e2724-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2724-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2724-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2724-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2724-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2724-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2724-107">Чтение свойств и связей объекта [AndroidWorkProfileCompliancePolicy.](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e2724-107">Read properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2724-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e2724-108">Prerequisites</span></span>
<span data-ttu-id="e2724-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2724-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2724-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2724-111">Permission type</span></span>|<span data-ttu-id="e2724-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2724-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2724-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2724-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2724-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2724-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2724-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2724-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2724-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2724-116">Not supported.</span></span>|
|<span data-ttu-id="e2724-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e2724-117">Application</span></span>|<span data-ttu-id="e2724-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2724-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2724-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2724-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2724-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e2724-120">Optional query parameters</span></span>
<span data-ttu-id="e2724-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e2724-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2724-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2724-122">Request headers</span></span>
|<span data-ttu-id="e2724-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2724-123">Header</span></span>|<span data-ttu-id="e2724-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e2724-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2724-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2724-125">Authorization</span></span>|<span data-ttu-id="e2724-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2724-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2724-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e2724-127">Accept</span></span>|<span data-ttu-id="e2724-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e2724-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2724-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2724-129">Request body</span></span>
<span data-ttu-id="e2724-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2724-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2724-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2724-131">Response</span></span>
<span data-ttu-id="e2724-132">В случае успешного использования этот метод возвращает код отклика и `200 OK` [объект AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e2724-132">If successful, this method returns a `200 OK` response code and [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2724-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e2724-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2724-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2724-134">Request</span></span>
<span data-ttu-id="e2724-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2724-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="e2724-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2724-136">Response</span></span>
<span data-ttu-id="e2724-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2724-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1680

{
  "value": {
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
}
```




