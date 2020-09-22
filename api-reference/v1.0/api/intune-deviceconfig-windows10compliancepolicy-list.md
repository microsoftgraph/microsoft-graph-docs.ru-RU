---
title: Перечисление объектов windows10CompliancePolicy
description: Список свойств и связей объектов windows10CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9364dc5fe672912e28b3c3327afdea09939c5c17
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021016"
---
# <a name="list-windows10compliancepolicies"></a><span data-ttu-id="4f73e-103">Перечисление объектов windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4f73e-103">List windows10CompliancePolicies</span></span>

<span data-ttu-id="4f73e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f73e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f73e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f73e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f73e-106">Список свойств и связей объектов [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4f73e-106">List properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f73e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4f73e-107">Prerequisites</span></span>
<span data-ttu-id="4f73e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f73e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f73e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f73e-110">Permission type</span></span>|<span data-ttu-id="4f73e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f73e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f73e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f73e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f73e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f73e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4f73e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f73e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f73e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f73e-115">Not supported.</span></span>|
|<span data-ttu-id="4f73e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f73e-116">Application</span></span>|<span data-ttu-id="4f73e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f73e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f73e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f73e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="4f73e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4f73e-119">Request headers</span></span>
|<span data-ttu-id="4f73e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f73e-120">Header</span></span>|<span data-ttu-id="4f73e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4f73e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f73e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f73e-122">Authorization</span></span>|<span data-ttu-id="4f73e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f73e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f73e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4f73e-124">Accept</span></span>|<span data-ttu-id="4f73e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f73e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f73e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4f73e-126">Request body</span></span>
<span data-ttu-id="4f73e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f73e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f73e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f73e-128">Response</span></span>
<span data-ttu-id="4f73e-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4f73e-129">If successful, this method returns a `200 OK` response code and a collection of [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f73e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4f73e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f73e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f73e-131">Request</span></span>
<span data-ttu-id="4f73e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f73e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="4f73e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f73e-133">Response</span></span>
<span data-ttu-id="4f73e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f73e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1263

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
      "id": "2919ae62-ae62-2919-62ae-192962ae1929",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordRequiredToUnlockFromIdle": true,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "requireHealthyDeviceReport": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
      "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
      "earlyLaunchAntiMalwareDriverEnabled": true,
      "bitLockerEnabled": true,
      "secureBootEnabled": true,
      "codeIntegrityEnabled": true,
      "storageRequireEncryption": true
    }
  ]
}
```









