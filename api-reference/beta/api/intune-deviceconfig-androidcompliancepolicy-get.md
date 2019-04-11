---
title: Get androidCompliancePolicy
description: Чтение свойств и связей объекта androidCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a4ac196e391bd9464001afebb7189c003458e54
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805504"
---
# <a name="get-androidcompliancepolicy"></a><span data-ttu-id="9f243-103">Get androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9f243-103">Get androidCompliancePolicy</span></span>

> <span data-ttu-id="9f243-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f243-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f243-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f243-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f243-106">Чтение свойств и связей объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9f243-106">Read properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f243-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9f243-107">Prerequisites</span></span>
<span data-ttu-id="9f243-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f243-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f243-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f243-110">Permission type</span></span>|<span data-ttu-id="9f243-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f243-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f243-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f243-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f243-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f243-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9f243-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f243-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f243-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f243-115">Not supported.</span></span>|
|<span data-ttu-id="9f243-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f243-116">Application</span></span>|<span data-ttu-id="9f243-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f243-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f243-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f243-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f243-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9f243-119">Optional query parameters</span></span>
<span data-ttu-id="9f243-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9f243-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f243-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f243-121">Request headers</span></span>
|<span data-ttu-id="9f243-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f243-122">Header</span></span>|<span data-ttu-id="9f243-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9f243-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f243-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f243-124">Authorization</span></span>|<span data-ttu-id="9f243-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f243-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f243-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9f243-126">Accept</span></span>|<span data-ttu-id="9f243-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9f243-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f243-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f243-128">Request body</span></span>
<span data-ttu-id="9f243-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f243-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f243-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f243-130">Response</span></span>
<span data-ttu-id="9f243-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9f243-131">If successful, this method returns a `200 OK` response code and [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f243-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9f243-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f243-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f243-133">Request</span></span>
<span data-ttu-id="9f243-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f243-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="9f243-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f243-135">Response</span></span>
<span data-ttu-id="9f243-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f243-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1863

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
}
```





