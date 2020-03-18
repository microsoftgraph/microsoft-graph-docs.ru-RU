---
title: Get androidCompliancePolicy
description: Чтение свойств и связей объекта androidCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c45752ef3d67d40a9769959e48a0f6d7572c45c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759964"
---
# <a name="get-androidcompliancepolicy"></a><span data-ttu-id="19f08-103">Get androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="19f08-103">Get androidCompliancePolicy</span></span>

> <span data-ttu-id="19f08-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19f08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19f08-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19f08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19f08-106">Чтение свойств и связей объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="19f08-106">Read properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19f08-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="19f08-107">Prerequisites</span></span>
<span data-ttu-id="19f08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19f08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19f08-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19f08-110">Permission type</span></span>|<span data-ttu-id="19f08-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19f08-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19f08-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19f08-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19f08-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="19f08-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="19f08-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19f08-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19f08-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19f08-115">Not supported.</span></span>|
|<span data-ttu-id="19f08-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="19f08-116">Application</span></span>|<span data-ttu-id="19f08-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="19f08-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19f08-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19f08-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19f08-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="19f08-119">Optional query parameters</span></span>
<span data-ttu-id="19f08-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="19f08-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19f08-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19f08-121">Request headers</span></span>
|<span data-ttu-id="19f08-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19f08-122">Header</span></span>|<span data-ttu-id="19f08-123">Значение</span><span class="sxs-lookup"><span data-stu-id="19f08-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19f08-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="19f08-124">Authorization</span></span>|<span data-ttu-id="19f08-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19f08-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19f08-126">Accept</span><span class="sxs-lookup"><span data-stu-id="19f08-126">Accept</span></span>|<span data-ttu-id="19f08-127">application/json</span><span class="sxs-lookup"><span data-stu-id="19f08-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19f08-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19f08-128">Request body</span></span>
<span data-ttu-id="19f08-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19f08-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19f08-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="19f08-130">Response</span></span>
<span data-ttu-id="19f08-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="19f08-131">If successful, this method returns a `200 OK` response code and [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19f08-132">Пример</span><span class="sxs-lookup"><span data-stu-id="19f08-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="19f08-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="19f08-133">Request</span></span>
<span data-ttu-id="19f08-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19f08-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="19f08-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="19f08-135">Response</span></span>
<span data-ttu-id="19f08-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19f08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1989

{
  "value": {
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
}
```




