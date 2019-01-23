---
title: Тип ресурса groupPolicyConfigurationAssignment
description: Сущности Назначение конфигурации групповой политики, назначает одной или нескольких групп AAD Настройка определенных групповой политики.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 508581ba7b5ac689338c179f4f6b211928c9abaf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430657"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="99624-103">Тип ресурса groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="99624-103">groupPolicyConfigurationAssignment resource type</span></span>

> <span data-ttu-id="99624-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="99624-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="99624-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99624-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99624-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99624-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99624-107">Сущности Назначение конфигурации групповой политики, назначает одной или нескольких групп AAD Настройка определенных групповой политики.</span><span class="sxs-lookup"><span data-stu-id="99624-107">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="99624-108">Методы</span><span class="sxs-lookup"><span data-stu-id="99624-108">Methods</span></span>
|<span data-ttu-id="99624-109">Метод</span><span class="sxs-lookup"><span data-stu-id="99624-109">Method</span></span>|<span data-ttu-id="99624-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="99624-110">Return Type</span></span>|<span data-ttu-id="99624-111">Описание</span><span class="sxs-lookup"><span data-stu-id="99624-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="99624-112">Список groupPolicyConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="99624-112">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="99624-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="99624-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="99624-114">Свойства списка и связей объектов [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="99624-114">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="99624-115">Получение groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="99624-115">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="99624-116">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="99624-116">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="99624-117">Чтение свойства и связи объекта [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="99624-117">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="99624-118">Создание groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="99624-118">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="99624-119">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="99624-119">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="99624-120">Создание нового объекта [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="99624-120">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="99624-121">Удаление groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="99624-121">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="99624-122">Нет</span><span class="sxs-lookup"><span data-stu-id="99624-122">None</span></span>|<span data-ttu-id="99624-123">Удаляет [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="99624-123">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="99624-124">Обновление groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="99624-124">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="99624-125">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="99624-125">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="99624-126">Обновление свойства объекта [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="99624-126">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="99624-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="99624-127">Properties</span></span>
|<span data-ttu-id="99624-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="99624-128">Property</span></span>|<span data-ttu-id="99624-129">Тип</span><span class="sxs-lookup"><span data-stu-id="99624-129">Type</span></span>|<span data-ttu-id="99624-130">Описание</span><span class="sxs-lookup"><span data-stu-id="99624-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99624-131">id</span><span class="sxs-lookup"><span data-stu-id="99624-131">id</span></span>|<span data-ttu-id="99624-132">String</span><span class="sxs-lookup"><span data-stu-id="99624-132">String</span></span>|<span data-ttu-id="99624-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="99624-133">Key of the entity.</span></span>|
|<span data-ttu-id="99624-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99624-134">lastModifiedDateTime</span></span>|<span data-ttu-id="99624-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99624-135">DateTimeOffset</span></span>|<span data-ttu-id="99624-136">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="99624-136">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="99624-137">target</span><span class="sxs-lookup"><span data-stu-id="99624-137">target</span></span>|[<span data-ttu-id="99624-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="99624-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="99624-139">Тип группы целевой параметры групповой политики.</span><span class="sxs-lookup"><span data-stu-id="99624-139">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99624-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="99624-140">Relationships</span></span>
<span data-ttu-id="99624-141">Нет</span><span class="sxs-lookup"><span data-stu-id="99624-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99624-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="99624-142">JSON Representation</span></span>
<span data-ttu-id="99624-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99624-143">Here is a JSON representation of the resource.</span></span>
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




