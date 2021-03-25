---
title: Обновление объекта deviceCompliancePolicyAssignment
description: Обновление свойств объекта deviceCompliancePolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5050253f407b2a251c37146cc50cec19450828b2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155458"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="ca4e3-103">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="ca4e3-103">Update deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="ca4e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca4e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca4e3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca4e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca4e3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca4e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca4e3-107">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ca4e3-107">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca4e3-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ca4e3-108">Prerequisites</span></span>
<span data-ttu-id="ca4e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca4e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca4e3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca4e3-111">Permission type</span></span>|<span data-ttu-id="ca4e3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca4e3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca4e3-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca4e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca4e3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca4e3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca4e3-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca4e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca4e3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca4e3-116">Not supported.</span></span>|
|<span data-ttu-id="ca4e3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ca4e3-117">Application</span></span>|<span data-ttu-id="ca4e3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca4e3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca4e3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca4e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ca4e3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ca4e3-120">Request headers</span></span>
|<span data-ttu-id="ca4e3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca4e3-121">Header</span></span>|<span data-ttu-id="ca4e3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ca4e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca4e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca4e3-123">Authorization</span></span>|<span data-ttu-id="ca4e3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca4e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca4e3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ca4e3-125">Accept</span></span>|<span data-ttu-id="ca4e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca4e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca4e3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca4e3-127">Request body</span></span>
<span data-ttu-id="ca4e3-128">В тексте запроса добавьте представление объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca4e3-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="ca4e3-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ca4e3-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="ca4e3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca4e3-130">Property</span></span>|<span data-ttu-id="ca4e3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ca4e3-131">Type</span></span>|<span data-ttu-id="ca4e3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ca4e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca4e3-133">id</span><span class="sxs-lookup"><span data-stu-id="ca4e3-133">id</span></span>|<span data-ttu-id="ca4e3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ca4e3-134">String</span></span>|<span data-ttu-id="ca4e3-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ca4e3-135">Key of the entity.</span></span>|
|<span data-ttu-id="ca4e3-136">target</span><span class="sxs-lookup"><span data-stu-id="ca4e3-136">target</span></span>|[<span data-ttu-id="ca4e3-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ca4e3-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ca4e3-138">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="ca4e3-138">Target for the compliance policy assignment.</span></span>|
|<span data-ttu-id="ca4e3-139">source</span><span class="sxs-lookup"><span data-stu-id="ca4e3-139">source</span></span>|[<span data-ttu-id="ca4e3-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="ca4e3-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="ca4e3-141">Источник назначения для политики соответствия требованиям устройств, прямой или пакетной или политикиSet.</span><span class="sxs-lookup"><span data-stu-id="ca4e3-141">The assignment source for the device compliance policy, direct or parcel/policySet.</span></span> <span data-ttu-id="ca4e3-142">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="ca4e3-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="ca4e3-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="ca4e3-143">sourceId</span></span>|<span data-ttu-id="ca4e3-144">Строка</span><span class="sxs-lookup"><span data-stu-id="ca4e3-144">String</span></span>|<span data-ttu-id="ca4e3-145">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="ca4e3-145">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="ca4e3-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca4e3-146">Response</span></span>
<span data-ttu-id="ca4e3-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca4e3-147">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca4e3-148">Пример</span><span class="sxs-lookup"><span data-stu-id="ca4e3-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca4e3-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca4e3-149">Request</span></span>
<span data-ttu-id="ca4e3-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca4e3-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 452

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="ca4e3-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca4e3-151">Response</span></span>
<span data-ttu-id="ca4e3-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca4e3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 501

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```




