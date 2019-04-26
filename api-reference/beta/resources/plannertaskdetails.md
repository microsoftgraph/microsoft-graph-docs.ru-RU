---
title: Тип ресурса plannerTaskDetails
description: Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. Каждый объект Task содержит объект Details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 579ecdbf43275de90468883d158af725eb1d1734
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563616"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="0c9e5-104">Тип ресурса plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="0c9e5-104">plannerTaskDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c9e5-105">Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="0c9e5-105">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="0c9e5-106">Каждый объект [Task](plannertask.md) содержит объект Details.</span><span class="sxs-lookup"><span data-stu-id="0c9e5-106">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="0c9e5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0c9e5-107">Methods</span></span>

| <span data-ttu-id="0c9e5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="0c9e5-108">Method</span></span>           | <span data-ttu-id="0c9e5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0c9e5-109">Return Type</span></span>    |<span data-ttu-id="0c9e5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0c9e5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0c9e5-111">Получение объекта plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="0c9e5-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | <span data-ttu-id="0c9e5-112">[plannerTaskDetails](plannertaskdetails.md);</span><span class="sxs-lookup"><span data-stu-id="0c9e5-112">[plannerTaskDetails](plannertaskdetails.md)</span></span> |<span data-ttu-id="0c9e5-113">Чтение свойств и связей объекта **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="0c9e5-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="0c9e5-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="0c9e5-114">Update</span></span>](../api/plannertaskdetails-update.md) | <span data-ttu-id="0c9e5-115">[plannerTaskDetails](plannertaskdetails.md);</span><span class="sxs-lookup"><span data-stu-id="0c9e5-115">[plannerTaskDetails](plannertaskdetails.md)</span></span>    |<span data-ttu-id="0c9e5-116">Обновление объекта **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="0c9e5-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0c9e5-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c9e5-117">Properties</span></span>
| <span data-ttu-id="0c9e5-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c9e5-118">Property</span></span>     | <span data-ttu-id="0c9e5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0c9e5-119">Type</span></span>   |<span data-ttu-id="0c9e5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0c9e5-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c9e5-121">checklist</span><span class="sxs-lookup"><span data-stu-id="0c9e5-121">checklist</span></span>|[<span data-ttu-id="0c9e5-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="0c9e5-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="0c9e5-123">Коллекция элементов контрольного списка задачи.</span><span class="sxs-lookup"><span data-stu-id="0c9e5-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="0c9e5-124">description</span><span class="sxs-lookup"><span data-stu-id="0c9e5-124">description</span></span>|<span data-ttu-id="0c9e5-125">String</span><span class="sxs-lookup"><span data-stu-id="0c9e5-125">String</span></span>|<span data-ttu-id="0c9e5-126">Описание задачи.</span><span class="sxs-lookup"><span data-stu-id="0c9e5-126">Description of the task</span></span>|
|<span data-ttu-id="0c9e5-127">id</span><span class="sxs-lookup"><span data-stu-id="0c9e5-127">id</span></span>|<span data-ttu-id="0c9e5-128">String</span><span class="sxs-lookup"><span data-stu-id="0c9e5-128">String</span></span>| <span data-ttu-id="0c9e5-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c9e5-129">Read-only.</span></span> <span data-ttu-id="0c9e5-130">Идентификатор сведений о задаче.</span><span class="sxs-lookup"><span data-stu-id="0c9e5-130">ID of the task details.</span></span> <span data-ttu-id="0c9e5-131">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="0c9e5-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="0c9e5-132">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="0c9e5-132">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="0c9e5-133">previewType</span><span class="sxs-lookup"><span data-stu-id="0c9e5-133">previewType</span></span>|<span data-ttu-id="0c9e5-134">string</span><span class="sxs-lookup"><span data-stu-id="0c9e5-134">string</span></span>|<span data-ttu-id="0c9e5-p104">Устанавливает тип эскиза задачи. Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Если установлено значение `automatic`, отображаемый эскиз выбирается приложением, просматривающим задачу.</span><span class="sxs-lookup"><span data-stu-id="0c9e5-p104">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="0c9e5-138">references</span><span class="sxs-lookup"><span data-stu-id="0c9e5-138">references</span></span>|[<span data-ttu-id="0c9e5-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="0c9e5-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="0c9e5-140">Коллекция ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="0c9e5-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c9e5-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="0c9e5-141">Relationships</span></span>
<span data-ttu-id="0c9e5-142">Нет</span><span class="sxs-lookup"><span data-stu-id="0c9e5-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0c9e5-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c9e5-143">JSON representation</span></span>
<span data-ttu-id="0c9e5-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c9e5-144">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannertaskdetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
