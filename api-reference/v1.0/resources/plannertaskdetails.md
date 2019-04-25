---
title: Тип ресурса plannerTaskDetails
description: Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. Каждый объект Task содержит объект Details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 75e17200dc52fff385c7be8fb0269a3da20464b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534327"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="3b59e-104">Тип ресурса plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="3b59e-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="3b59e-105">Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="3b59e-105">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="3b59e-106">Каждый объект [Task](plannertask.md) содержит объект Details.</span><span class="sxs-lookup"><span data-stu-id="3b59e-106">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="3b59e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3b59e-107">Methods</span></span>

| <span data-ttu-id="3b59e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="3b59e-108">Method</span></span>           | <span data-ttu-id="3b59e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3b59e-109">Return Type</span></span>    |<span data-ttu-id="3b59e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3b59e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b59e-111">Получение объекта plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="3b59e-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | <span data-ttu-id="3b59e-112">[plannerTaskDetails](plannertaskdetails.md);</span><span class="sxs-lookup"><span data-stu-id="3b59e-112">[plannerTaskDetails](plannertaskdetails.md)</span></span> |<span data-ttu-id="3b59e-113">Чтение свойств и связей объекта **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="3b59e-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="3b59e-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="3b59e-114">Update</span></span>](../api/plannertaskdetails-update.md) | <span data-ttu-id="3b59e-115">[plannerTaskDetails](plannertaskdetails.md);</span><span class="sxs-lookup"><span data-stu-id="3b59e-115">[plannerTaskDetails](plannertaskdetails.md)</span></span>    |<span data-ttu-id="3b59e-116">Обновление объекта **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="3b59e-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3b59e-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b59e-117">Properties</span></span>
| <span data-ttu-id="3b59e-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b59e-118">Property</span></span>     | <span data-ttu-id="3b59e-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3b59e-119">Type</span></span>   |<span data-ttu-id="3b59e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3b59e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b59e-121">checklist</span><span class="sxs-lookup"><span data-stu-id="3b59e-121">checklist</span></span>|[<span data-ttu-id="3b59e-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="3b59e-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="3b59e-123">Коллекция элементов контрольного списка задачи.</span><span class="sxs-lookup"><span data-stu-id="3b59e-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="3b59e-124">description</span><span class="sxs-lookup"><span data-stu-id="3b59e-124">description</span></span>|<span data-ttu-id="3b59e-125">String</span><span class="sxs-lookup"><span data-stu-id="3b59e-125">String</span></span>|<span data-ttu-id="3b59e-126">Описание задачи.</span><span class="sxs-lookup"><span data-stu-id="3b59e-126">Description of the task</span></span>|
|<span data-ttu-id="3b59e-127">id</span><span class="sxs-lookup"><span data-stu-id="3b59e-127">id</span></span>|<span data-ttu-id="3b59e-128">String</span><span class="sxs-lookup"><span data-stu-id="3b59e-128">String</span></span>| <span data-ttu-id="3b59e-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b59e-129">Read-only.</span></span> <span data-ttu-id="3b59e-130">Идентификатор сведений о задаче.</span><span class="sxs-lookup"><span data-stu-id="3b59e-130">ID of the task details.</span></span> <span data-ttu-id="3b59e-131">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="3b59e-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="3b59e-132">[Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="3b59e-132">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="3b59e-133">previewType</span><span class="sxs-lookup"><span data-stu-id="3b59e-133">previewType</span></span>|<span data-ttu-id="3b59e-134">string</span><span class="sxs-lookup"><span data-stu-id="3b59e-134">string</span></span>|<span data-ttu-id="3b59e-135">Устанавливает тип предварительного просмотра задачи.</span><span class="sxs-lookup"><span data-stu-id="3b59e-135">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="3b59e-136">Допустимые значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="3b59e-136">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="3b59e-137">`automatic` Если выбран отображаемый предварительный просмотр, то приложение просматривает задачу.</span><span class="sxs-lookup"><span data-stu-id="3b59e-137">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="3b59e-138">references</span><span class="sxs-lookup"><span data-stu-id="3b59e-138">references</span></span>|[<span data-ttu-id="3b59e-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="3b59e-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="3b59e-140">Коллекция ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="3b59e-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b59e-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="3b59e-141">Relationships</span></span>
<span data-ttu-id="3b59e-142">Нет</span><span class="sxs-lookup"><span data-stu-id="3b59e-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3b59e-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3b59e-143">JSON representation</span></span>
<span data-ttu-id="3b59e-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b59e-144">Here is a JSON representation of the resource.</span></span>

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
