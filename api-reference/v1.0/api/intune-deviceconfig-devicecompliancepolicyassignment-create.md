---
title: Создание объекта deviceCompliancePolicyAssignment
description: Создание объекта deviceCompliancePolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68326b0c845b043a939988ca605b666680c1a0b5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985615"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="09509-103">Создание объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="09509-103">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="09509-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09509-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09509-105">Создание объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="09509-105">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09509-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="09509-106">Prerequisites</span></span>
<span data-ttu-id="09509-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09509-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09509-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09509-109">Permission type</span></span>|<span data-ttu-id="09509-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09509-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09509-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09509-111">Delegated (work or school account)</span></span>|<span data-ttu-id="09509-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09509-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09509-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09509-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09509-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09509-114">Not supported.</span></span>|
|<span data-ttu-id="09509-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09509-115">Application</span></span>|<span data-ttu-id="09509-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09509-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09509-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09509-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="09509-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09509-118">Request headers</span></span>
|<span data-ttu-id="09509-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09509-119">Header</span></span>|<span data-ttu-id="09509-120">Значение</span><span class="sxs-lookup"><span data-stu-id="09509-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09509-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09509-121">Authorization</span></span>|<span data-ttu-id="09509-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09509-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09509-123">Accept</span><span class="sxs-lookup"><span data-stu-id="09509-123">Accept</span></span>|<span data-ttu-id="09509-124">application/json</span><span class="sxs-lookup"><span data-stu-id="09509-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09509-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="09509-125">Request body</span></span>
<span data-ttu-id="09509-126">В тексте запроса добавьте представление объекта deviceCompliancePolicyAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09509-126">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="09509-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="09509-127">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="09509-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="09509-128">Property</span></span>|<span data-ttu-id="09509-129">Тип</span><span class="sxs-lookup"><span data-stu-id="09509-129">Type</span></span>|<span data-ttu-id="09509-130">Описание</span><span class="sxs-lookup"><span data-stu-id="09509-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09509-131">id</span><span class="sxs-lookup"><span data-stu-id="09509-131">id</span></span>|<span data-ttu-id="09509-132">String</span><span class="sxs-lookup"><span data-stu-id="09509-132">String</span></span>|<span data-ttu-id="09509-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="09509-133">Key of the entity.</span></span>|
|<span data-ttu-id="09509-134">target</span><span class="sxs-lookup"><span data-stu-id="09509-134">target</span></span>|[<span data-ttu-id="09509-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="09509-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="09509-136">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="09509-136">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="09509-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="09509-137">Response</span></span>
<span data-ttu-id="09509-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="09509-138">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09509-139">Пример</span><span class="sxs-lookup"><span data-stu-id="09509-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="09509-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="09509-140">Request</span></span>
<span data-ttu-id="09509-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09509-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="09509-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="09509-142">Response</span></span>
<span data-ttu-id="09509-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09509-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



