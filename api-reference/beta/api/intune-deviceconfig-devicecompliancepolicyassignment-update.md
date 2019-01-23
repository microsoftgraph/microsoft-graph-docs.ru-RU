---
title: Обновление объекта deviceCompliancePolicyAssignment
description: Обновление свойств объекта deviceCompliancePolicyAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6867d55434d1c2e496e264002969289c12576461
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394910"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="65db9-103">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="65db9-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="65db9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="65db9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="65db9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65db9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65db9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65db9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65db9-107">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="65db9-107">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65db9-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="65db9-108">Prerequisites</span></span>
<span data-ttu-id="65db9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="65db9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="65db9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65db9-111">Permission type</span></span>|<span data-ttu-id="65db9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="65db9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65db9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65db9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65db9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65db9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65db9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65db9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65db9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65db9-116">Not supported.</span></span>|
|<span data-ttu-id="65db9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65db9-117">Application</span></span>|<span data-ttu-id="65db9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65db9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65db9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65db9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="65db9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65db9-120">Request headers</span></span>
|<span data-ttu-id="65db9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65db9-121">Header</span></span>|<span data-ttu-id="65db9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="65db9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65db9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="65db9-123">Authorization</span></span>|<span data-ttu-id="65db9-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="65db9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65db9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="65db9-125">Accept</span></span>|<span data-ttu-id="65db9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65db9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65db9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65db9-127">Request body</span></span>
<span data-ttu-id="65db9-128">В тексте запроса добавьте представление объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65db9-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="65db9-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="65db9-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="65db9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="65db9-130">Property</span></span>|<span data-ttu-id="65db9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="65db9-131">Type</span></span>|<span data-ttu-id="65db9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="65db9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65db9-133">id</span><span class="sxs-lookup"><span data-stu-id="65db9-133">id</span></span>|<span data-ttu-id="65db9-134">String</span><span class="sxs-lookup"><span data-stu-id="65db9-134">String</span></span>|<span data-ttu-id="65db9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="65db9-135">Key of the entity.</span></span>|
|<span data-ttu-id="65db9-136">target</span><span class="sxs-lookup"><span data-stu-id="65db9-136">target</span></span>|[<span data-ttu-id="65db9-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="65db9-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="65db9-138">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="65db9-138">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="65db9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="65db9-139">Response</span></span>
<span data-ttu-id="65db9-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="65db9-140">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65db9-141">Пример</span><span class="sxs-lookup"><span data-stu-id="65db9-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="65db9-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="65db9-142">Request</span></span>
<span data-ttu-id="65db9-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65db9-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="65db9-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="65db9-144">Response</span></span>
<span data-ttu-id="65db9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="65db9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




