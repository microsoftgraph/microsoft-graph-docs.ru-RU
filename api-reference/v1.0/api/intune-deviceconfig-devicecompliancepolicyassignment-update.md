---
title: Обновление объекта deviceCompliancePolicyAssignment
description: Обновление свойств объекта deviceCompliancePolicyAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 083c74d87e22990f491ed087186b47e98de638fe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515037"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="2a6fc-103">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="2a6fc-103">Update deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="2a6fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a6fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a6fc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a6fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a6fc-106">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2a6fc-106">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a6fc-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2a6fc-107">Prerequisites</span></span>
<span data-ttu-id="2a6fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a6fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a6fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a6fc-110">Permission type</span></span>|<span data-ttu-id="2a6fc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a6fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a6fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a6fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a6fc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a6fc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2a6fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a6fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a6fc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a6fc-115">Not supported.</span></span>|
|<span data-ttu-id="2a6fc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a6fc-116">Application</span></span>|<span data-ttu-id="2a6fc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a6fc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a6fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a6fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2a6fc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2a6fc-119">Request headers</span></span>
|<span data-ttu-id="2a6fc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a6fc-120">Header</span></span>|<span data-ttu-id="2a6fc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2a6fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a6fc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a6fc-122">Authorization</span></span>|<span data-ttu-id="2a6fc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a6fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a6fc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2a6fc-124">Accept</span></span>|<span data-ttu-id="2a6fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a6fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a6fc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a6fc-126">Request body</span></span>
<span data-ttu-id="2a6fc-127">В тексте запроса добавьте представление объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a6fc-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="2a6fc-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2a6fc-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="2a6fc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a6fc-129">Property</span></span>|<span data-ttu-id="2a6fc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2a6fc-130">Type</span></span>|<span data-ttu-id="2a6fc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2a6fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a6fc-132">id</span><span class="sxs-lookup"><span data-stu-id="2a6fc-132">id</span></span>|<span data-ttu-id="2a6fc-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2a6fc-133">String</span></span>|<span data-ttu-id="2a6fc-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2a6fc-134">Key of the entity.</span></span>|
|<span data-ttu-id="2a6fc-135">target</span><span class="sxs-lookup"><span data-stu-id="2a6fc-135">target</span></span>|[<span data-ttu-id="2a6fc-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2a6fc-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2a6fc-137">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="2a6fc-137">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="2a6fc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a6fc-138">Response</span></span>
<span data-ttu-id="2a6fc-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2a6fc-139">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a6fc-140">Пример</span><span class="sxs-lookup"><span data-stu-id="2a6fc-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a6fc-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a6fc-141">Request</span></span>
<span data-ttu-id="2a6fc-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a6fc-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2a6fc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a6fc-143">Response</span></span>
<span data-ttu-id="2a6fc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a6fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




