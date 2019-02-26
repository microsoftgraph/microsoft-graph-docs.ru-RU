---
title: Обновление объекта deviceCompliancePolicyAssignment
description: Обновление свойств объекта deviceCompliancePolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5bfc22224b9ae1661c9a57c785df488212a6d5e2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254235"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="47b96-103">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="47b96-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="47b96-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47b96-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47b96-105">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="47b96-105">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47b96-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="47b96-106">Prerequisites</span></span>
<span data-ttu-id="47b96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="47b96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="47b96-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47b96-109">Permission type</span></span>|<span data-ttu-id="47b96-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47b96-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47b96-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47b96-111">Delegated (work or school account)</span></span>|<span data-ttu-id="47b96-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47b96-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47b96-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47b96-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47b96-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47b96-114">Not supported.</span></span>|
|<span data-ttu-id="47b96-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47b96-115">Application</span></span>|<span data-ttu-id="47b96-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47b96-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47b96-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47b96-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="47b96-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47b96-118">Request headers</span></span>
|<span data-ttu-id="47b96-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47b96-119">Header</span></span>|<span data-ttu-id="47b96-120">Значение</span><span class="sxs-lookup"><span data-stu-id="47b96-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47b96-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="47b96-121">Authorization</span></span>|<span data-ttu-id="47b96-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="47b96-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47b96-123">Accept</span><span class="sxs-lookup"><span data-stu-id="47b96-123">Accept</span></span>|<span data-ttu-id="47b96-124">application/json</span><span class="sxs-lookup"><span data-stu-id="47b96-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47b96-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47b96-125">Request body</span></span>
<span data-ttu-id="47b96-126">В тексте запроса добавьте представление объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47b96-126">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="47b96-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="47b96-127">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="47b96-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="47b96-128">Property</span></span>|<span data-ttu-id="47b96-129">Тип</span><span class="sxs-lookup"><span data-stu-id="47b96-129">Type</span></span>|<span data-ttu-id="47b96-130">Описание</span><span class="sxs-lookup"><span data-stu-id="47b96-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47b96-131">id</span><span class="sxs-lookup"><span data-stu-id="47b96-131">id</span></span>|<span data-ttu-id="47b96-132">String</span><span class="sxs-lookup"><span data-stu-id="47b96-132">String</span></span>|<span data-ttu-id="47b96-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="47b96-133">Key of the entity.</span></span>|
|<span data-ttu-id="47b96-134">target</span><span class="sxs-lookup"><span data-stu-id="47b96-134">target</span></span>|[<span data-ttu-id="47b96-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="47b96-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="47b96-136">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="47b96-136">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="47b96-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="47b96-137">Response</span></span>
<span data-ttu-id="47b96-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47b96-138">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47b96-139">Пример</span><span class="sxs-lookup"><span data-stu-id="47b96-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="47b96-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="47b96-140">Request</span></span>
<span data-ttu-id="47b96-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47b96-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47b96-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="47b96-142">Response</span></span>
<span data-ttu-id="47b96-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="47b96-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



