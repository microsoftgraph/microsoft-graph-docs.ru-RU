---
title: Тип ресурса plannerTaskDetails
description: Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. С каждым объектом task связан объект details.
localization_priority: Normal
ms.openlocfilehash: 0bec5b47d1472eae43906841c5074e4080672817
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888167"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="b88bb-104">Тип ресурса plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="b88bb-104">plannerTaskDetails resource type</span></span>

> <span data-ttu-id="b88bb-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b88bb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b88bb-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b88bb-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b88bb-p103">Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. С каждым объектом [task](plannertask.md) связан объект details.</span><span class="sxs-lookup"><span data-stu-id="b88bb-p103">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="b88bb-109">Методы</span><span class="sxs-lookup"><span data-stu-id="b88bb-109">Methods</span></span>

| <span data-ttu-id="b88bb-110">Метод</span><span class="sxs-lookup"><span data-stu-id="b88bb-110">Method</span></span>           | <span data-ttu-id="b88bb-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b88bb-111">Return Type</span></span>    |<span data-ttu-id="b88bb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b88bb-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b88bb-113">Получение объекта plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="b88bb-113">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="b88bb-114">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="b88bb-114">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="b88bb-115">Чтение свойств и отношений объекта **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="b88bb-115">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="b88bb-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="b88bb-116">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="b88bb-117">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="b88bb-117">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="b88bb-118">Обновление объекта **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="b88bb-118">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b88bb-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="b88bb-119">Properties</span></span>
| <span data-ttu-id="b88bb-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="b88bb-120">Property</span></span>     | <span data-ttu-id="b88bb-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b88bb-121">Type</span></span>   |<span data-ttu-id="b88bb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b88bb-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b88bb-123">checklist</span><span class="sxs-lookup"><span data-stu-id="b88bb-123">checklist</span></span>|[<span data-ttu-id="b88bb-124">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="b88bb-124">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="b88bb-125">Коллекция элементов контрольного списка задачи.</span><span class="sxs-lookup"><span data-stu-id="b88bb-125">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="b88bb-126">описание</span><span class="sxs-lookup"><span data-stu-id="b88bb-126">description</span></span>|<span data-ttu-id="b88bb-127">Строка</span><span class="sxs-lookup"><span data-stu-id="b88bb-127">String</span></span>|<span data-ttu-id="b88bb-128">Описание задачи.</span><span class="sxs-lookup"><span data-stu-id="b88bb-128">Description of the task</span></span>|
|<span data-ttu-id="b88bb-129">id</span><span class="sxs-lookup"><span data-stu-id="b88bb-129">id</span></span>|<span data-ttu-id="b88bb-130">Строка</span><span class="sxs-lookup"><span data-stu-id="b88bb-130">String</span></span>| <span data-ttu-id="b88bb-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b88bb-131">Read-only.</span></span> <span data-ttu-id="b88bb-132">Идентификатор сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="b88bb-132">ID of the task details.</span></span> <span data-ttu-id="b88bb-133">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="b88bb-133">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="b88bb-134">[Формат](tasks-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="b88bb-134">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="b88bb-135">previewType</span><span class="sxs-lookup"><span data-stu-id="b88bb-135">previewType</span></span>|<span data-ttu-id="b88bb-136">строка</span><span class="sxs-lookup"><span data-stu-id="b88bb-136">string</span></span>|<span data-ttu-id="b88bb-p105">Устанавливает тип эскиза задачи. Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Если установлено значение `automatic`, отображаемый эскиз выбирается приложением, просматривающим задачу.</span><span class="sxs-lookup"><span data-stu-id="b88bb-p105">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="b88bb-140">references</span><span class="sxs-lookup"><span data-stu-id="b88bb-140">references</span></span>|[<span data-ttu-id="b88bb-141">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="b88bb-141">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="b88bb-142">Коллекция ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="b88bb-142">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b88bb-143">Отношения</span><span class="sxs-lookup"><span data-stu-id="b88bb-143">Relationships</span></span>
<span data-ttu-id="b88bb-144">Нет</span><span class="sxs-lookup"><span data-stu-id="b88bb-144">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b88bb-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b88bb-145">JSON representation</span></span>
<span data-ttu-id="b88bb-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b88bb-146">Here is a JSON representation of the resource.</span></span>

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
