---
title: Обновление объекта deviceCompliancePolicyAssignment
description: Обновление свойств объекта deviceCompliancePolicyAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f3ec6c1f38cbe2b6130a4f8f9f4b3b97ae85117
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354177"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="e76b0-103">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e76b0-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="e76b0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e76b0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e76b0-105">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e76b0-105">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e76b0-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e76b0-106">Prerequisites</span></span>
<span data-ttu-id="e76b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e76b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e76b0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e76b0-109">Permission type</span></span>|<span data-ttu-id="e76b0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e76b0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e76b0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e76b0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e76b0-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e76b0-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e76b0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e76b0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e76b0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e76b0-114">Not supported.</span></span>|
|<span data-ttu-id="e76b0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e76b0-115">Application</span></span>|<span data-ttu-id="e76b0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e76b0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e76b0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e76b0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e76b0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e76b0-118">Request headers</span></span>
|<span data-ttu-id="e76b0-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e76b0-119">Header</span></span>|<span data-ttu-id="e76b0-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e76b0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e76b0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e76b0-121">Authorization</span></span>|<span data-ttu-id="e76b0-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e76b0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e76b0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e76b0-123">Accept</span></span>|<span data-ttu-id="e76b0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e76b0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e76b0-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e76b0-125">Request body</span></span>
<span data-ttu-id="e76b0-126">В тексте запроса добавьте представление объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e76b0-126">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="e76b0-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e76b0-127">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="e76b0-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e76b0-128">Property</span></span>|<span data-ttu-id="e76b0-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e76b0-129">Type</span></span>|<span data-ttu-id="e76b0-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e76b0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e76b0-131">id</span><span class="sxs-lookup"><span data-stu-id="e76b0-131">id</span></span>|<span data-ttu-id="e76b0-132">String</span><span class="sxs-lookup"><span data-stu-id="e76b0-132">String</span></span>|<span data-ttu-id="e76b0-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e76b0-133">Key of the entity.</span></span>|
|<span data-ttu-id="e76b0-134">target</span><span class="sxs-lookup"><span data-stu-id="e76b0-134">target</span></span>|[<span data-ttu-id="e76b0-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e76b0-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e76b0-136">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="e76b0-136">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="e76b0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e76b0-137">Response</span></span>
<span data-ttu-id="e76b0-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e76b0-138">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e76b0-139">Пример</span><span class="sxs-lookup"><span data-stu-id="e76b0-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="e76b0-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e76b0-140">Request</span></span>
<span data-ttu-id="e76b0-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e76b0-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e76b0-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e76b0-142">Response</span></span>
<span data-ttu-id="e76b0-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e76b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




