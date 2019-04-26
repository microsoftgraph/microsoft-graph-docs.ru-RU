---
title: Тип ресурса deviceConfigurationGroupAssignment
description: Назначение группы конфигурации устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1805cb29e8920876d8a340c9379d7b3200c4c779
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568147"
---
# <a name="deviceconfigurationgroupassignment-resource-type"></a><span data-ttu-id="8c331-103">Тип ресурса deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="8c331-103">deviceConfigurationGroupAssignment resource type</span></span>

> <span data-ttu-id="8c331-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c331-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c331-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c331-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c331-106">Назначение группы конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8c331-106">Device configuration group assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="8c331-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8c331-107">Methods</span></span>
|<span data-ttu-id="8c331-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8c331-108">Method</span></span>|<span data-ttu-id="8c331-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8c331-109">Return Type</span></span>|<span data-ttu-id="8c331-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8c331-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8c331-111">Список Девицеконфигуратионграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="8c331-111">List deviceConfigurationGroupAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-list.md)|<span data-ttu-id="8c331-112">Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8c331-112">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="8c331-113">Список свойств и связей объектов [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8c331-113">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="8c331-114">Получение deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="8c331-114">Get deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-get.md)|[<span data-ttu-id="8c331-115">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="8c331-115">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="8c331-116">Чтение свойств и связей объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8c331-116">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="8c331-117">Создание deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="8c331-117">Create deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-create.md)|[<span data-ttu-id="8c331-118">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="8c331-118">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="8c331-119">Создание нового объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8c331-119">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="8c331-120">Удаление deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="8c331-120">Delete deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-delete.md)|<span data-ttu-id="8c331-121">Нет</span><span class="sxs-lookup"><span data-stu-id="8c331-121">None</span></span>|<span data-ttu-id="8c331-122">Удаляет объект [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8c331-122">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>|
|[<span data-ttu-id="8c331-123">Обновление deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="8c331-123">Update deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-update.md)|[<span data-ttu-id="8c331-124">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="8c331-124">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="8c331-125">Обновление свойств объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8c331-125">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8c331-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c331-126">Properties</span></span>
|<span data-ttu-id="8c331-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c331-127">Property</span></span>|<span data-ttu-id="8c331-128">Тип</span><span class="sxs-lookup"><span data-stu-id="8c331-128">Type</span></span>|<span data-ttu-id="8c331-129">Описание</span><span class="sxs-lookup"><span data-stu-id="8c331-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c331-130">id</span><span class="sxs-lookup"><span data-stu-id="8c331-130">id</span></span>|<span data-ttu-id="8c331-131">String</span><span class="sxs-lookup"><span data-stu-id="8c331-131">String</span></span>|<span data-ttu-id="8c331-132">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8c331-132">Key of the entity.</span></span>|
|<span data-ttu-id="8c331-133">Таржетграупид</span><span class="sxs-lookup"><span data-stu-id="8c331-133">targetGroupId</span></span>|<span data-ttu-id="8c331-134">String</span><span class="sxs-lookup"><span data-stu-id="8c331-134">String</span></span>|<span data-ttu-id="8c331-135">Идентификатор группы AAD, на которую направляться конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="8c331-135">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="8c331-136">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="8c331-136">excludeGroup</span></span>|<span data-ttu-id="8c331-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c331-137">Boolean</span></span>|<span data-ttu-id="8c331-138">Указывает, следует ли исключить эту группу.</span><span class="sxs-lookup"><span data-stu-id="8c331-138">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="8c331-139">Значения по умолчанию, включаемые в группу</span><span class="sxs-lookup"><span data-stu-id="8c331-139">Defaults that the group should be included</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c331-140">Связи</span><span class="sxs-lookup"><span data-stu-id="8c331-140">Relationships</span></span>
|<span data-ttu-id="8c331-141">Отношение</span><span class="sxs-lookup"><span data-stu-id="8c331-141">Relationship</span></span>|<span data-ttu-id="8c331-142">Тип</span><span class="sxs-lookup"><span data-stu-id="8c331-142">Type</span></span>|<span data-ttu-id="8c331-143">Описание</span><span class="sxs-lookup"><span data-stu-id="8c331-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c331-144">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c331-144">deviceConfiguration</span></span>|<span data-ttu-id="8c331-145">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="8c331-145">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|<span data-ttu-id="8c331-146">Ссылка навигации на целевую конфигурацию устройства.</span><span class="sxs-lookup"><span data-stu-id="8c331-146">The navigation link to the Device Configuration being targeted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c331-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c331-147">JSON Representation</span></span>
<span data-ttu-id="8c331-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c331-148">Here is a JSON representation of the resource.</span></span>
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





