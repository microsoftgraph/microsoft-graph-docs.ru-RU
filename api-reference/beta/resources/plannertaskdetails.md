---
title: Тип ресурса plannerTaskDetails
description: Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. С каждым объектом task связан объект details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 579ecdbf43275de90468883d158af725eb1d1734
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512313"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="538d5-104">Тип ресурса plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="538d5-104">plannerTaskDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="538d5-p102">Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. С каждым объектом [task](plannertask.md) связан объект details.</span><span class="sxs-lookup"><span data-stu-id="538d5-p102">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="538d5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="538d5-107">Methods</span></span>

| <span data-ttu-id="538d5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="538d5-108">Method</span></span>           | <span data-ttu-id="538d5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="538d5-109">Return Type</span></span>    |<span data-ttu-id="538d5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="538d5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="538d5-111">Получение объекта plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="538d5-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | <span data-ttu-id="538d5-112">[plannerTaskDetails](plannertaskdetails.md);</span><span class="sxs-lookup"><span data-stu-id="538d5-112">[plannerTaskDetails](plannertaskdetails.md)</span></span> |<span data-ttu-id="538d5-113">Чтение свойств и отношений объекта **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="538d5-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="538d5-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="538d5-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="538d5-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="538d5-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="538d5-116">Обновление объекта **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="538d5-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="538d5-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="538d5-117">Properties</span></span>
| <span data-ttu-id="538d5-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="538d5-118">Property</span></span>     | <span data-ttu-id="538d5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="538d5-119">Type</span></span>   |<span data-ttu-id="538d5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="538d5-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="538d5-121">checklist</span><span class="sxs-lookup"><span data-stu-id="538d5-121">checklist</span></span>|[<span data-ttu-id="538d5-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="538d5-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="538d5-123">Коллекция элементов контрольного списка задачи.</span><span class="sxs-lookup"><span data-stu-id="538d5-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="538d5-124">description</span><span class="sxs-lookup"><span data-stu-id="538d5-124">description</span></span>|<span data-ttu-id="538d5-125">Строка</span><span class="sxs-lookup"><span data-stu-id="538d5-125">String</span></span>|<span data-ttu-id="538d5-126">Описание задачи.</span><span class="sxs-lookup"><span data-stu-id="538d5-126">Description of the task</span></span>|
|<span data-ttu-id="538d5-127">id</span><span class="sxs-lookup"><span data-stu-id="538d5-127">id</span></span>|<span data-ttu-id="538d5-128">String</span><span class="sxs-lookup"><span data-stu-id="538d5-128">String</span></span>| <span data-ttu-id="538d5-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="538d5-129">Read-only.</span></span> <span data-ttu-id="538d5-130">Идентификатор сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="538d5-130">ID of the task details.</span></span> <span data-ttu-id="538d5-131">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="538d5-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="538d5-132">[Формат](tasks-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="538d5-132">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="538d5-133">previewType</span><span class="sxs-lookup"><span data-stu-id="538d5-133">previewType</span></span>|<span data-ttu-id="538d5-134">string</span><span class="sxs-lookup"><span data-stu-id="538d5-134">string</span></span>|<span data-ttu-id="538d5-p104">Устанавливает тип эскиза задачи. Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Если установлено значение `automatic`, отображаемый эскиз выбирается приложением, просматривающим задачу.</span><span class="sxs-lookup"><span data-stu-id="538d5-p104">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="538d5-138">references</span><span class="sxs-lookup"><span data-stu-id="538d5-138">references</span></span>|[<span data-ttu-id="538d5-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="538d5-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="538d5-140">Коллекция ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="538d5-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="538d5-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="538d5-141">Relationships</span></span>
<span data-ttu-id="538d5-142">Нет</span><span class="sxs-lookup"><span data-stu-id="538d5-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="538d5-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="538d5-143">JSON representation</span></span>
<span data-ttu-id="538d5-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="538d5-144">Here is a JSON representation of the resource.</span></span>

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
