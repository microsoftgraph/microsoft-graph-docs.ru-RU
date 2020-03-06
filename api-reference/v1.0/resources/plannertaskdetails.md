---
title: Тип ресурса plannerTaskDetails
description: Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. Каждый объект Task содержит объект Details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 4dda174401ebf3435c7a190a3f92167ac6b47c0d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533972"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="364e2-104">Тип ресурса plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="364e2-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="364e2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="364e2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="364e2-106">Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="364e2-106">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="364e2-107">Каждый объект [Task](plannertask.md) содержит объект Details.</span><span class="sxs-lookup"><span data-stu-id="364e2-107">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="364e2-108">Методы</span><span class="sxs-lookup"><span data-stu-id="364e2-108">Methods</span></span>

| <span data-ttu-id="364e2-109">Метод</span><span class="sxs-lookup"><span data-stu-id="364e2-109">Method</span></span>           | <span data-ttu-id="364e2-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="364e2-110">Return Type</span></span>    |<span data-ttu-id="364e2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="364e2-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="364e2-112">Получение объекта plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="364e2-112">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | <span data-ttu-id="364e2-113">[plannerTaskDetails](plannertaskdetails.md);</span><span class="sxs-lookup"><span data-stu-id="364e2-113">[plannerTaskDetails](plannertaskdetails.md)</span></span> |<span data-ttu-id="364e2-114">Чтение свойств и связей объекта **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="364e2-114">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="364e2-115">Обновление</span><span class="sxs-lookup"><span data-stu-id="364e2-115">Update</span></span>](../api/plannertaskdetails-update.md) | <span data-ttu-id="364e2-116">[plannerTaskDetails](plannertaskdetails.md);</span><span class="sxs-lookup"><span data-stu-id="364e2-116">[plannerTaskDetails](plannertaskdetails.md)</span></span>    |<span data-ttu-id="364e2-117">Обновление объекта **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="364e2-117">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="364e2-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="364e2-118">Properties</span></span>
| <span data-ttu-id="364e2-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="364e2-119">Property</span></span>     | <span data-ttu-id="364e2-120">Тип</span><span class="sxs-lookup"><span data-stu-id="364e2-120">Type</span></span>   |<span data-ttu-id="364e2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="364e2-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="364e2-122">checklist</span><span class="sxs-lookup"><span data-stu-id="364e2-122">checklist</span></span>|[<span data-ttu-id="364e2-123">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="364e2-123">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="364e2-124">Коллекция элементов контрольного списка задачи.</span><span class="sxs-lookup"><span data-stu-id="364e2-124">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="364e2-125">description</span><span class="sxs-lookup"><span data-stu-id="364e2-125">description</span></span>|<span data-ttu-id="364e2-126">Строка</span><span class="sxs-lookup"><span data-stu-id="364e2-126">String</span></span>|<span data-ttu-id="364e2-127">Описание задачи.</span><span class="sxs-lookup"><span data-stu-id="364e2-127">Description of the task</span></span>|
|<span data-ttu-id="364e2-128">id</span><span class="sxs-lookup"><span data-stu-id="364e2-128">id</span></span>|<span data-ttu-id="364e2-129">Строка</span><span class="sxs-lookup"><span data-stu-id="364e2-129">String</span></span>| <span data-ttu-id="364e2-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="364e2-130">Read-only.</span></span> <span data-ttu-id="364e2-131">Идентификатор сведений о задаче.</span><span class="sxs-lookup"><span data-stu-id="364e2-131">ID of the task details.</span></span> <span data-ttu-id="364e2-132">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="364e2-132">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="364e2-133">[Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="364e2-133">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="364e2-134">previewType</span><span class="sxs-lookup"><span data-stu-id="364e2-134">previewType</span></span>|<span data-ttu-id="364e2-135">string</span><span class="sxs-lookup"><span data-stu-id="364e2-135">string</span></span>|<span data-ttu-id="364e2-136">Устанавливает тип предварительного просмотра задачи.</span><span class="sxs-lookup"><span data-stu-id="364e2-136">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="364e2-137">Допустимые значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="364e2-137">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="364e2-138">`automatic` Если выбран отображаемый предварительный просмотр, то приложение просматривает задачу.</span><span class="sxs-lookup"><span data-stu-id="364e2-138">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="364e2-139">references</span><span class="sxs-lookup"><span data-stu-id="364e2-139">references</span></span>|[<span data-ttu-id="364e2-140">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="364e2-140">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="364e2-141">Коллекция ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="364e2-141">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="364e2-142">Связи</span><span class="sxs-lookup"><span data-stu-id="364e2-142">Relationships</span></span>
<span data-ttu-id="364e2-143">Нет</span><span class="sxs-lookup"><span data-stu-id="364e2-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="364e2-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="364e2-144">JSON representation</span></span>
<span data-ttu-id="364e2-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="364e2-145">Here is a JSON representation of the resource.</span></span>

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
