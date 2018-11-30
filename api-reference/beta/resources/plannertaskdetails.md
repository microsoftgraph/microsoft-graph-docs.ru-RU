---
title: Тип ресурса plannerTaskDetails
description: Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. С каждым объектом task связан объект details.
ms.openlocfilehash: 3d5ab0b3a2f0c2e6c1abf284d5a87c2726c7aa15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082670"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="9d110-104">Тип ресурса plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="9d110-104">plannerTaskDetails resource type</span></span>

> <span data-ttu-id="9d110-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9d110-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d110-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d110-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d110-p103">Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. С каждым объектом [task](plannertask.md) связан объект details.</span><span class="sxs-lookup"><span data-stu-id="9d110-p103">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="9d110-109">Методы</span><span class="sxs-lookup"><span data-stu-id="9d110-109">Methods</span></span>

| <span data-ttu-id="9d110-110">Метод</span><span class="sxs-lookup"><span data-stu-id="9d110-110">Method</span></span>           | <span data-ttu-id="9d110-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9d110-111">Return Type</span></span>    |<span data-ttu-id="9d110-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9d110-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9d110-113">Получение объекта plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="9d110-113">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="9d110-114">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="9d110-114">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="9d110-115">Чтение свойств и отношений объекта **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="9d110-115">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="9d110-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="9d110-116">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="9d110-117">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="9d110-117">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="9d110-118">Обновление объекта **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="9d110-118">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9d110-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d110-119">Properties</span></span>
| <span data-ttu-id="9d110-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d110-120">Property</span></span>     | <span data-ttu-id="9d110-121">Тип</span><span class="sxs-lookup"><span data-stu-id="9d110-121">Type</span></span>   |<span data-ttu-id="9d110-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9d110-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d110-123">checklist</span><span class="sxs-lookup"><span data-stu-id="9d110-123">checklist</span></span>|[<span data-ttu-id="9d110-124">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="9d110-124">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="9d110-125">Коллекция элементов контрольного списка задачи.</span><span class="sxs-lookup"><span data-stu-id="9d110-125">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="9d110-126">описание</span><span class="sxs-lookup"><span data-stu-id="9d110-126">description</span></span>|<span data-ttu-id="9d110-127">Строка</span><span class="sxs-lookup"><span data-stu-id="9d110-127">String</span></span>|<span data-ttu-id="9d110-128">Описание задачи.</span><span class="sxs-lookup"><span data-stu-id="9d110-128">Description of the task</span></span>|
|<span data-ttu-id="9d110-129">id</span><span class="sxs-lookup"><span data-stu-id="9d110-129">id</span></span>|<span data-ttu-id="9d110-130">String</span><span class="sxs-lookup"><span data-stu-id="9d110-130">String</span></span>| <span data-ttu-id="9d110-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d110-131">Read-only.</span></span> <span data-ttu-id="9d110-132">Идентификатор сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="9d110-132">ID of the task details.</span></span> <span data-ttu-id="9d110-133">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="9d110-133">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="9d110-134">[Формат](tasks-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="9d110-134">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="9d110-135">previewType</span><span class="sxs-lookup"><span data-stu-id="9d110-135">previewType</span></span>|<span data-ttu-id="9d110-136">строка</span><span class="sxs-lookup"><span data-stu-id="9d110-136">string</span></span>|<span data-ttu-id="9d110-p105">Устанавливает тип эскиза задачи. Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Если установлено значение `automatic`, отображаемый эскиз выбирается приложением, просматривающим задачу.</span><span class="sxs-lookup"><span data-stu-id="9d110-p105">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="9d110-140">references</span><span class="sxs-lookup"><span data-stu-id="9d110-140">references</span></span>|[<span data-ttu-id="9d110-141">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="9d110-141">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="9d110-142">Коллекция ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="9d110-142">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d110-143">Отношения</span><span class="sxs-lookup"><span data-stu-id="9d110-143">Relationships</span></span>
<span data-ttu-id="9d110-144">Нет</span><span class="sxs-lookup"><span data-stu-id="9d110-144">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9d110-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d110-145">JSON representation</span></span>
<span data-ttu-id="9d110-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d110-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->