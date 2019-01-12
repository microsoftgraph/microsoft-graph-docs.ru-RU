---
title: Тип ресурса deviceConfigurationGroupAssignment
description: Назначение группы конфигурации устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 53e998044760dba40f40f3658b141d8aa05d7082
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943118"
---
# <a name="deviceconfigurationgroupassignment-resource-type"></a><span data-ttu-id="1d838-103">Тип ресурса deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1d838-103">deviceConfigurationGroupAssignment resource type</span></span>

> <span data-ttu-id="1d838-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1d838-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d838-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d838-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d838-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1d838-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d838-107">Назначение группы конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1d838-107">Device configuration group assignment.</span></span>
## <a name="methods"></a><span data-ttu-id="1d838-108">Методы</span><span class="sxs-lookup"><span data-stu-id="1d838-108">Methods</span></span>
|<span data-ttu-id="1d838-109">Метод</span><span class="sxs-lookup"><span data-stu-id="1d838-109">Method</span></span>|<span data-ttu-id="1d838-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1d838-110">Return Type</span></span>|<span data-ttu-id="1d838-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1d838-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1d838-112">Список deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="1d838-112">List deviceConfigurationGroupAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-list.md)|<span data-ttu-id="1d838-113">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="1d838-113">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="1d838-114">Свойства списка и связей объектов [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1d838-114">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="1d838-115">Получение deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1d838-115">Get deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-get.md)|[<span data-ttu-id="1d838-116">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1d838-116">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="1d838-117">Чтение свойства и связи объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1d838-117">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="1d838-118">Создание deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1d838-118">Create deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-create.md)|[<span data-ttu-id="1d838-119">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1d838-119">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="1d838-120">Создание нового объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1d838-120">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="1d838-121">Удаление deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1d838-121">Delete deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-delete.md)|<span data-ttu-id="1d838-122">Нет</span><span class="sxs-lookup"><span data-stu-id="1d838-122">None</span></span>|<span data-ttu-id="1d838-123">Удаляет [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1d838-123">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>|
|[<span data-ttu-id="1d838-124">Обновление deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1d838-124">Update deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-update.md)|[<span data-ttu-id="1d838-125">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1d838-125">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="1d838-126">Обновление свойства объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1d838-126">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1d838-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d838-127">Properties</span></span>
|<span data-ttu-id="1d838-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d838-128">Property</span></span>|<span data-ttu-id="1d838-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1d838-129">Type</span></span>|<span data-ttu-id="1d838-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1d838-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d838-131">id</span><span class="sxs-lookup"><span data-stu-id="1d838-131">id</span></span>|<span data-ttu-id="1d838-132">String</span><span class="sxs-lookup"><span data-stu-id="1d838-132">String</span></span>|<span data-ttu-id="1d838-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1d838-133">Key of the entity.</span></span>|
|<span data-ttu-id="1d838-134">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="1d838-134">targetGroupId</span></span>|<span data-ttu-id="1d838-135">String</span><span class="sxs-lookup"><span data-stu-id="1d838-135">String</span></span>|<span data-ttu-id="1d838-136">Идентификатор группы AAD мы ориентация для настройки устройств.</span><span class="sxs-lookup"><span data-stu-id="1d838-136">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="1d838-137">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="1d838-137">excludeGroup</span></span>|<span data-ttu-id="1d838-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d838-138">Boolean</span></span>|<span data-ttu-id="1d838-139">Указывает, является ли эта группа следует исключить.</span><span class="sxs-lookup"><span data-stu-id="1d838-139">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="1d838-140">Параметры по умолчанию, что группы должны быть включены</span><span class="sxs-lookup"><span data-stu-id="1d838-140">Defaults that the group should be included</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d838-141">Связи</span><span class="sxs-lookup"><span data-stu-id="1d838-141">Relationships</span></span>
|<span data-ttu-id="1d838-142">Связь</span><span class="sxs-lookup"><span data-stu-id="1d838-142">Relationship</span></span>|<span data-ttu-id="1d838-143">Тип</span><span class="sxs-lookup"><span data-stu-id="1d838-143">Type</span></span>|<span data-ttu-id="1d838-144">Описание</span><span class="sxs-lookup"><span data-stu-id="1d838-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d838-145">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1d838-145">deviceConfiguration</span></span>|<span data-ttu-id="1d838-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="1d838-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|<span data-ttu-id="1d838-147">Навигационная ссылка для целевой настройки устройств.</span><span class="sxs-lookup"><span data-stu-id="1d838-147">The navigation link to the Device Configuration being targeted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d838-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d838-148">JSON Representation</span></span>
<span data-ttu-id="1d838-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d838-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String",
  "excludeGroup": true
}
```





