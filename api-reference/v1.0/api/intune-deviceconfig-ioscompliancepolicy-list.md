---
title: Перечисление объектов iosCompliancePolicy
description: Список свойств и связей объектов iosCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4557edfe695d5ba00cbb96dd9155e859b36b3438
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753876"
---
# <a name="list-ioscompliancepolicies"></a><span data-ttu-id="a87d9-103">Перечисление объектов iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a87d9-103">List iosCompliancePolicies</span></span>

<span data-ttu-id="a87d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a87d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a87d9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a87d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a87d9-106">Список свойств и связей объектов [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a87d9-106">List properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a87d9-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a87d9-107">Prerequisites</span></span>
<span data-ttu-id="a87d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a87d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a87d9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a87d9-110">Permission type</span></span>|<span data-ttu-id="a87d9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a87d9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a87d9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a87d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a87d9-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a87d9-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a87d9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a87d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a87d9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a87d9-115">Not supported.</span></span>|
|<span data-ttu-id="a87d9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a87d9-116">Application</span></span>|<span data-ttu-id="a87d9-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a87d9-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a87d9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a87d9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="a87d9-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a87d9-119">Request headers</span></span>
|<span data-ttu-id="a87d9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a87d9-120">Header</span></span>|<span data-ttu-id="a87d9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a87d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a87d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a87d9-122">Authorization</span></span>|<span data-ttu-id="a87d9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a87d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a87d9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a87d9-124">Accept</span></span>|<span data-ttu-id="a87d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a87d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a87d9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a87d9-126">Request body</span></span>
<span data-ttu-id="a87d9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a87d9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a87d9-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a87d9-128">Response</span></span>
<span data-ttu-id="a87d9-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a87d9-129">If successful, this method returns a `200 OK` response code and a collection of [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a87d9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a87d9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a87d9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a87d9-131">Request</span></span>
<span data-ttu-id="a87d9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a87d9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="a87d9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a87d9-133">Response</span></span>
<span data-ttu-id="a87d9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a87d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1034

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCompliancePolicy",
      "id": "4f501351-1351-4f50-5113-504f5113504f",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passcodeBlockSimple": true,
      "passcodeExpirationDays": 6,
      "passcodeMinimumLength": 5,
      "passcodeMinutesOfInactivityBeforeLock": 5,
      "passcodePreviousPasscodeBlockCount": 2,
      "passcodeMinimumCharacterSetCount": 0,
      "passcodeRequiredType": "alphanumeric",
      "passcodeRequired": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "securityBlockJailbrokenDevices": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "managedEmailProfileRequired": true
    }
  ]
}
```




