---
title: Тип ресурса deviceManagementScriptGroupAssignment
description: Содержит свойства, используемые для назначения сценарий управления устройства в группу.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8c1077cb3892cad210033abcd21a7abf2ee2e397
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934760"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a><span data-ttu-id="a6fd7-103">Тип ресурса deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a6fd7-103">deviceManagementScriptGroupAssignment resource type</span></span>

> <span data-ttu-id="a6fd7-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a6fd7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6fd7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6fd7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6fd7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a6fd7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6fd7-107">Содержит свойства, используемые для назначения сценарий управления устройства в группу.</span><span class="sxs-lookup"><span data-stu-id="a6fd7-107">Contains properties used to assign a device management script to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="a6fd7-108">Методы</span><span class="sxs-lookup"><span data-stu-id="a6fd7-108">Methods</span></span>
|<span data-ttu-id="a6fd7-109">Метод</span><span class="sxs-lookup"><span data-stu-id="a6fd7-109">Method</span></span>|<span data-ttu-id="a6fd7-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a6fd7-110">Return Type</span></span>|<span data-ttu-id="a6fd7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a6fd7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a6fd7-112">Список deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="a6fd7-112">List deviceManagementScriptGroupAssignments</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|<span data-ttu-id="a6fd7-113">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a6fd7-113">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="a6fd7-114">Свойства списка и связей объектов [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a6fd7-114">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="a6fd7-115">Получение deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a6fd7-115">Get deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[<span data-ttu-id="a6fd7-116">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a6fd7-116">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="a6fd7-117">Чтение свойства и связи объекта [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a6fd7-117">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="a6fd7-118">Создание deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a6fd7-118">Create deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[<span data-ttu-id="a6fd7-119">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a6fd7-119">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="a6fd7-120">Создание нового объекта [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a6fd7-120">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="a6fd7-121">Удаление deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a6fd7-121">Delete deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|<span data-ttu-id="a6fd7-122">Нет</span><span class="sxs-lookup"><span data-stu-id="a6fd7-122">None</span></span>|<span data-ttu-id="a6fd7-123">Удаляет [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a6fd7-123">Deletes a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>|
|[<span data-ttu-id="a6fd7-124">Обновление deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a6fd7-124">Update deviceManagementScriptGroupAssignment</span></span>](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[<span data-ttu-id="a6fd7-125">deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a6fd7-125">deviceManagementScriptGroupAssignment</span></span>](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|<span data-ttu-id="a6fd7-126">Обновление свойства объекта [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a6fd7-126">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a6fd7-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6fd7-127">Properties</span></span>
|<span data-ttu-id="a6fd7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6fd7-128">Property</span></span>|<span data-ttu-id="a6fd7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a6fd7-129">Type</span></span>|<span data-ttu-id="a6fd7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a6fd7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6fd7-131">id</span><span class="sxs-lookup"><span data-stu-id="a6fd7-131">id</span></span>|<span data-ttu-id="a6fd7-132">Строка</span><span class="sxs-lookup"><span data-stu-id="a6fd7-132">String</span></span>|<span data-ttu-id="a6fd7-133">Ключ объекта назначения группы, сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="a6fd7-133">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="a6fd7-134">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="a6fd7-134">targetGroupId</span></span>|<span data-ttu-id="a6fd7-135">Строка</span><span class="sxs-lookup"><span data-stu-id="a6fd7-135">String</span></span>|<span data-ttu-id="a6fd7-136">Идентификатор группы Azure Active Directory мы ориентация сценария.</span><span class="sxs-lookup"><span data-stu-id="a6fd7-136">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6fd7-137">Связи</span><span class="sxs-lookup"><span data-stu-id="a6fd7-137">Relationships</span></span>
<span data-ttu-id="a6fd7-138">Нет</span><span class="sxs-lookup"><span data-stu-id="a6fd7-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a6fd7-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6fd7-139">JSON Representation</span></span>
<span data-ttu-id="a6fd7-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6fd7-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```





