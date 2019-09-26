---
title: Обновление объекта deviceCompliancePolicyAssignment
description: Обновление свойств объекта deviceCompliancePolicyAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 37f2c7047950f9de93d609e3549a3efe03f77419
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37168525"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="fa761-103">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="fa761-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="fa761-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa761-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa761-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa761-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa761-106">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fa761-106">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa761-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fa761-107">Prerequisites</span></span>
<span data-ttu-id="fa761-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa761-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa761-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa761-110">Permission type</span></span>|<span data-ttu-id="fa761-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa761-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa761-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa761-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa761-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa761-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fa761-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa761-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa761-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa761-115">Not supported.</span></span>|
|<span data-ttu-id="fa761-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa761-116">Application</span></span>|<span data-ttu-id="fa761-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa761-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa761-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa761-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="fa761-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa761-119">Request headers</span></span>
|<span data-ttu-id="fa761-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa761-120">Header</span></span>|<span data-ttu-id="fa761-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fa761-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa761-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa761-122">Authorization</span></span>|<span data-ttu-id="fa761-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa761-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa761-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fa761-124">Accept</span></span>|<span data-ttu-id="fa761-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa761-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa761-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa761-126">Request body</span></span>
<span data-ttu-id="fa761-127">В тексте запроса добавьте представление объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa761-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="fa761-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fa761-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="fa761-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa761-129">Property</span></span>|<span data-ttu-id="fa761-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fa761-130">Type</span></span>|<span data-ttu-id="fa761-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fa761-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa761-132">id</span><span class="sxs-lookup"><span data-stu-id="fa761-132">id</span></span>|<span data-ttu-id="fa761-133">String</span><span class="sxs-lookup"><span data-stu-id="fa761-133">String</span></span>|<span data-ttu-id="fa761-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fa761-134">Key of the entity.</span></span>|
|<span data-ttu-id="fa761-135">target</span><span class="sxs-lookup"><span data-stu-id="fa761-135">target</span></span>|[<span data-ttu-id="fa761-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fa761-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fa761-137">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="fa761-137">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="fa761-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa761-138">Response</span></span>
<span data-ttu-id="fa761-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa761-139">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa761-140">Пример</span><span class="sxs-lookup"><span data-stu-id="fa761-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa761-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa761-141">Request</span></span>
<span data-ttu-id="fa761-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa761-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="fa761-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa761-143">Response</span></span>
<span data-ttu-id="fa761-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa761-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




