---
title: Тип ресурса Граупполициконфигуратионассигнмент
description: Объект назначения настройки групповой политики назначает одну или несколько групп AAD определенной конфигурации групповой политики.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f6fcd7ace912075189ec3e9b5a817181dd392a5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575823"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="8bb39-103">Тип ресурса Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="8bb39-103">groupPolicyConfigurationAssignment resource type</span></span>

> <span data-ttu-id="8bb39-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bb39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bb39-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bb39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bb39-106">Объект назначения настройки групповой политики назначает одну или несколько групп AAD определенной конфигурации групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8bb39-106">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="8bb39-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8bb39-107">Methods</span></span>
|<span data-ttu-id="8bb39-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8bb39-108">Method</span></span>|<span data-ttu-id="8bb39-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8bb39-109">Return Type</span></span>|<span data-ttu-id="8bb39-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8bb39-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8bb39-111">Список Граупполициконфигуратионассигнментс</span><span class="sxs-lookup"><span data-stu-id="8bb39-111">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="8bb39-112">Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8bb39-112">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8bb39-113">Список свойств и связей объектов [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8bb39-113">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="8bb39-114">Получение Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="8bb39-114">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="8bb39-115">Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="8bb39-115">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="8bb39-116">Чтение свойств и связей объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8bb39-116">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="8bb39-117">Создание Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="8bb39-117">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="8bb39-118">Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="8bb39-118">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="8bb39-119">Создание нового объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8bb39-119">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="8bb39-120">Удаление Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="8bb39-120">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="8bb39-121">Нет</span><span class="sxs-lookup"><span data-stu-id="8bb39-121">None</span></span>|<span data-ttu-id="8bb39-122">Удаляет объект [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8bb39-122">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="8bb39-123">Обновление Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="8bb39-123">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="8bb39-124">Граупполициконфигуратионассигнмент</span><span class="sxs-lookup"><span data-stu-id="8bb39-124">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="8bb39-125">Обновление свойств объекта [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8bb39-125">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8bb39-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="8bb39-126">Properties</span></span>
|<span data-ttu-id="8bb39-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bb39-127">Property</span></span>|<span data-ttu-id="8bb39-128">Тип</span><span class="sxs-lookup"><span data-stu-id="8bb39-128">Type</span></span>|<span data-ttu-id="8bb39-129">Описание</span><span class="sxs-lookup"><span data-stu-id="8bb39-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bb39-130">id</span><span class="sxs-lookup"><span data-stu-id="8bb39-130">id</span></span>|<span data-ttu-id="8bb39-131">String</span><span class="sxs-lookup"><span data-stu-id="8bb39-131">String</span></span>|<span data-ttu-id="8bb39-132">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8bb39-132">Key of the entity.</span></span>|
|<span data-ttu-id="8bb39-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bb39-133">lastModifiedDateTime</span></span>|<span data-ttu-id="8bb39-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bb39-134">DateTimeOffset</span></span>|<span data-ttu-id="8bb39-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8bb39-135">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="8bb39-136">target</span><span class="sxs-lookup"><span data-stu-id="8bb39-136">target</span></span>|[<span data-ttu-id="8bb39-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8bb39-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8bb39-138">Тип групп, нацеленных на конфигурацию групповой политики.</span><span class="sxs-lookup"><span data-stu-id="8bb39-138">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bb39-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="8bb39-139">Relationships</span></span>
<span data-ttu-id="8bb39-140">Нет</span><span class="sxs-lookup"><span data-stu-id="8bb39-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bb39-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8bb39-141">JSON Representation</span></span>
<span data-ttu-id="8bb39-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bb39-142">Here is a JSON representation of the resource.</span></span>
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





