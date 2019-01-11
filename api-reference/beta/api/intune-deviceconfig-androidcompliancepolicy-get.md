---
title: Get androidCompliancePolicy
description: Чтение свойств и связей объекта androidCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dd8f0e2ee5505347d8aa661dc32a1463754314e1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878563"
---
# <a name="get-androidcompliancepolicy"></a><span data-ttu-id="4cfed-103">Get androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4cfed-103">Get androidCompliancePolicy</span></span>

> <span data-ttu-id="4cfed-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4cfed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4cfed-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cfed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4cfed-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4cfed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4cfed-107">Чтение свойств и связей объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4cfed-107">Read properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4cfed-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4cfed-108">Prerequisites</span></span>
<span data-ttu-id="4cfed-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cfed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cfed-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cfed-111">Permission type</span></span>|<span data-ttu-id="4cfed-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cfed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cfed-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cfed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4cfed-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cfed-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4cfed-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cfed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cfed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cfed-116">Not supported.</span></span>|
|<span data-ttu-id="4cfed-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cfed-117">Application</span></span>|<span data-ttu-id="4cfed-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cfed-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cfed-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cfed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4cfed-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4cfed-120">Optional query parameters</span></span>
<span data-ttu-id="4cfed-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4cfed-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4cfed-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4cfed-122">Request headers</span></span>
|<span data-ttu-id="4cfed-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4cfed-123">Header</span></span>|<span data-ttu-id="4cfed-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4cfed-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cfed-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cfed-125">Authorization</span></span>|<span data-ttu-id="4cfed-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4cfed-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cfed-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4cfed-127">Accept</span></span>|<span data-ttu-id="4cfed-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4cfed-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cfed-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4cfed-129">Request body</span></span>
<span data-ttu-id="4cfed-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4cfed-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cfed-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="4cfed-131">Response</span></span>
<span data-ttu-id="4cfed-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4cfed-132">If successful, this method returns a `200 OK` response code and [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cfed-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4cfed-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="4cfed-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cfed-134">Request</span></span>
<span data-ttu-id="4cfed-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cfed-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="4cfed-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4cfed-136">Response</span></span>
<span data-ttu-id="4cfed-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4cfed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1806

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





