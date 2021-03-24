---
title: Get androidDeviceOwnerCompliancePolicy
description: Чтение свойств и связей объекта androidDeviceOwnerCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f549e89d381eab6c1e911e23c17896be77f789d8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128497"
---
# <a name="get-androiddeviceownercompliancepolicy"></a><span data-ttu-id="bb4ca-103">Get androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="bb4ca-103">Get androidDeviceOwnerCompliancePolicy</span></span>

<span data-ttu-id="bb4ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb4ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb4ca-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb4ca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb4ca-107">Чтение свойств и связей [объекта androidDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bb4ca-107">Read properties and relationships of the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb4ca-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bb4ca-108">Prerequisites</span></span>
<span data-ttu-id="bb4ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb4ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb4ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb4ca-111">Permission type</span></span>|<span data-ttu-id="bb4ca-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb4ca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb4ca-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb4ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb4ca-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb4ca-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb4ca-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb4ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb4ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-116">Not supported.</span></span>|
|<span data-ttu-id="bb4ca-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bb4ca-117">Application</span></span>|<span data-ttu-id="bb4ca-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb4ca-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb4ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb4ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb4ca-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bb4ca-120">Optional query parameters</span></span>
<span data-ttu-id="bb4ca-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb4ca-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb4ca-122">Request headers</span></span>
|<span data-ttu-id="bb4ca-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb4ca-123">Header</span></span>|<span data-ttu-id="bb4ca-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bb4ca-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb4ca-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb4ca-125">Authorization</span></span>|<span data-ttu-id="bb4ca-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb4ca-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bb4ca-127">Accept</span></span>|<span data-ttu-id="bb4ca-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bb4ca-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb4ca-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb4ca-129">Request body</span></span>
<span data-ttu-id="bb4ca-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb4ca-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb4ca-131">Response</span></span>
<span data-ttu-id="bb4ca-132">В случае успешного использования этот метод возвращает код отклика и `200 OK` [объект AndroidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-132">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb4ca-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bb4ca-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb4ca-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb4ca-134">Request</span></span>
<span data-ttu-id="bb4ca-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="bb4ca-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb4ca-136">Response</span></span>
<span data-ttu-id="bb4ca-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1476

{
  "value": {
    "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "be2464b4-64b4-be24-b464-24beb46424be",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "advancedThreatProtectionRequiredSecurityLevel": "secured",
    "securityRequireSafetyNetAttestationBasicIntegrity": true,
    "securityRequireSafetyNetAttestationCertifiedDevice": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
    "passwordRequired": true,
    "passwordMinimumLength": 5,
    "passwordMinimumLetterCharacters": 15,
    "passwordMinimumLowerCaseCharacters": 2,
    "passwordMinimumNonLetterCharacters": 2,
    "passwordMinimumNumericCharacters": 0,
    "passwordMinimumSymbolCharacters": 15,
    "passwordMinimumUpperCaseCharacters": 2,
    "passwordRequiredType": "required",
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordExpirationDays": 6,
    "passwordPreviousPasswordCountToBlock": 4,
    "storageRequireEncryption": true
  }
}
```




