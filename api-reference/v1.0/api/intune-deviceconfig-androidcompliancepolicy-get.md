---
title: Get androidCompliancePolicy
description: Чтение свойств и связей объекта androidCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: a3e9657e472a58a41e335321685c7a6cb7ac8bb9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354308"
---
# <a name="get-androidcompliancepolicy"></a><span data-ttu-id="c76da-103">Get androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c76da-103">Get androidCompliancePolicy</span></span>

> <span data-ttu-id="c76da-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c76da-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c76da-105">Чтение свойств и связей объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c76da-105">Read properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c76da-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c76da-106">Prerequisites</span></span>
<span data-ttu-id="c76da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c76da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c76da-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c76da-109">Permission type</span></span>|<span data-ttu-id="c76da-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c76da-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c76da-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c76da-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c76da-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c76da-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c76da-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c76da-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c76da-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c76da-114">Not supported.</span></span>|
|<span data-ttu-id="c76da-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c76da-115">Application</span></span>|<span data-ttu-id="c76da-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c76da-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c76da-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c76da-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c76da-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c76da-118">Optional query parameters</span></span>
<span data-ttu-id="c76da-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c76da-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c76da-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c76da-120">Request headers</span></span>
|<span data-ttu-id="c76da-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c76da-121">Header</span></span>|<span data-ttu-id="c76da-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c76da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c76da-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c76da-123">Authorization</span></span>|<span data-ttu-id="c76da-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c76da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c76da-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c76da-125">Accept</span></span>|<span data-ttu-id="c76da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c76da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c76da-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c76da-127">Request body</span></span>
<span data-ttu-id="c76da-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c76da-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c76da-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c76da-129">Response</span></span>
<span data-ttu-id="c76da-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c76da-130">If successful, this method returns a `200 OK` response code and [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c76da-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c76da-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c76da-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c76da-132">Request</span></span>
<span data-ttu-id="c76da-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c76da-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="c76da-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c76da-134">Response</span></span>
<span data-ttu-id="c76da-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c76da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1406

{
  "value": {
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
}
```



