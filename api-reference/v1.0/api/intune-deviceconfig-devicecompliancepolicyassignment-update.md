---
title: Обновление объекта deviceCompliancePolicyAssignment
description: Обновление свойств объекта deviceCompliancePolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9bc05524538cbb9fd1321d2fdb12da4c5a6b7412
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459691"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="0a42d-103">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="0a42d-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="0a42d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a42d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a42d-105">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0a42d-105">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a42d-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0a42d-106">Prerequisites</span></span>
<span data-ttu-id="0a42d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a42d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a42d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a42d-109">Permission type</span></span>|<span data-ttu-id="0a42d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a42d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a42d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a42d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0a42d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a42d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0a42d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a42d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a42d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a42d-114">Not supported.</span></span>|
|<span data-ttu-id="0a42d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a42d-115">Application</span></span>|<span data-ttu-id="0a42d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a42d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a42d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a42d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="0a42d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a42d-118">Request headers</span></span>
|<span data-ttu-id="0a42d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a42d-119">Header</span></span>|<span data-ttu-id="0a42d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0a42d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a42d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a42d-121">Authorization</span></span>|<span data-ttu-id="0a42d-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a42d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a42d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0a42d-123">Accept</span></span>|<span data-ttu-id="0a42d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0a42d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a42d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a42d-125">Request body</span></span>
<span data-ttu-id="0a42d-126">В тексте запроса добавьте представление объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a42d-126">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="0a42d-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0a42d-127">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="0a42d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a42d-128">Property</span></span>|<span data-ttu-id="0a42d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0a42d-129">Type</span></span>|<span data-ttu-id="0a42d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0a42d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a42d-131">id</span><span class="sxs-lookup"><span data-stu-id="0a42d-131">id</span></span>|<span data-ttu-id="0a42d-132">String</span><span class="sxs-lookup"><span data-stu-id="0a42d-132">String</span></span>|<span data-ttu-id="0a42d-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0a42d-133">Key of the entity.</span></span>|
|<span data-ttu-id="0a42d-134">target</span><span class="sxs-lookup"><span data-stu-id="0a42d-134">target</span></span>|[<span data-ttu-id="0a42d-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0a42d-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0a42d-136">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="0a42d-136">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="0a42d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a42d-137">Response</span></span>
<span data-ttu-id="0a42d-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0a42d-138">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a42d-139">Пример</span><span class="sxs-lookup"><span data-stu-id="0a42d-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a42d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a42d-140">Request</span></span>
<span data-ttu-id="0a42d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a42d-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0a42d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a42d-142">Response</span></span>
<span data-ttu-id="0a42d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a42d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



