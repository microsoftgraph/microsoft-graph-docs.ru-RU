---
title: Создание объекта deviceCompliancePolicyAssignment
description: Создание объекта deviceCompliancePolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8eb1eb9b2d88ce211c0c452e054d2c02924f54eb
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178698"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="4c2d5-103">Создание объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="4c2d5-103">Create deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="4c2d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c2d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c2d5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c2d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c2d5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c2d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c2d5-107">Создание объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4c2d5-107">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c2d5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4c2d5-108">Prerequisites</span></span>
<span data-ttu-id="4c2d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c2d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c2d5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c2d5-111">Permission type</span></span>|<span data-ttu-id="4c2d5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c2d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c2d5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c2d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c2d5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c2d5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c2d5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c2d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c2d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c2d5-116">Not supported.</span></span>|
|<span data-ttu-id="4c2d5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c2d5-117">Application</span></span>|<span data-ttu-id="4c2d5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c2d5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c2d5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c2d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4c2d5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4c2d5-120">Request headers</span></span>
|<span data-ttu-id="4c2d5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c2d5-121">Header</span></span>|<span data-ttu-id="4c2d5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4c2d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c2d5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c2d5-123">Authorization</span></span>|<span data-ttu-id="4c2d5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c2d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c2d5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4c2d5-125">Accept</span></span>|<span data-ttu-id="4c2d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c2d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c2d5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c2d5-127">Request body</span></span>
<span data-ttu-id="4c2d5-128">В тексте запроса добавьте представление объекта deviceCompliancePolicyAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c2d5-128">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="4c2d5-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="4c2d5-129">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="4c2d5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c2d5-130">Property</span></span>|<span data-ttu-id="4c2d5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4c2d5-131">Type</span></span>|<span data-ttu-id="4c2d5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4c2d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c2d5-133">id</span><span class="sxs-lookup"><span data-stu-id="4c2d5-133">id</span></span>|<span data-ttu-id="4c2d5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4c2d5-134">String</span></span>|<span data-ttu-id="4c2d5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4c2d5-135">Key of the entity.</span></span>|
|<span data-ttu-id="4c2d5-136">target</span><span class="sxs-lookup"><span data-stu-id="4c2d5-136">target</span></span>|[<span data-ttu-id="4c2d5-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4c2d5-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4c2d5-138">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="4c2d5-138">Target for the compliance policy assignment.</span></span>|
|<span data-ttu-id="4c2d5-139">source</span><span class="sxs-lookup"><span data-stu-id="4c2d5-139">source</span></span>|[<span data-ttu-id="4c2d5-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="4c2d5-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="4c2d5-141">Источник назначения для политики соответствия требованиям устройств, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="4c2d5-141">The assignment source for the device compliance policy, direct or parcel/policySet.</span></span> <span data-ttu-id="4c2d5-142">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="4c2d5-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="4c2d5-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="4c2d5-143">sourceId</span></span>|<span data-ttu-id="4c2d5-144">Строка</span><span class="sxs-lookup"><span data-stu-id="4c2d5-144">String</span></span>|<span data-ttu-id="4c2d5-145">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="4c2d5-145">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="4c2d5-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c2d5-146">Response</span></span>
<span data-ttu-id="4c2d5-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c2d5-147">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c2d5-148">Пример</span><span class="sxs-lookup"><span data-stu-id="4c2d5-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c2d5-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c2d5-149">Request</span></span>
<span data-ttu-id="4c2d5-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c2d5-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
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

### <a name="response"></a><span data-ttu-id="4c2d5-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c2d5-151">Response</span></span>
<span data-ttu-id="4c2d5-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c2d5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



