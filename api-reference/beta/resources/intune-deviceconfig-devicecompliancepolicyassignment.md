---
title: Тип ресурса deviceCompliancePolicyAssignment
description: Назначение политики соответствия устройств требованиям.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0f49aaf815730ea2c12ced1a811335c3b2779fb5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822843"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="abb14-103">Тип ресурса deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="abb14-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="abb14-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="abb14-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abb14-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abb14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abb14-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="abb14-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abb14-107">Назначение политики соответствия устройств требованиям.</span><span class="sxs-lookup"><span data-stu-id="abb14-107">Device compliance policy assignment.</span></span>
## <a name="methods"></a><span data-ttu-id="abb14-108">Методы</span><span class="sxs-lookup"><span data-stu-id="abb14-108">Methods</span></span>
|<span data-ttu-id="abb14-109">Метод</span><span class="sxs-lookup"><span data-stu-id="abb14-109">Method</span></span>|<span data-ttu-id="abb14-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="abb14-110">Return Type</span></span>|<span data-ttu-id="abb14-111">Описание</span><span class="sxs-lookup"><span data-stu-id="abb14-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="abb14-112">Список объектов deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="abb14-112">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="abb14-113">Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="abb14-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="abb14-114">Список свойств и связей объектов [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="abb14-114">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="abb14-115">Получение объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="abb14-115">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="abb14-116">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="abb14-116">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="abb14-117">Чтение свойств и связей объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="abb14-117">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="abb14-118">Создание объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="abb14-118">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="abb14-119">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="abb14-119">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="abb14-120">Создание объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="abb14-120">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="abb14-121">Удаление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="abb14-121">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="abb14-122">Нет</span><span class="sxs-lookup"><span data-stu-id="abb14-122">None</span></span>|<span data-ttu-id="abb14-123">Удаляет объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="abb14-123">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="abb14-124">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="abb14-124">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="abb14-125">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="abb14-125">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="abb14-126">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="abb14-126">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="abb14-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="abb14-127">Properties</span></span>
|<span data-ttu-id="abb14-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="abb14-128">Property</span></span>|<span data-ttu-id="abb14-129">Тип</span><span class="sxs-lookup"><span data-stu-id="abb14-129">Type</span></span>|<span data-ttu-id="abb14-130">Описание</span><span class="sxs-lookup"><span data-stu-id="abb14-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abb14-131">id</span><span class="sxs-lookup"><span data-stu-id="abb14-131">id</span></span>|<span data-ttu-id="abb14-132">Строка</span><span class="sxs-lookup"><span data-stu-id="abb14-132">String</span></span>|<span data-ttu-id="abb14-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="abb14-133">Key of the entity.</span></span>|
|<span data-ttu-id="abb14-134">target</span><span class="sxs-lookup"><span data-stu-id="abb14-134">target</span></span>|[<span data-ttu-id="abb14-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="abb14-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="abb14-136">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="abb14-136">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="abb14-137">Связи</span><span class="sxs-lookup"><span data-stu-id="abb14-137">Relationships</span></span>
<span data-ttu-id="abb14-138">Нет</span><span class="sxs-lookup"><span data-stu-id="abb14-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="abb14-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="abb14-139">JSON Representation</span></span>
<span data-ttu-id="abb14-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="abb14-140">Here is a JSON representation of the resource.</span></span>
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





