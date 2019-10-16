---
title: Обновление объекта deviceCompliancePolicyAssignment
description: Обновление свойств объекта deviceCompliancePolicyAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b1c5774eb9e40e42005c65b2910098578d511e00
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534185"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="1caf7-103">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="1caf7-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="1caf7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1caf7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1caf7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1caf7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1caf7-106">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1caf7-106">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1caf7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1caf7-107">Prerequisites</span></span>
<span data-ttu-id="1caf7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1caf7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1caf7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1caf7-110">Permission type</span></span>|<span data-ttu-id="1caf7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1caf7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1caf7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1caf7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1caf7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1caf7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1caf7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1caf7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1caf7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1caf7-115">Not supported.</span></span>|
|<span data-ttu-id="1caf7-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1caf7-116">Application</span></span>|<span data-ttu-id="1caf7-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1caf7-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1caf7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1caf7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1caf7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1caf7-119">Request headers</span></span>
|<span data-ttu-id="1caf7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1caf7-120">Header</span></span>|<span data-ttu-id="1caf7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1caf7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1caf7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1caf7-122">Authorization</span></span>|<span data-ttu-id="1caf7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1caf7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1caf7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1caf7-124">Accept</span></span>|<span data-ttu-id="1caf7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1caf7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1caf7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1caf7-126">Request body</span></span>
<span data-ttu-id="1caf7-127">В тексте запроса добавьте представление объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1caf7-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="1caf7-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1caf7-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="1caf7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1caf7-129">Property</span></span>|<span data-ttu-id="1caf7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1caf7-130">Type</span></span>|<span data-ttu-id="1caf7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1caf7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1caf7-132">id</span><span class="sxs-lookup"><span data-stu-id="1caf7-132">id</span></span>|<span data-ttu-id="1caf7-133">String</span><span class="sxs-lookup"><span data-stu-id="1caf7-133">String</span></span>|<span data-ttu-id="1caf7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1caf7-134">Key of the entity.</span></span>|
|<span data-ttu-id="1caf7-135">target</span><span class="sxs-lookup"><span data-stu-id="1caf7-135">target</span></span>|[<span data-ttu-id="1caf7-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1caf7-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1caf7-137">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="1caf7-137">Target for the compliance policy assignment.</span></span>|
|<span data-ttu-id="1caf7-138">source</span><span class="sxs-lookup"><span data-stu-id="1caf7-138">source</span></span>|[<span data-ttu-id="1caf7-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="1caf7-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="1caf7-140">Источник назначения для политики соответствия требованиям устройств, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="1caf7-140">The assignment source for the device compliance policy, direct or parcel/policySet.</span></span> <span data-ttu-id="1caf7-141">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="1caf7-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="1caf7-142">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="1caf7-142">sourceId</span></span>|<span data-ttu-id="1caf7-143">String</span><span class="sxs-lookup"><span data-stu-id="1caf7-143">String</span></span>|<span data-ttu-id="1caf7-144">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="1caf7-144">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="1caf7-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="1caf7-145">Response</span></span>
<span data-ttu-id="1caf7-146">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1caf7-146">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1caf7-147">Пример</span><span class="sxs-lookup"><span data-stu-id="1caf7-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="1caf7-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="1caf7-148">Request</span></span>
<span data-ttu-id="1caf7-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1caf7-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1caf7-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="1caf7-150">Response</span></span>
<span data-ttu-id="1caf7-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1caf7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






