---
title: Тип ресурса deviceManagementScriptAssignment
description: Содержит свойства, используемые для назначения сценарий управления устройства в группу.
author: tfitzmac
ms.openlocfilehash: d0b08363de392a337338bb2cd892359b8b9a9345
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351242"
---
# <a name="devicemanagementscriptassignment-resource-type"></a><span data-ttu-id="40417-103">Тип ресурса deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="40417-103">deviceManagementScriptAssignment resource type</span></span>

> <span data-ttu-id="40417-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="40417-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40417-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40417-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40417-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="40417-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40417-107">Содержит свойства, используемые для назначения сценарий управления устройства в группу.</span><span class="sxs-lookup"><span data-stu-id="40417-107">Contains properties used to assign a device management script to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="40417-108">Методы</span><span class="sxs-lookup"><span data-stu-id="40417-108">Methods</span></span>
|<span data-ttu-id="40417-109">Метод</span><span class="sxs-lookup"><span data-stu-id="40417-109">Method</span></span>|<span data-ttu-id="40417-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="40417-110">Return Type</span></span>|<span data-ttu-id="40417-111">Описание</span><span class="sxs-lookup"><span data-stu-id="40417-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="40417-112">Список deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="40417-112">List deviceManagementScriptAssignments</span></span>](../api/intune-devices-devicemanagementscriptassignment-list.md)|<span data-ttu-id="40417-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="40417-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="40417-114">Свойства списка и связей объектов [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="40417-114">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="40417-115">Получение deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="40417-115">Get deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-get.md)|<span data-ttu-id="40417-116">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md);</span><span class="sxs-lookup"><span data-stu-id="40417-116">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)</span></span>|<span data-ttu-id="40417-117">Чтение свойства и связи объекта [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="40417-117">Read properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="40417-118">Создание deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="40417-118">Create deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-create.md)|<span data-ttu-id="40417-119">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md);</span><span class="sxs-lookup"><span data-stu-id="40417-119">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)</span></span>|<span data-ttu-id="40417-120">Создание нового объекта [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="40417-120">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="40417-121">Удаление deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="40417-121">Delete deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-delete.md)|<span data-ttu-id="40417-122">Нет</span><span class="sxs-lookup"><span data-stu-id="40417-122">None</span></span>|<span data-ttu-id="40417-123">Удаляет [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="40417-123">Deletes a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>|
|[<span data-ttu-id="40417-124">Обновление deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="40417-124">Update deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-update.md)|<span data-ttu-id="40417-125">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md);</span><span class="sxs-lookup"><span data-stu-id="40417-125">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)</span></span>|<span data-ttu-id="40417-126">Обновление свойства объекта [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="40417-126">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="40417-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="40417-127">Properties</span></span>
|<span data-ttu-id="40417-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="40417-128">Property</span></span>|<span data-ttu-id="40417-129">Тип</span><span class="sxs-lookup"><span data-stu-id="40417-129">Type</span></span>|<span data-ttu-id="40417-130">Описание</span><span class="sxs-lookup"><span data-stu-id="40417-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40417-131">id</span><span class="sxs-lookup"><span data-stu-id="40417-131">id</span></span>|<span data-ttu-id="40417-132">Строка</span><span class="sxs-lookup"><span data-stu-id="40417-132">String</span></span>|<span data-ttu-id="40417-133">Ключ объекта назначения группы, сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="40417-133">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="40417-134">target</span><span class="sxs-lookup"><span data-stu-id="40417-134">target</span></span>|[<span data-ttu-id="40417-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="40417-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="40417-136">Идентификатор группы Azure Active Directory мы ориентация сценария.</span><span class="sxs-lookup"><span data-stu-id="40417-136">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40417-137">Связи</span><span class="sxs-lookup"><span data-stu-id="40417-137">Relationships</span></span>
<span data-ttu-id="40417-138">Нет</span><span class="sxs-lookup"><span data-stu-id="40417-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="40417-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40417-139">JSON Representation</span></span>
<span data-ttu-id="40417-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40417-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





