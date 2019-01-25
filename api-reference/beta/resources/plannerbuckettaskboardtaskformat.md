---
title: Тип ресурса plannerBucketTaskBoardTaskFormat
description: Ресурс **plannerBucketTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении Buckets на доске задач (представление, предусматривающее упорядочивание по задачам в сегментах, которым назначены). С каждым объектом **task** связан один объект plannerBucketTaskBoardTaskFormat.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: eca8865e54d68fb7b403364b065e642ad61e9276
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526951"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="48f6d-104">Тип ресурса plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="48f6d-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48f6d-p102">Ресурс **plannerBucketTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении Buckets на доске задач (представление, предусматривающее упорядочивание по задачам в сегментах, которым назначены). С каждым объектом [task](plannertask.md) связан один объект **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="48f6d-p102">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="48f6d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="48f6d-107">Methods</span></span>

| <span data-ttu-id="48f6d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="48f6d-108">Method</span></span>           | <span data-ttu-id="48f6d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="48f6d-109">Return Type</span></span>    |<span data-ttu-id="48f6d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="48f6d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48f6d-111">Получение plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="48f6d-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | <span data-ttu-id="48f6d-112">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md);</span><span class="sxs-lookup"><span data-stu-id="48f6d-112">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)</span></span> |<span data-ttu-id="48f6d-113">Считывание свойств и связей объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="48f6d-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="48f6d-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="48f6d-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="48f6d-115">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="48f6d-115">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="48f6d-116">Обновление объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="48f6d-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="48f6d-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="48f6d-117">Properties</span></span>
| <span data-ttu-id="48f6d-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="48f6d-118">Property</span></span>     | <span data-ttu-id="48f6d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="48f6d-119">Type</span></span>   |<span data-ttu-id="48f6d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="48f6d-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48f6d-121">id</span><span class="sxs-lookup"><span data-stu-id="48f6d-121">id</span></span>|<span data-ttu-id="48f6d-122">String</span><span class="sxs-lookup"><span data-stu-id="48f6d-122">String</span></span>| <span data-ttu-id="48f6d-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="48f6d-123">Read-only.</span></span> <span data-ttu-id="48f6d-124">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="48f6d-124">ID of the resource.</span></span> <span data-ttu-id="48f6d-125">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="48f6d-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="48f6d-126">[Формат](tasks-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="48f6d-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="48f6d-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="48f6d-127">orderHint</span></span>|<span data-ttu-id="48f6d-128">String</span><span class="sxs-lookup"><span data-stu-id="48f6d-128">String</span></span>|<span data-ttu-id="48f6d-p104">Указание, используемое для расположения задач в представлении сегментов на доске задач. Используемый формат описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="48f6d-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="48f6d-131">Связи</span><span class="sxs-lookup"><span data-stu-id="48f6d-131">Relationships</span></span>
<span data-ttu-id="48f6d-132">Нет</span><span class="sxs-lookup"><span data-stu-id="48f6d-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="48f6d-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="48f6d-133">JSON representation</span></span>
<span data-ttu-id="48f6d-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48f6d-134">Here is a JSON representation of the resource.</span></span>

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
