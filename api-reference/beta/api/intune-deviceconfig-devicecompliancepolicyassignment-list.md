---
title: Перечисление объектов deviceCompliancePolicyAssignment
description: Список свойств и связей объектов deviceCompliancePolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1eca501ef89ddd3badb14ecd58e0f5c692a9c80c
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793033"
---
# <a name="list-devicecompliancepolicyassignments"></a><span data-ttu-id="c1916-103">Перечисление объектов deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="c1916-103">List deviceCompliancePolicyAssignments</span></span>

<span data-ttu-id="c1916-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1916-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1916-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1916-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1916-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1916-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1916-107">Список свойств и связей объектов [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c1916-107">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1916-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c1916-108">Prerequisites</span></span>
<span data-ttu-id="c1916-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c1916-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c1916-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1916-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1916-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1916-111">Permission type</span></span>|<span data-ttu-id="c1916-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1916-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1916-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1916-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1916-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1916-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c1916-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1916-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1916-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1916-116">Not supported.</span></span>|
|<span data-ttu-id="c1916-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1916-117">Application</span></span>|<span data-ttu-id="c1916-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1916-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1916-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1916-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c1916-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c1916-120">Request headers</span></span>
|<span data-ttu-id="c1916-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1916-121">Header</span></span>|<span data-ttu-id="c1916-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c1916-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1916-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1916-123">Authorization</span></span>|<span data-ttu-id="c1916-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1916-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1916-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c1916-125">Accept</span></span>|<span data-ttu-id="c1916-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1916-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1916-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c1916-127">Request body</span></span>
<span data-ttu-id="c1916-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c1916-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1916-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1916-129">Response</span></span>
<span data-ttu-id="c1916-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1916-130">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1916-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c1916-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1916-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1916-132">Request</span></span>
<span data-ttu-id="c1916-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1916-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="c1916-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1916-134">Response</span></span>
<span data-ttu-id="c1916-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="c1916-135">Here is an example of the response.</span></span> <span data-ttu-id="c1916-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="c1916-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c1916-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c1916-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 506

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```



