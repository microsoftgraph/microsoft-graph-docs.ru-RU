---
title: Тип ресурса deviceCompliancePolicyAssignment
description: Назначение политики соответствия устройств требованиям.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 881153242e2af2aeafa39f30b6d303313083cbcf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980071"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="8ad46-103">Тип ресурса deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8ad46-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="8ad46-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8ad46-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ad46-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ad46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ad46-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8ad46-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ad46-107">Назначение политики соответствия устройств требованиям.</span><span class="sxs-lookup"><span data-stu-id="8ad46-107">Device compliance policy assignment.</span></span>
## <a name="methods"></a><span data-ttu-id="8ad46-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8ad46-108">Methods</span></span>
|<span data-ttu-id="8ad46-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8ad46-109">Method</span></span>|<span data-ttu-id="8ad46-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8ad46-110">Return Type</span></span>|<span data-ttu-id="8ad46-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8ad46-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8ad46-112">Список объектов deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8ad46-112">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="8ad46-113">Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8ad46-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="8ad46-114">Список свойств и связей объектов [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8ad46-114">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="8ad46-115">Получение объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8ad46-115">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="8ad46-116">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8ad46-116">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="8ad46-117">Чтение свойств и связей объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8ad46-117">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="8ad46-118">Создание объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8ad46-118">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="8ad46-119">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8ad46-119">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="8ad46-120">Создание объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8ad46-120">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="8ad46-121">Удаление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8ad46-121">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="8ad46-122">Нет</span><span class="sxs-lookup"><span data-stu-id="8ad46-122">None</span></span>|<span data-ttu-id="8ad46-123">Удаляет объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8ad46-123">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="8ad46-124">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8ad46-124">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="8ad46-125">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8ad46-125">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="8ad46-126">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8ad46-126">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8ad46-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ad46-127">Properties</span></span>
|<span data-ttu-id="8ad46-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ad46-128">Property</span></span>|<span data-ttu-id="8ad46-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8ad46-129">Type</span></span>|<span data-ttu-id="8ad46-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8ad46-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ad46-131">id</span><span class="sxs-lookup"><span data-stu-id="8ad46-131">id</span></span>|<span data-ttu-id="8ad46-132">Строка</span><span class="sxs-lookup"><span data-stu-id="8ad46-132">String</span></span>|<span data-ttu-id="8ad46-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8ad46-133">Key of the entity.</span></span>|
|<span data-ttu-id="8ad46-134">target</span><span class="sxs-lookup"><span data-stu-id="8ad46-134">target</span></span>|[<span data-ttu-id="8ad46-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8ad46-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8ad46-136">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="8ad46-136">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ad46-137">Связи</span><span class="sxs-lookup"><span data-stu-id="8ad46-137">Relationships</span></span>
<span data-ttu-id="8ad46-138">Нет</span><span class="sxs-lookup"><span data-stu-id="8ad46-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8ad46-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ad46-139">JSON Representation</span></span>
<span data-ttu-id="8ad46-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ad46-140">Here is a JSON representation of the resource.</span></span>
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





