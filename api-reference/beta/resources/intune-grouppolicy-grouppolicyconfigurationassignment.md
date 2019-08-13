---
title: Тип ресурса Граупполициконфигуратионассигнмент
description: Объект назначения настройки групповой политики назначает одну или несколько групп AAD определенной конфигурации групповой политики.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 82101853def989bad8b80794d176b7d2bca2582b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331520"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="3331f-103">Тип ресурса Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="3331f-103">groupPolicyConfigurationAssignment resource type</span></span>

> <span data-ttu-id="3331f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3331f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3331f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3331f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3331f-106">Объект назначения настройки групповой политики назначает одну или несколько групп AAD определенной конфигурации групповой политики.</span><span class="sxs-lookup"><span data-stu-id="3331f-106">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="3331f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3331f-107">Methods</span></span>
|<span data-ttu-id="3331f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="3331f-108">Method</span></span>|<span data-ttu-id="3331f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3331f-109">Return Type</span></span>|<span data-ttu-id="3331f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3331f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3331f-111">Список Граупполициконфигуратионассигнментс</span><span class="sxs-lookup"><span data-stu-id="3331f-111">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="3331f-112">Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3331f-112">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3331f-113">Список свойств и связей объектов [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3331f-113">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="3331f-114">Получение Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="3331f-114">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="3331f-115">граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="3331f-115">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="3331f-116">Чтение свойств и связей объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3331f-116">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="3331f-117">Создание Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="3331f-117">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="3331f-118">граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="3331f-118">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="3331f-119">Создание нового объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3331f-119">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="3331f-120">Удаление Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="3331f-120">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="3331f-121">Нет</span><span class="sxs-lookup"><span data-stu-id="3331f-121">None</span></span>|<span data-ttu-id="3331f-122">Удаляет объект [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3331f-122">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="3331f-123">Обновление Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="3331f-123">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="3331f-124">граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="3331f-124">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="3331f-125">Обновление свойств объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3331f-125">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3331f-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="3331f-126">Properties</span></span>
|<span data-ttu-id="3331f-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="3331f-127">Property</span></span>|<span data-ttu-id="3331f-128">Тип</span><span class="sxs-lookup"><span data-stu-id="3331f-128">Type</span></span>|<span data-ttu-id="3331f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="3331f-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3331f-130">id</span><span class="sxs-lookup"><span data-stu-id="3331f-130">id</span></span>|<span data-ttu-id="3331f-131">String</span><span class="sxs-lookup"><span data-stu-id="3331f-131">String</span></span>|<span data-ttu-id="3331f-132">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3331f-132">Key of the entity.</span></span>|
|<span data-ttu-id="3331f-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3331f-133">lastModifiedDateTime</span></span>|<span data-ttu-id="3331f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3331f-134">DateTimeOffset</span></span>|<span data-ttu-id="3331f-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3331f-135">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="3331f-136">target</span><span class="sxs-lookup"><span data-stu-id="3331f-136">target</span></span>|[<span data-ttu-id="3331f-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3331f-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3331f-138">Тип групп, нацеленных на конфигурацию групповой политики.</span><span class="sxs-lookup"><span data-stu-id="3331f-138">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3331f-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="3331f-139">Relationships</span></span>
<span data-ttu-id="3331f-140">Нет</span><span class="sxs-lookup"><span data-stu-id="3331f-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3331f-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3331f-141">JSON Representation</span></span>
<span data-ttu-id="3331f-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3331f-142">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



