---
title: Тип ресурса plannerTaskDetails
description: Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. Каждый объект Task содержит объект Details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d22c932989b9c0d21350842babd9b4bbf420124c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035170"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="df590-104">Тип ресурса plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="df590-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="df590-105">Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="df590-105">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="df590-106">Каждый объект [Task](plannertask.md) содержит объект Details.</span><span class="sxs-lookup"><span data-stu-id="df590-106">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="df590-107">Методы</span><span class="sxs-lookup"><span data-stu-id="df590-107">Methods</span></span>

| <span data-ttu-id="df590-108">Метод</span><span class="sxs-lookup"><span data-stu-id="df590-108">Method</span></span>           | <span data-ttu-id="df590-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="df590-109">Return Type</span></span>    |<span data-ttu-id="df590-110">Описание</span><span class="sxs-lookup"><span data-stu-id="df590-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="df590-111">Получение объекта plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="df590-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | <span data-ttu-id="df590-112">[plannerTaskDetails](plannertaskdetails.md);</span><span class="sxs-lookup"><span data-stu-id="df590-112">[plannerTaskDetails](plannertaskdetails.md)</span></span> |<span data-ttu-id="df590-113">Чтение свойств и связей объекта **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="df590-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|<span data-ttu-id="df590-114">[обновление](../api/plannertaskdetails-update.md);</span><span class="sxs-lookup"><span data-stu-id="df590-114">[Update](../api/plannertaskdetails-update.md)</span></span> | <span data-ttu-id="df590-115">[plannerTaskDetails](plannertaskdetails.md);</span><span class="sxs-lookup"><span data-stu-id="df590-115">[plannerTaskDetails](plannertaskdetails.md)</span></span>    |<span data-ttu-id="df590-116">Обновление объекта **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="df590-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="df590-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="df590-117">Properties</span></span>
| <span data-ttu-id="df590-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="df590-118">Property</span></span>     | <span data-ttu-id="df590-119">Тип</span><span class="sxs-lookup"><span data-stu-id="df590-119">Type</span></span>   |<span data-ttu-id="df590-120">Описание</span><span class="sxs-lookup"><span data-stu-id="df590-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df590-121">checklist</span><span class="sxs-lookup"><span data-stu-id="df590-121">checklist</span></span>|[<span data-ttu-id="df590-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="df590-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="df590-123">Коллекция элементов контрольного списка задачи.</span><span class="sxs-lookup"><span data-stu-id="df590-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="df590-124">description</span><span class="sxs-lookup"><span data-stu-id="df590-124">description</span></span>|<span data-ttu-id="df590-125">Строка</span><span class="sxs-lookup"><span data-stu-id="df590-125">String</span></span>|<span data-ttu-id="df590-126">Описание задачи.</span><span class="sxs-lookup"><span data-stu-id="df590-126">Description of the task</span></span>|
|<span data-ttu-id="df590-127">id</span><span class="sxs-lookup"><span data-stu-id="df590-127">id</span></span>|<span data-ttu-id="df590-128">Строка</span><span class="sxs-lookup"><span data-stu-id="df590-128">String</span></span>| <span data-ttu-id="df590-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="df590-129">Read-only.</span></span> <span data-ttu-id="df590-130">Идентификатор сведений о задаче.</span><span class="sxs-lookup"><span data-stu-id="df590-130">ID of the task details.</span></span> <span data-ttu-id="df590-131">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="df590-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="df590-132">[Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="df590-132">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="df590-133">previewType</span><span class="sxs-lookup"><span data-stu-id="df590-133">previewType</span></span>|<span data-ttu-id="df590-134">string</span><span class="sxs-lookup"><span data-stu-id="df590-134">string</span></span>|<span data-ttu-id="df590-135">Устанавливает тип предварительного просмотра задачи.</span><span class="sxs-lookup"><span data-stu-id="df590-135">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="df590-136">Допустимые значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="df590-136">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="df590-137">`automatic` Если выбран отображаемый предварительный просмотр, то приложение просматривает задачу.</span><span class="sxs-lookup"><span data-stu-id="df590-137">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="df590-138">references</span><span class="sxs-lookup"><span data-stu-id="df590-138">references</span></span>|[<span data-ttu-id="df590-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="df590-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="df590-140">Коллекция ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="df590-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df590-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="df590-141">Relationships</span></span>
<span data-ttu-id="df590-142">Нет</span><span class="sxs-lookup"><span data-stu-id="df590-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="df590-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="df590-143">JSON representation</span></span>
<span data-ttu-id="df590-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df590-144">Here is a JSON representation of the resource.</span></span>

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
