---
title: Тип ресурса groupPolicyConfigurationAssignment
description: Объект назначения конфигурации групповой политики назначает одну или несколько групп AAD определенной конфигурации групповой политики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 951219f66d8c73a94b24a7370aefd14086107bba
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155925"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="677df-103">Тип ресурса groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="677df-103">groupPolicyConfigurationAssignment resource type</span></span>

<span data-ttu-id="677df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="677df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="677df-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="677df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="677df-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="677df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="677df-107">Объект назначения конфигурации групповой политики назначает одну или несколько групп AAD определенной конфигурации групповой политики.</span><span class="sxs-lookup"><span data-stu-id="677df-107">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="677df-108">Методы</span><span class="sxs-lookup"><span data-stu-id="677df-108">Methods</span></span>
|<span data-ttu-id="677df-109">Метод</span><span class="sxs-lookup"><span data-stu-id="677df-109">Method</span></span>|<span data-ttu-id="677df-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="677df-110">Return Type</span></span>|<span data-ttu-id="677df-111">Описание</span><span class="sxs-lookup"><span data-stu-id="677df-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="677df-112">Список groupPolicyConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="677df-112">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="677df-113">[Коллекция groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="677df-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="677df-114">Список свойств и связей объектов [groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="677df-114">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="677df-115">Get groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="677df-115">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="677df-116">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="677df-116">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="677df-117">Чтение свойств и связей объекта [groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="677df-117">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="677df-118">Создание groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="677df-118">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="677df-119">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="677df-119">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="677df-120">Создание объекта [groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="677df-120">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="677df-121">Удаление groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="677df-121">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="677df-122">Нет</span><span class="sxs-lookup"><span data-stu-id="677df-122">None</span></span>|<span data-ttu-id="677df-123">Удаляет [groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="677df-123">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="677df-124">Обновление groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="677df-124">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="677df-125">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="677df-125">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="677df-126">Обновление свойств объекта [groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="677df-126">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="677df-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="677df-127">Properties</span></span>
|<span data-ttu-id="677df-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="677df-128">Property</span></span>|<span data-ttu-id="677df-129">Тип</span><span class="sxs-lookup"><span data-stu-id="677df-129">Type</span></span>|<span data-ttu-id="677df-130">Описание</span><span class="sxs-lookup"><span data-stu-id="677df-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="677df-131">id</span><span class="sxs-lookup"><span data-stu-id="677df-131">id</span></span>|<span data-ttu-id="677df-132">String</span><span class="sxs-lookup"><span data-stu-id="677df-132">String</span></span>|<span data-ttu-id="677df-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="677df-133">Key of the entity.</span></span>|
|<span data-ttu-id="677df-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="677df-134">lastModifiedDateTime</span></span>|<span data-ttu-id="677df-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="677df-135">DateTimeOffset</span></span>|<span data-ttu-id="677df-136">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="677df-136">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="677df-137">target</span><span class="sxs-lookup"><span data-stu-id="677df-137">target</span></span>|[<span data-ttu-id="677df-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="677df-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="677df-139">Тип групп, нацеленных на конфигурацию групповой политики.</span><span class="sxs-lookup"><span data-stu-id="677df-139">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="677df-140">Связи</span><span class="sxs-lookup"><span data-stu-id="677df-140">Relationships</span></span>
<span data-ttu-id="677df-141">Нет</span><span class="sxs-lookup"><span data-stu-id="677df-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="677df-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="677df-142">JSON Representation</span></span>
<span data-ttu-id="677df-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="677df-143">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




