---
title: Тип ресурса plannerBucketTaskBoardTaskFormat
description: Ресурс **plannerBucketTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении "сегменты" доски задач (представление, упорядоченное по задачам в сегментах, которым они назначены). Каждой задаче будет назначен один объект **plannerBucketTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: eca8865e54d68fb7b403364b065e642ad61e9276
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457062"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="a3d5b-104">Тип ресурса plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="a3d5b-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3d5b-105">Ресурс **plannerBucketTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении "сегменты" доски задач (представление, упорядоченное по задачам в сегментах, которым они назначены).</span><span class="sxs-lookup"><span data-stu-id="a3d5b-105">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to).</span></span> <span data-ttu-id="a3d5b-106">Каждой [задаче](plannertask.md) будет назначен один объект **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="a3d5b-106">Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="a3d5b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a3d5b-107">Methods</span></span>

| <span data-ttu-id="a3d5b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a3d5b-108">Method</span></span>           | <span data-ttu-id="a3d5b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a3d5b-109">Return Type</span></span>    |<span data-ttu-id="a3d5b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a3d5b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a3d5b-111">Получение объекта plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="a3d5b-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | <span data-ttu-id="a3d5b-112">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md);</span><span class="sxs-lookup"><span data-stu-id="a3d5b-112">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)</span></span> |<span data-ttu-id="a3d5b-113">Чтение свойств и связей объекта **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="a3d5b-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|<span data-ttu-id="a3d5b-114">[обновление](../api/plannerbuckettaskboardtaskformat-update.md);</span><span class="sxs-lookup"><span data-stu-id="a3d5b-114">[Update](../api/plannerbuckettaskboardtaskformat-update.md)</span></span> | <span data-ttu-id="a3d5b-115">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md);</span><span class="sxs-lookup"><span data-stu-id="a3d5b-115">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)</span></span>  |<span data-ttu-id="a3d5b-116">Обновление объекта **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="a3d5b-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a3d5b-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3d5b-117">Properties</span></span>
| <span data-ttu-id="a3d5b-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3d5b-118">Property</span></span>     | <span data-ttu-id="a3d5b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a3d5b-119">Type</span></span>   |<span data-ttu-id="a3d5b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a3d5b-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3d5b-121">id</span><span class="sxs-lookup"><span data-stu-id="a3d5b-121">id</span></span>|<span data-ttu-id="a3d5b-122">String</span><span class="sxs-lookup"><span data-stu-id="a3d5b-122">String</span></span>| <span data-ttu-id="a3d5b-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3d5b-123">Read-only.</span></span> <span data-ttu-id="a3d5b-124">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="a3d5b-124">ID of the resource.</span></span> <span data-ttu-id="a3d5b-125">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="a3d5b-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="a3d5b-126">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="a3d5b-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="a3d5b-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="a3d5b-127">orderHint</span></span>|<span data-ttu-id="a3d5b-128">Строка</span><span class="sxs-lookup"><span data-stu-id="a3d5b-128">String</span></span>|<span data-ttu-id="a3d5b-p104">Указание, используемое для расположения задач в окне "Сегмент" доски задачи. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="a3d5b-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3d5b-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="a3d5b-131">Relationships</span></span>
<span data-ttu-id="a3d5b-132">Нет</span><span class="sxs-lookup"><span data-stu-id="a3d5b-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a3d5b-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3d5b-133">JSON representation</span></span>
<span data-ttu-id="a3d5b-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3d5b-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerbuckettaskboardtaskformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
