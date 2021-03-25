---
title: Перечисление объектов windows81CompliancePolicy
description: Список свойств и связей объектов windows81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8ef7e66774a763fb71f6edb34c9601a034d813f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154947"
---
# <a name="list-windows81compliancepolicies"></a><span data-ttu-id="24487-103">Перечисление объектов windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="24487-103">List windows81CompliancePolicies</span></span>

<span data-ttu-id="24487-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24487-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24487-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24487-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24487-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24487-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24487-107">Список свойств и связей объектов [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24487-107">List properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24487-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="24487-108">Prerequisites</span></span>
<span data-ttu-id="24487-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24487-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24487-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24487-111">Permission type</span></span>|<span data-ttu-id="24487-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24487-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24487-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24487-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24487-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24487-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24487-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24487-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24487-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24487-116">Not supported.</span></span>|
|<span data-ttu-id="24487-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="24487-117">Application</span></span>|<span data-ttu-id="24487-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24487-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24487-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24487-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="24487-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="24487-120">Request headers</span></span>
|<span data-ttu-id="24487-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24487-121">Header</span></span>|<span data-ttu-id="24487-122">Значение</span><span class="sxs-lookup"><span data-stu-id="24487-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24487-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="24487-123">Authorization</span></span>|<span data-ttu-id="24487-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24487-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24487-125">Accept</span><span class="sxs-lookup"><span data-stu-id="24487-125">Accept</span></span>|<span data-ttu-id="24487-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24487-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24487-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24487-127">Request body</span></span>
<span data-ttu-id="24487-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24487-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24487-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="24487-129">Response</span></span>
<span data-ttu-id="24487-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24487-130">If successful, this method returns a `200 OK` response code and a collection of [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24487-131">Пример</span><span class="sxs-lookup"><span data-stu-id="24487-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="24487-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="24487-132">Request</span></span>
<span data-ttu-id="24487-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24487-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="24487-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="24487-134">Response</span></span>
<span data-ttu-id="24487-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24487-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 953

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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




