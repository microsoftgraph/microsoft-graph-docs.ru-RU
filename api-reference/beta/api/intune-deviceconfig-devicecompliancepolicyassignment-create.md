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
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="7f1af-103">Создание объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="7f1af-103">Create deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="7f1af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f1af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f1af-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f1af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f1af-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f1af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f1af-107">Создание объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7f1af-107">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f1af-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7f1af-108">Prerequisites</span></span>
<span data-ttu-id="7f1af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f1af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f1af-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f1af-111">Permission type</span></span>|<span data-ttu-id="7f1af-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f1af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f1af-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f1af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f1af-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f1af-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f1af-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f1af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f1af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f1af-116">Not supported.</span></span>|
|<span data-ttu-id="7f1af-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f1af-117">Application</span></span>|<span data-ttu-id="7f1af-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f1af-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f1af-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f1af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7f1af-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7f1af-120">Request headers</span></span>
|<span data-ttu-id="7f1af-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f1af-121">Header</span></span>|<span data-ttu-id="7f1af-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7f1af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f1af-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f1af-123">Authorization</span></span>|<span data-ttu-id="7f1af-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f1af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f1af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f1af-125">Accept</span></span>|<span data-ttu-id="7f1af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f1af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f1af-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f1af-127">Request body</span></span>
<span data-ttu-id="7f1af-128">В тексте запроса добавьте представление объекта deviceCompliancePolicyAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f1af-128">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="7f1af-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="7f1af-129">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="7f1af-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f1af-130">Property</span></span>|<span data-ttu-id="7f1af-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7f1af-131">Type</span></span>|<span data-ttu-id="7f1af-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7f1af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f1af-133">id</span><span class="sxs-lookup"><span data-stu-id="7f1af-133">id</span></span>|<span data-ttu-id="7f1af-134">String</span><span class="sxs-lookup"><span data-stu-id="7f1af-134">String</span></span>|<span data-ttu-id="7f1af-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7f1af-135">Key of the entity.</span></span>|
|<span data-ttu-id="7f1af-136">target</span><span class="sxs-lookup"><span data-stu-id="7f1af-136">target</span></span>|[<span data-ttu-id="7f1af-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7f1af-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7f1af-138">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="7f1af-138">Target for the compliance policy assignment.</span></span>|
|<span data-ttu-id="7f1af-139">source</span><span class="sxs-lookup"><span data-stu-id="7f1af-139">source</span></span>|[<span data-ttu-id="7f1af-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="7f1af-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="7f1af-141">Источник назначения для политики соответствия требованиям устройств, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="7f1af-141">The assignment source for the device compliance policy, direct or parcel/policySet.</span></span> <span data-ttu-id="7f1af-142">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="7f1af-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="7f1af-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="7f1af-143">sourceId</span></span>|<span data-ttu-id="7f1af-144">String</span><span class="sxs-lookup"><span data-stu-id="7f1af-144">String</span></span>|<span data-ttu-id="7f1af-145">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="7f1af-145">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="7f1af-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f1af-146">Response</span></span>
<span data-ttu-id="7f1af-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f1af-147">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f1af-148">Пример</span><span class="sxs-lookup"><span data-stu-id="7f1af-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f1af-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f1af-149">Request</span></span>
<span data-ttu-id="7f1af-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f1af-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7f1af-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f1af-151">Response</span></span>
<span data-ttu-id="7f1af-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f1af-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



