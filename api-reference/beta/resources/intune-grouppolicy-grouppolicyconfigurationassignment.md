---
title: Тип ресурса Граупполициконфигуратионассигнмент
description: Объект назначения настройки групповой политики назначает одну или несколько групп AAD определенной конфигурации групповой политики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fe21e130a870225b7e0b96c3926f1115361bde0e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256136"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="9f0d0-103">Тип ресурса Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="9f0d0-103">groupPolicyConfigurationAssignment resource type</span></span>

<span data-ttu-id="9f0d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f0d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f0d0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f0d0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f0d0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f0d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f0d0-107">Объект назначения настройки групповой политики назначает одну или несколько групп AAD определенной конфигурации групповой политики.</span><span class="sxs-lookup"><span data-stu-id="9f0d0-107">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="9f0d0-108">Методы</span><span class="sxs-lookup"><span data-stu-id="9f0d0-108">Methods</span></span>
|<span data-ttu-id="9f0d0-109">Метод</span><span class="sxs-lookup"><span data-stu-id="9f0d0-109">Method</span></span>|<span data-ttu-id="9f0d0-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9f0d0-110">Return Type</span></span>|<span data-ttu-id="9f0d0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9f0d0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9f0d0-112">Список Граупполициконфигуратионассигнментс</span><span class="sxs-lookup"><span data-stu-id="9f0d0-112">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="9f0d0-113">Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9f0d0-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="9f0d0-114">Список свойств и связей объектов [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9f0d0-114">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="9f0d0-115">Получение Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="9f0d0-115">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="9f0d0-116">граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="9f0d0-116">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="9f0d0-117">Чтение свойств и связей объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9f0d0-117">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="9f0d0-118">Создание Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="9f0d0-118">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="9f0d0-119">граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="9f0d0-119">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="9f0d0-120">Создание нового объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9f0d0-120">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="9f0d0-121">Удаление Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="9f0d0-121">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="9f0d0-122">Нет</span><span class="sxs-lookup"><span data-stu-id="9f0d0-122">None</span></span>|<span data-ttu-id="9f0d0-123">Удаляет объект [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9f0d0-123">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="9f0d0-124">Обновление Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="9f0d0-124">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="9f0d0-125">граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="9f0d0-125">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="9f0d0-126">Обновление свойств объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9f0d0-126">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9f0d0-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f0d0-127">Properties</span></span>
|<span data-ttu-id="9f0d0-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f0d0-128">Property</span></span>|<span data-ttu-id="9f0d0-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9f0d0-129">Type</span></span>|<span data-ttu-id="9f0d0-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9f0d0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f0d0-131">id</span><span class="sxs-lookup"><span data-stu-id="9f0d0-131">id</span></span>|<span data-ttu-id="9f0d0-132">String</span><span class="sxs-lookup"><span data-stu-id="9f0d0-132">String</span></span>|<span data-ttu-id="9f0d0-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9f0d0-133">Key of the entity.</span></span>|
|<span data-ttu-id="9f0d0-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f0d0-134">lastModifiedDateTime</span></span>|<span data-ttu-id="9f0d0-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f0d0-135">DateTimeOffset</span></span>|<span data-ttu-id="9f0d0-136">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9f0d0-136">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="9f0d0-137">target</span><span class="sxs-lookup"><span data-stu-id="9f0d0-137">target</span></span>|[<span data-ttu-id="9f0d0-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9f0d0-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9f0d0-139">Тип групп, нацеленных на конфигурацию групповой политики.</span><span class="sxs-lookup"><span data-stu-id="9f0d0-139">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f0d0-140">Связи</span><span class="sxs-lookup"><span data-stu-id="9f0d0-140">Relationships</span></span>
<span data-ttu-id="9f0d0-141">Нет</span><span class="sxs-lookup"><span data-stu-id="9f0d0-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f0d0-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9f0d0-142">JSON Representation</span></span>
<span data-ttu-id="9f0d0-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f0d0-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```




