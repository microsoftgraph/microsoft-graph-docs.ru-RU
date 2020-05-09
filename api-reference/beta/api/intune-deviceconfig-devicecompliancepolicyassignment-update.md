---
title: Обновление объекта deviceCompliancePolicyAssignment
description: Обновление свойств объекта deviceCompliancePolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0dbee404d4f2b6fb32dbe5f8a6c93f7238f2dd5c
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178677"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="ddffe-103">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="ddffe-103">Update deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="ddffe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddffe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ddffe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddffe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddffe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ddffe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddffe-107">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ddffe-107">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddffe-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ddffe-108">Prerequisites</span></span>
<span data-ttu-id="ddffe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddffe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddffe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddffe-111">Permission type</span></span>|<span data-ttu-id="ddffe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddffe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddffe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddffe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ddffe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddffe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ddffe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddffe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddffe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddffe-116">Not supported.</span></span>|
|<span data-ttu-id="ddffe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddffe-117">Application</span></span>|<span data-ttu-id="ddffe-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddffe-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddffe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddffe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ddffe-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ddffe-120">Request headers</span></span>
|<span data-ttu-id="ddffe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ddffe-121">Header</span></span>|<span data-ttu-id="ddffe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ddffe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddffe-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ddffe-123">Authorization</span></span>|<span data-ttu-id="ddffe-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddffe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddffe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ddffe-125">Accept</span></span>|<span data-ttu-id="ddffe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ddffe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddffe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddffe-127">Request body</span></span>
<span data-ttu-id="ddffe-128">В тексте запроса добавьте представление объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddffe-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="ddffe-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ddffe-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="ddffe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddffe-130">Property</span></span>|<span data-ttu-id="ddffe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ddffe-131">Type</span></span>|<span data-ttu-id="ddffe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ddffe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddffe-133">id</span><span class="sxs-lookup"><span data-stu-id="ddffe-133">id</span></span>|<span data-ttu-id="ddffe-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ddffe-134">String</span></span>|<span data-ttu-id="ddffe-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ddffe-135">Key of the entity.</span></span>|
|<span data-ttu-id="ddffe-136">target</span><span class="sxs-lookup"><span data-stu-id="ddffe-136">target</span></span>|[<span data-ttu-id="ddffe-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ddffe-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ddffe-138">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="ddffe-138">Target for the compliance policy assignment.</span></span>|
|<span data-ttu-id="ddffe-139">source</span><span class="sxs-lookup"><span data-stu-id="ddffe-139">source</span></span>|[<span data-ttu-id="ddffe-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="ddffe-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="ddffe-141">Источник назначения для политики соответствия требованиям устройств, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="ddffe-141">The assignment source for the device compliance policy, direct or parcel/policySet.</span></span> <span data-ttu-id="ddffe-142">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="ddffe-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="ddffe-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="ddffe-143">sourceId</span></span>|<span data-ttu-id="ddffe-144">Строка</span><span class="sxs-lookup"><span data-stu-id="ddffe-144">String</span></span>|<span data-ttu-id="ddffe-145">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="ddffe-145">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="ddffe-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddffe-146">Response</span></span>
<span data-ttu-id="ddffe-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ddffe-147">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddffe-148">Пример</span><span class="sxs-lookup"><span data-stu-id="ddffe-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddffe-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddffe-149">Request</span></span>
<span data-ttu-id="ddffe-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddffe-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 221

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="ddffe-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddffe-151">Response</span></span>
<span data-ttu-id="ddffe-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ddffe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



