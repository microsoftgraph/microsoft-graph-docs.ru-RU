---
title: Get androidCompliancePolicy
description: Чтение свойств и связей объекта androidCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20d84b161ededcdd40f53178fce91d0fe2771809
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020383"
---
# <a name="get-androidcompliancepolicy"></a><span data-ttu-id="d41f4-103">Get androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d41f4-103">Get androidCompliancePolicy</span></span>

> <span data-ttu-id="d41f4-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d41f4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d41f4-105">Чтение свойств и связей объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d41f4-105">Read properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d41f4-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d41f4-106">Prerequisites</span></span>
<span data-ttu-id="d41f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d41f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d41f4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d41f4-109">Permission type</span></span>|<span data-ttu-id="d41f4-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d41f4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d41f4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d41f4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d41f4-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d41f4-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d41f4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d41f4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d41f4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d41f4-114">Not supported.</span></span>|
|<span data-ttu-id="d41f4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d41f4-115">Application</span></span>|<span data-ttu-id="d41f4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d41f4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d41f4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d41f4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d41f4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d41f4-118">Optional query parameters</span></span>
<span data-ttu-id="d41f4-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d41f4-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d41f4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d41f4-120">Request headers</span></span>
|<span data-ttu-id="d41f4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d41f4-121">Header</span></span>|<span data-ttu-id="d41f4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d41f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d41f4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d41f4-123">Authorization</span></span>|<span data-ttu-id="d41f4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d41f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d41f4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d41f4-125">Accept</span></span>|<span data-ttu-id="d41f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d41f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d41f4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d41f4-127">Request body</span></span>
<span data-ttu-id="d41f4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d41f4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d41f4-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d41f4-129">Response</span></span>
<span data-ttu-id="d41f4-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d41f4-130">If successful, this method returns a `200 OK` response code and [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d41f4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d41f4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d41f4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d41f4-132">Request</span></span>
<span data-ttu-id="d41f4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d41f4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="d41f4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d41f4-134">Response</span></span>
<span data-ttu-id="d41f4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d41f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



