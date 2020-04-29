---
title: Обновление объекта deviceCompliancePolicyAssignment
description: Обновление свойств объекта deviceCompliancePolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2cd2895b83eca1ab8ce99c026ef8c02ce8e2ccde
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399965"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="4f824-103">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="4f824-103">Update deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="4f824-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f824-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f824-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f824-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f824-106">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4f824-106">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f824-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4f824-107">Prerequisites</span></span>
<span data-ttu-id="4f824-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f824-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f824-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f824-110">Permission type</span></span>|<span data-ttu-id="4f824-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f824-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f824-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f824-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f824-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f824-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f824-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f824-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f824-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f824-115">Not supported.</span></span>|
|<span data-ttu-id="4f824-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f824-116">Application</span></span>|<span data-ttu-id="4f824-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f824-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f824-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f824-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4f824-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4f824-119">Request headers</span></span>
|<span data-ttu-id="4f824-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f824-120">Header</span></span>|<span data-ttu-id="4f824-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4f824-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f824-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f824-122">Authorization</span></span>|<span data-ttu-id="4f824-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f824-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f824-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4f824-124">Accept</span></span>|<span data-ttu-id="4f824-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f824-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f824-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4f824-126">Request body</span></span>
<span data-ttu-id="4f824-127">В тексте запроса добавьте представление объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f824-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="4f824-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4f824-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="4f824-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f824-129">Property</span></span>|<span data-ttu-id="4f824-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4f824-130">Type</span></span>|<span data-ttu-id="4f824-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4f824-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f824-132">id</span><span class="sxs-lookup"><span data-stu-id="4f824-132">id</span></span>|<span data-ttu-id="4f824-133">String</span><span class="sxs-lookup"><span data-stu-id="4f824-133">String</span></span>|<span data-ttu-id="4f824-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4f824-134">Key of the entity.</span></span>|
|<span data-ttu-id="4f824-135">target</span><span class="sxs-lookup"><span data-stu-id="4f824-135">target</span></span>|[<span data-ttu-id="4f824-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4f824-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4f824-137">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="4f824-137">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="4f824-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f824-138">Response</span></span>
<span data-ttu-id="4f824-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4f824-139">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f824-140">Пример</span><span class="sxs-lookup"><span data-stu-id="4f824-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f824-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f824-141">Request</span></span>
<span data-ttu-id="4f824-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f824-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="4f824-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f824-143">Response</span></span>
<span data-ttu-id="4f824-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f824-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```






