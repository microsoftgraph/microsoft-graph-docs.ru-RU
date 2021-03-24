---
title: Список androidDeviceOwnerCompliancePolicies
description: Список свойств и связей объектов AndroidDeviceOwnerCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 36fc236e827dc1a02d925a565614bd9f7819a07c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132851"
---
# <a name="list-androiddeviceownercompliancepolicies"></a><span data-ttu-id="8ef64-103">Список androidDeviceOwnerCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="8ef64-103">List androidDeviceOwnerCompliancePolicies</span></span>

<span data-ttu-id="8ef64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ef64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ef64-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ef64-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ef64-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ef64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ef64-107">Список свойств и связей [объектов AndroidDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8ef64-107">List properties and relationships of the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ef64-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8ef64-108">Prerequisites</span></span>
<span data-ttu-id="8ef64-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ef64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ef64-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ef64-111">Permission type</span></span>|<span data-ttu-id="8ef64-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ef64-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ef64-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ef64-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ef64-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ef64-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ef64-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ef64-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ef64-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ef64-116">Not supported.</span></span>|
|<span data-ttu-id="8ef64-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8ef64-117">Application</span></span>|<span data-ttu-id="8ef64-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ef64-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ef64-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ef64-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="8ef64-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8ef64-120">Request headers</span></span>
|<span data-ttu-id="8ef64-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ef64-121">Header</span></span>|<span data-ttu-id="8ef64-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8ef64-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ef64-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ef64-123">Authorization</span></span>|<span data-ttu-id="8ef64-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ef64-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ef64-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8ef64-125">Accept</span></span>|<span data-ttu-id="8ef64-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ef64-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ef64-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ef64-127">Request body</span></span>
<span data-ttu-id="8ef64-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ef64-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ef64-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ef64-129">Response</span></span>
<span data-ttu-id="8ef64-130">В случае успешного использования этот метод возвращает код отклика и коллекцию объектов `200 OK` [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8ef64-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ef64-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8ef64-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ef64-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ef64-132">Request</span></span>
<span data-ttu-id="8ef64-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ef64-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="8ef64-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ef64-134">Response</span></span>
<span data-ttu-id="8ef64-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ef64-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1552

{
  "value": [
    {
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
  ]
}
```




