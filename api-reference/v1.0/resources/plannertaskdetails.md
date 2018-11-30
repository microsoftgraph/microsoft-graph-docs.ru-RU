---
title: Тип ресурса plannerTaskDetails
description: Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. С каждым объектом task связан объект details.
ms.openlocfilehash: 74ba1c5b7c607f30253463e6cfc256fd3119bf45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028206"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="dc57d-104">Тип ресурса plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="dc57d-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="dc57d-p102">Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. С каждым объектом [task](plannertask.md) связан объект details.</span><span class="sxs-lookup"><span data-stu-id="dc57d-p102">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="dc57d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="dc57d-107">Methods</span></span>

| <span data-ttu-id="dc57d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="dc57d-108">Method</span></span>           | <span data-ttu-id="dc57d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dc57d-109">Return Type</span></span>    |<span data-ttu-id="dc57d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dc57d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dc57d-111">Получение объекта plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="dc57d-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="dc57d-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="dc57d-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="dc57d-113">Чтение свойств и отношений объекта **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="dc57d-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="dc57d-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="dc57d-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="dc57d-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="dc57d-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="dc57d-116">Обновление объекта **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="dc57d-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dc57d-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc57d-117">Properties</span></span>
| <span data-ttu-id="dc57d-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc57d-118">Property</span></span>     | <span data-ttu-id="dc57d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="dc57d-119">Type</span></span>   |<span data-ttu-id="dc57d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dc57d-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc57d-121">checklist</span><span class="sxs-lookup"><span data-stu-id="dc57d-121">checklist</span></span>|[<span data-ttu-id="dc57d-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="dc57d-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="dc57d-123">Коллекция элементов контрольного списка задачи.</span><span class="sxs-lookup"><span data-stu-id="dc57d-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="dc57d-124">описание</span><span class="sxs-lookup"><span data-stu-id="dc57d-124">description</span></span>|<span data-ttu-id="dc57d-125">Строка</span><span class="sxs-lookup"><span data-stu-id="dc57d-125">String</span></span>|<span data-ttu-id="dc57d-126">Описание задачи.</span><span class="sxs-lookup"><span data-stu-id="dc57d-126">Description of the task</span></span>|
|<span data-ttu-id="dc57d-127">id</span><span class="sxs-lookup"><span data-stu-id="dc57d-127">id</span></span>|<span data-ttu-id="dc57d-128">String</span><span class="sxs-lookup"><span data-stu-id="dc57d-128">String</span></span>| <span data-ttu-id="dc57d-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc57d-129">Read-only.</span></span> <span data-ttu-id="dc57d-130">Идентификатор сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="dc57d-130">ID of the task details.</span></span> <span data-ttu-id="dc57d-131">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="dc57d-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="dc57d-132">[Формат](planner-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="dc57d-132">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="dc57d-133">previewType</span><span class="sxs-lookup"><span data-stu-id="dc57d-133">previewType</span></span>|<span data-ttu-id="dc57d-134">строка</span><span class="sxs-lookup"><span data-stu-id="dc57d-134">string</span></span>|<span data-ttu-id="dc57d-135">Задается тип предварительного просмотра, который появляется на задачу.</span><span class="sxs-lookup"><span data-stu-id="dc57d-135">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="dc57d-136">Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="dc57d-136">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="dc57d-137">Если параметр имеет значение `automatic` отображаемой предварительного просмотра выбирается по приложению, просмотр задачи.</span><span class="sxs-lookup"><span data-stu-id="dc57d-137">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="dc57d-138">references</span><span class="sxs-lookup"><span data-stu-id="dc57d-138">references</span></span>|[<span data-ttu-id="dc57d-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="dc57d-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="dc57d-140">Коллекция ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="dc57d-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc57d-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="dc57d-141">Relationships</span></span>
<span data-ttu-id="dc57d-142">Нет</span><span class="sxs-lookup"><span data-stu-id="dc57d-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dc57d-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc57d-143">JSON representation</span></span>
<span data-ttu-id="dc57d-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc57d-144">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
