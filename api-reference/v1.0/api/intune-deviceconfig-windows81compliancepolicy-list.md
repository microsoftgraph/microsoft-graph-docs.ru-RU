---
title: Перечисление объектов windows81CompliancePolicy
description: Список свойств и связей объектов windows81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f593c3d8a9a54bb1afe0593e9cf38d0c6eaad972
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753820"
---
# <a name="list-windows81compliancepolicies"></a><span data-ttu-id="f833b-103">Перечисление объектов windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f833b-103">List windows81CompliancePolicies</span></span>

<span data-ttu-id="f833b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f833b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f833b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f833b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f833b-106">Список свойств и связей объектов [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f833b-106">List properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f833b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f833b-107">Prerequisites</span></span>
<span data-ttu-id="f833b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f833b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f833b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f833b-110">Permission type</span></span>|<span data-ttu-id="f833b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f833b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f833b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f833b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f833b-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f833b-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f833b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f833b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f833b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f833b-115">Not supported.</span></span>|
|<span data-ttu-id="f833b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f833b-116">Application</span></span>|<span data-ttu-id="f833b-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f833b-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f833b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f833b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f833b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f833b-119">Request headers</span></span>
|<span data-ttu-id="f833b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f833b-120">Header</span></span>|<span data-ttu-id="f833b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f833b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f833b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f833b-122">Authorization</span></span>|<span data-ttu-id="f833b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f833b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f833b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f833b-124">Accept</span></span>|<span data-ttu-id="f833b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f833b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f833b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f833b-126">Request body</span></span>
<span data-ttu-id="f833b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f833b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f833b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f833b-128">Response</span></span>
<span data-ttu-id="f833b-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f833b-129">If successful, this method returns a `200 OK` response code and a collection of [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f833b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f833b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f833b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f833b-131">Request</span></span>
<span data-ttu-id="f833b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f833b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="f833b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f833b-133">Response</span></span>
<span data-ttu-id="f833b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f833b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 879

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
      "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "storageRequireEncryption": true
    }
  ]
}
```




