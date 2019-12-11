---
title: Обновление объекта deviceCompliancePolicyAssignment
description: Обновление свойств объекта deviceCompliancePolicyAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d69d05c9135e57e798d028a9e785747d015d0db5
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949674"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="5442d-103">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="5442d-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="5442d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5442d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5442d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5442d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5442d-106">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5442d-106">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5442d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5442d-107">Prerequisites</span></span>
<span data-ttu-id="5442d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5442d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5442d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5442d-110">Permission type</span></span>|<span data-ttu-id="5442d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5442d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5442d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5442d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5442d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5442d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5442d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5442d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5442d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5442d-115">Not supported.</span></span>|
|<span data-ttu-id="5442d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5442d-116">Application</span></span>|<span data-ttu-id="5442d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5442d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5442d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5442d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5442d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5442d-119">Request headers</span></span>
|<span data-ttu-id="5442d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5442d-120">Header</span></span>|<span data-ttu-id="5442d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5442d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5442d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5442d-122">Authorization</span></span>|<span data-ttu-id="5442d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5442d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5442d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5442d-124">Accept</span></span>|<span data-ttu-id="5442d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5442d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5442d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5442d-126">Request body</span></span>
<span data-ttu-id="5442d-127">В тексте запроса добавьте представление объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5442d-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="5442d-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5442d-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="5442d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5442d-129">Property</span></span>|<span data-ttu-id="5442d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5442d-130">Type</span></span>|<span data-ttu-id="5442d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5442d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5442d-132">id</span><span class="sxs-lookup"><span data-stu-id="5442d-132">id</span></span>|<span data-ttu-id="5442d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5442d-133">String</span></span>|<span data-ttu-id="5442d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5442d-134">Key of the entity.</span></span>|
|<span data-ttu-id="5442d-135">target</span><span class="sxs-lookup"><span data-stu-id="5442d-135">target</span></span>|[<span data-ttu-id="5442d-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5442d-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5442d-137">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="5442d-137">Target for the compliance policy assignment.</span></span>|
|<span data-ttu-id="5442d-138">source</span><span class="sxs-lookup"><span data-stu-id="5442d-138">source</span></span>|[<span data-ttu-id="5442d-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="5442d-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="5442d-140">Источник назначения для политики соответствия требованиям устройств, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="5442d-140">The assignment source for the device compliance policy, direct or parcel/policySet.</span></span> <span data-ttu-id="5442d-141">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="5442d-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="5442d-142">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="5442d-142">sourceId</span></span>|<span data-ttu-id="5442d-143">Строка</span><span class="sxs-lookup"><span data-stu-id="5442d-143">String</span></span>|<span data-ttu-id="5442d-144">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="5442d-144">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="5442d-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="5442d-145">Response</span></span>
<span data-ttu-id="5442d-146">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5442d-146">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5442d-147">Пример</span><span class="sxs-lookup"><span data-stu-id="5442d-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="5442d-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="5442d-148">Request</span></span>
<span data-ttu-id="5442d-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5442d-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 233

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="5442d-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="5442d-150">Response</span></span>
<span data-ttu-id="5442d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5442d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 282

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```





