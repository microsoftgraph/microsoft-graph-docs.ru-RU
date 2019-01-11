---
title: Тип ресурса plannerBucketTaskBoardTaskFormat
description: Ресурс **plannerBucketTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении Buckets на доске задач (представление, предусматривающее упорядочивание по задачам в сегментах, которым назначены). С каждым объектом task связан один объект **plannerBucketTaskBoardTaskFormat**.
localization_priority: Normal
ms.openlocfilehash: 179f14c2cf0df7e1e4e82f6dbc2cd4ca3de977b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805350"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="adfab-104">Тип ресурса plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="adfab-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="adfab-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="adfab-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adfab-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adfab-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="adfab-p103">Ресурс **plannerBucketTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении Buckets на доске задач (представление, предусматривающее упорядочивание по задачам в сегментах, которым назначены). С каждым объектом [task](plannertask.md) связан один объект **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="adfab-p103">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="adfab-109">Методы</span><span class="sxs-lookup"><span data-stu-id="adfab-109">Methods</span></span>

| <span data-ttu-id="adfab-110">Метод</span><span class="sxs-lookup"><span data-stu-id="adfab-110">Method</span></span>           | <span data-ttu-id="adfab-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="adfab-111">Return Type</span></span>    |<span data-ttu-id="adfab-112">Описание</span><span class="sxs-lookup"><span data-stu-id="adfab-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="adfab-113">Получение plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="adfab-113">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="adfab-114">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="adfab-114">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="adfab-115">Считывание свойств и связей объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="adfab-115">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="adfab-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="adfab-116">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="adfab-117">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="adfab-117">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="adfab-118">Обновление объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="adfab-118">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="adfab-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="adfab-119">Properties</span></span>
| <span data-ttu-id="adfab-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="adfab-120">Property</span></span>     | <span data-ttu-id="adfab-121">Тип</span><span class="sxs-lookup"><span data-stu-id="adfab-121">Type</span></span>   |<span data-ttu-id="adfab-122">Описание</span><span class="sxs-lookup"><span data-stu-id="adfab-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adfab-123">id</span><span class="sxs-lookup"><span data-stu-id="adfab-123">id</span></span>|<span data-ttu-id="adfab-124">Строка</span><span class="sxs-lookup"><span data-stu-id="adfab-124">String</span></span>| <span data-ttu-id="adfab-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="adfab-125">Read-only.</span></span> <span data-ttu-id="adfab-126">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="adfab-126">ID of the resource.</span></span> <span data-ttu-id="adfab-127">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="adfab-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="adfab-128">[Формат](tasks-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="adfab-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="adfab-129">orderHint</span><span class="sxs-lookup"><span data-stu-id="adfab-129">orderHint</span></span>|<span data-ttu-id="adfab-130">Строка</span><span class="sxs-lookup"><span data-stu-id="adfab-130">String</span></span>|<span data-ttu-id="adfab-p105">Указание, используемое для расположения задач в представлении сегментов на доске задач. Используемый формат описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="adfab-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="adfab-133">Связи</span><span class="sxs-lookup"><span data-stu-id="adfab-133">Relationships</span></span>
<span data-ttu-id="adfab-134">Нет</span><span class="sxs-lookup"><span data-stu-id="adfab-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="adfab-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="adfab-135">JSON representation</span></span>
<span data-ttu-id="adfab-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adfab-136">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
