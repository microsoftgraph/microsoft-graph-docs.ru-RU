---
title: Создание объекта deviceCompliancePolicyAssignment
description: Создание объекта deviceCompliancePolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a22aa098d351471c2ddf3725250119ded077b27f
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793047"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="b673d-103">Создание объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="b673d-103">Create deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="b673d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b673d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b673d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b673d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b673d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b673d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b673d-107">Создание объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b673d-107">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b673d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b673d-108">Prerequisites</span></span>
<span data-ttu-id="b673d-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b673d-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b673d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b673d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b673d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b673d-111">Permission type</span></span>|<span data-ttu-id="b673d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b673d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b673d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b673d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b673d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b673d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b673d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b673d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b673d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b673d-116">Not supported.</span></span>|
|<span data-ttu-id="b673d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b673d-117">Application</span></span>|<span data-ttu-id="b673d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b673d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b673d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b673d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b673d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b673d-120">Request headers</span></span>
|<span data-ttu-id="b673d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b673d-121">Header</span></span>|<span data-ttu-id="b673d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b673d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b673d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b673d-123">Authorization</span></span>|<span data-ttu-id="b673d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b673d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b673d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b673d-125">Accept</span></span>|<span data-ttu-id="b673d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b673d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b673d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b673d-127">Request body</span></span>
<span data-ttu-id="b673d-128">В тексте запроса добавьте представление объекта deviceCompliancePolicyAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b673d-128">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="b673d-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="b673d-129">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="b673d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b673d-130">Property</span></span>|<span data-ttu-id="b673d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b673d-131">Type</span></span>|<span data-ttu-id="b673d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b673d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b673d-133">id</span><span class="sxs-lookup"><span data-stu-id="b673d-133">id</span></span>|<span data-ttu-id="b673d-134">String</span><span class="sxs-lookup"><span data-stu-id="b673d-134">String</span></span>|<span data-ttu-id="b673d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b673d-135">Key of the entity.</span></span>|
|<span data-ttu-id="b673d-136">target</span><span class="sxs-lookup"><span data-stu-id="b673d-136">target</span></span>|[<span data-ttu-id="b673d-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b673d-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b673d-138">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="b673d-138">Target for the compliance policy assignment.</span></span>|
|<span data-ttu-id="b673d-139">source</span><span class="sxs-lookup"><span data-stu-id="b673d-139">source</span></span>|[<span data-ttu-id="b673d-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="b673d-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="b673d-141">Источник назначения для политики соответствия требованиям устройств, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="b673d-141">The assignment source for the device compliance policy, direct or parcel/policySet.</span></span> <span data-ttu-id="b673d-142">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="b673d-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="b673d-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="b673d-143">sourceId</span></span>|<span data-ttu-id="b673d-144">String</span><span class="sxs-lookup"><span data-stu-id="b673d-144">String</span></span>|<span data-ttu-id="b673d-145">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="b673d-145">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="b673d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b673d-146">Response</span></span>
<span data-ttu-id="b673d-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b673d-147">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b673d-148">Пример</span><span class="sxs-lookup"><span data-stu-id="b673d-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="b673d-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="b673d-149">Request</span></span>
<span data-ttu-id="b673d-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b673d-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
Content-type: application/json
Content-length: 388

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="b673d-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="b673d-151">Response</span></span>
<span data-ttu-id="b673d-152">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="b673d-152">Here is an example of the response.</span></span> <span data-ttu-id="b673d-153">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b673d-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b673d-154">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b673d-154">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 437

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
```



