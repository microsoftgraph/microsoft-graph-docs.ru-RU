---
title: Тип ресурса deviceConfigurationGroupAssignment
description: Назначение группы конфигурации устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1805cb29e8920876d8a340c9379d7b3200c4c779
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789166"
---
# <a name="deviceconfigurationgroupassignment-resource-type"></a><span data-ttu-id="735f7-103">Тип ресурса deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="735f7-103">deviceConfigurationGroupAssignment resource type</span></span>

> <span data-ttu-id="735f7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="735f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="735f7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="735f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="735f7-106">Назначение группы конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="735f7-106">Device configuration group assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="735f7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="735f7-107">Methods</span></span>
|<span data-ttu-id="735f7-108">Метод</span><span class="sxs-lookup"><span data-stu-id="735f7-108">Method</span></span>|<span data-ttu-id="735f7-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="735f7-109">Return Type</span></span>|<span data-ttu-id="735f7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="735f7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="735f7-111">Список Девицеконфигуратионграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="735f7-111">List deviceConfigurationGroupAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-list.md)|<span data-ttu-id="735f7-112">Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="735f7-112">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="735f7-113">Список свойств и связей объектов [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="735f7-113">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="735f7-114">Получение deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="735f7-114">Get deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-get.md)|[<span data-ttu-id="735f7-115">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="735f7-115">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="735f7-116">Чтение свойств и связей объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="735f7-116">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="735f7-117">Создание deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="735f7-117">Create deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-create.md)|[<span data-ttu-id="735f7-118">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="735f7-118">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="735f7-119">Создание нового объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="735f7-119">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="735f7-120">Удаление deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="735f7-120">Delete deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-delete.md)|<span data-ttu-id="735f7-121">Нет</span><span class="sxs-lookup"><span data-stu-id="735f7-121">None</span></span>|<span data-ttu-id="735f7-122">Удаляет объект [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="735f7-122">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>|
|[<span data-ttu-id="735f7-123">Обновление deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="735f7-123">Update deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-update.md)|[<span data-ttu-id="735f7-124">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="735f7-124">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="735f7-125">Обновление свойств объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="735f7-125">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="735f7-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="735f7-126">Properties</span></span>
|<span data-ttu-id="735f7-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="735f7-127">Property</span></span>|<span data-ttu-id="735f7-128">Тип</span><span class="sxs-lookup"><span data-stu-id="735f7-128">Type</span></span>|<span data-ttu-id="735f7-129">Описание</span><span class="sxs-lookup"><span data-stu-id="735f7-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="735f7-130">id</span><span class="sxs-lookup"><span data-stu-id="735f7-130">id</span></span>|<span data-ttu-id="735f7-131">String</span><span class="sxs-lookup"><span data-stu-id="735f7-131">String</span></span>|<span data-ttu-id="735f7-132">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="735f7-132">Key of the entity.</span></span>|
|<span data-ttu-id="735f7-133">Таржетграупид</span><span class="sxs-lookup"><span data-stu-id="735f7-133">targetGroupId</span></span>|<span data-ttu-id="735f7-134">String</span><span class="sxs-lookup"><span data-stu-id="735f7-134">String</span></span>|<span data-ttu-id="735f7-135">Идентификатор группы AAD, на которую направляться конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="735f7-135">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="735f7-136">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="735f7-136">excludeGroup</span></span>|<span data-ttu-id="735f7-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="735f7-137">Boolean</span></span>|<span data-ttu-id="735f7-138">Указывает, следует ли исключить эту группу.</span><span class="sxs-lookup"><span data-stu-id="735f7-138">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="735f7-139">Значения по умолчанию, включаемые в группу</span><span class="sxs-lookup"><span data-stu-id="735f7-139">Defaults that the group should be included</span></span>|

## <a name="relationships"></a><span data-ttu-id="735f7-140">Связи</span><span class="sxs-lookup"><span data-stu-id="735f7-140">Relationships</span></span>
|<span data-ttu-id="735f7-141">Отношение</span><span class="sxs-lookup"><span data-stu-id="735f7-141">Relationship</span></span>|<span data-ttu-id="735f7-142">Тип</span><span class="sxs-lookup"><span data-stu-id="735f7-142">Type</span></span>|<span data-ttu-id="735f7-143">Описание</span><span class="sxs-lookup"><span data-stu-id="735f7-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="735f7-144">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="735f7-144">deviceConfiguration</span></span>|[<span data-ttu-id="735f7-145">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="735f7-145">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="735f7-146">Ссылка навигации на целевую конфигурацию устройства.</span><span class="sxs-lookup"><span data-stu-id="735f7-146">The navigation link to the Device Configuration being targeted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="735f7-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="735f7-147">JSON Representation</span></span>
<span data-ttu-id="735f7-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="735f7-148">Here is a JSON representation of the resource.</span></span>
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





