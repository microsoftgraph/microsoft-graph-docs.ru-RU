---
title: Тип ресурса plannerBucketTaskBoardTaskFormat
description: Ресурс **plannerBucketTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении Buckets на доске задач (представление, предусматривающее упорядочивание по задачам в сегментах, которым назначены). С каждым объектом task связан один объект **plannerBucketTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: ea557bad20aa0fd10a73e71902b959913e8fff12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986196"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="88e91-104">Тип ресурса plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="88e91-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="88e91-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="88e91-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88e91-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88e91-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="88e91-p103">Ресурс **plannerBucketTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении Buckets на доске задач (представление, предусматривающее упорядочивание по задачам в сегментах, которым назначены). С каждым объектом [task](plannertask.md) связан один объект **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="88e91-p103">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="88e91-109">Методы</span><span class="sxs-lookup"><span data-stu-id="88e91-109">Methods</span></span>

| <span data-ttu-id="88e91-110">Метод</span><span class="sxs-lookup"><span data-stu-id="88e91-110">Method</span></span>           | <span data-ttu-id="88e91-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="88e91-111">Return Type</span></span>    |<span data-ttu-id="88e91-112">Описание</span><span class="sxs-lookup"><span data-stu-id="88e91-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="88e91-113">Получение plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="88e91-113">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="88e91-114">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="88e91-114">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="88e91-115">Считывание свойств и связей объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="88e91-115">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="88e91-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="88e91-116">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="88e91-117">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="88e91-117">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="88e91-118">Обновление объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="88e91-118">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="88e91-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="88e91-119">Properties</span></span>
| <span data-ttu-id="88e91-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="88e91-120">Property</span></span>     | <span data-ttu-id="88e91-121">Тип</span><span class="sxs-lookup"><span data-stu-id="88e91-121">Type</span></span>   |<span data-ttu-id="88e91-122">Описание</span><span class="sxs-lookup"><span data-stu-id="88e91-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88e91-123">id</span><span class="sxs-lookup"><span data-stu-id="88e91-123">id</span></span>|<span data-ttu-id="88e91-124">Строка</span><span class="sxs-lookup"><span data-stu-id="88e91-124">String</span></span>| <span data-ttu-id="88e91-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88e91-125">Read-only.</span></span> <span data-ttu-id="88e91-126">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="88e91-126">ID of the resource.</span></span> <span data-ttu-id="88e91-127">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="88e91-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="88e91-128">[Формат](tasks-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="88e91-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="88e91-129">orderHint</span><span class="sxs-lookup"><span data-stu-id="88e91-129">orderHint</span></span>|<span data-ttu-id="88e91-130">Строка</span><span class="sxs-lookup"><span data-stu-id="88e91-130">String</span></span>|<span data-ttu-id="88e91-p105">Указание, используемое для расположения задач в представлении сегментов на доске задач. Используемый формат описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="88e91-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="88e91-133">Связи</span><span class="sxs-lookup"><span data-stu-id="88e91-133">Relationships</span></span>
<span data-ttu-id="88e91-134">Нет</span><span class="sxs-lookup"><span data-stu-id="88e91-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="88e91-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88e91-135">JSON representation</span></span>
<span data-ttu-id="88e91-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88e91-136">Here is a JSON representation of the resource.</span></span>

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
