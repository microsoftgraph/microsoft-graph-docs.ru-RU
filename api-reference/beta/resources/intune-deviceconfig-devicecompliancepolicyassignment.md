---
title: Тип ресурса deviceCompliancePolicyAssignment
description: Назначение политики соответствия устройств требованиям.
ms.openlocfilehash: 1e553553e81a3d3d68f0766754d770c3f3f24d7f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080841"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="dc7f2-103">Тип ресурса deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="dc7f2-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="dc7f2-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dc7f2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc7f2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc7f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc7f2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dc7f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc7f2-107">Назначение политики соответствия устройств требованиям.</span><span class="sxs-lookup"><span data-stu-id="dc7f2-107">Device compliance policy assignment.</span></span>
## <a name="methods"></a><span data-ttu-id="dc7f2-108">Методы</span><span class="sxs-lookup"><span data-stu-id="dc7f2-108">Methods</span></span>
|<span data-ttu-id="dc7f2-109">Метод</span><span class="sxs-lookup"><span data-stu-id="dc7f2-109">Method</span></span>|<span data-ttu-id="dc7f2-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dc7f2-110">Return Type</span></span>|<span data-ttu-id="dc7f2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dc7f2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dc7f2-112">Список объектов deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="dc7f2-112">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="dc7f2-113">Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="dc7f2-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="dc7f2-114">Список свойств и связей объектов [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dc7f2-114">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="dc7f2-115">Получение объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="dc7f2-115">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="dc7f2-116">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="dc7f2-116">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="dc7f2-117">Чтение свойств и связей объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dc7f2-117">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="dc7f2-118">Создание объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="dc7f2-118">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="dc7f2-119">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="dc7f2-119">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="dc7f2-120">Создание объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dc7f2-120">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="dc7f2-121">Удаление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="dc7f2-121">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="dc7f2-122">Нет</span><span class="sxs-lookup"><span data-stu-id="dc7f2-122">None</span></span>|<span data-ttu-id="dc7f2-123">Удаляет объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dc7f2-123">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="dc7f2-124">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="dc7f2-124">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="dc7f2-125">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="dc7f2-125">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="dc7f2-126">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dc7f2-126">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc7f2-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc7f2-127">Properties</span></span>
|<span data-ttu-id="dc7f2-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc7f2-128">Property</span></span>|<span data-ttu-id="dc7f2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="dc7f2-129">Type</span></span>|<span data-ttu-id="dc7f2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="dc7f2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc7f2-131">id</span><span class="sxs-lookup"><span data-stu-id="dc7f2-131">id</span></span>|<span data-ttu-id="dc7f2-132">String</span><span class="sxs-lookup"><span data-stu-id="dc7f2-132">String</span></span>|<span data-ttu-id="dc7f2-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dc7f2-133">Key of the entity.</span></span>|
|<span data-ttu-id="dc7f2-134">target</span><span class="sxs-lookup"><span data-stu-id="dc7f2-134">target</span></span>|[<span data-ttu-id="dc7f2-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="dc7f2-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="dc7f2-136">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="dc7f2-136">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc7f2-137">Связи</span><span class="sxs-lookup"><span data-stu-id="dc7f2-137">Relationships</span></span>
<span data-ttu-id="dc7f2-138">Нет</span><span class="sxs-lookup"><span data-stu-id="dc7f2-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dc7f2-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc7f2-139">JSON Representation</span></span>
<span data-ttu-id="dc7f2-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc7f2-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





