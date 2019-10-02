---
title: Получение androidWorkProfileCompliancePolicy
description: Чтение свойств и связей объекта androidWorkProfileCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ff8a98468bebc2ea5437d0347faa682de3099d02
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354450"
---
# <a name="get-androidworkprofilecompliancepolicy"></a><span data-ttu-id="ff358-103">Получение androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ff358-103">Get androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="ff358-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff358-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff358-105">Чтение свойств и связей объекта [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ff358-105">Read properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff358-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ff358-106">Prerequisites</span></span>
<span data-ttu-id="ff358-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff358-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff358-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff358-109">Permission type</span></span>|<span data-ttu-id="ff358-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff358-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff358-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff358-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ff358-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff358-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ff358-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff358-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff358-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff358-114">Not supported.</span></span>|
|<span data-ttu-id="ff358-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff358-115">Application</span></span>|<span data-ttu-id="ff358-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff358-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff358-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff358-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff358-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ff358-118">Optional query parameters</span></span>
<span data-ttu-id="ff358-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ff358-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff358-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff358-120">Request headers</span></span>
|<span data-ttu-id="ff358-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff358-121">Header</span></span>|<span data-ttu-id="ff358-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ff358-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff358-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff358-123">Authorization</span></span>|<span data-ttu-id="ff358-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff358-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff358-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ff358-125">Accept</span></span>|<span data-ttu-id="ff358-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff358-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff358-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff358-127">Request body</span></span>
<span data-ttu-id="ff358-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff358-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff358-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff358-129">Response</span></span>
<span data-ttu-id="ff358-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ff358-130">If successful, this method returns a `200 OK` response code and [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff358-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ff358-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff358-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff358-132">Request</span></span>
<span data-ttu-id="ff358-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff358-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="ff358-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff358-134">Response</span></span>
<span data-ttu-id="ff358-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff358-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1417

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
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




