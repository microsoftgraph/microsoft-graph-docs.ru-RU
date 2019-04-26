---
title: Тип ресурса Едукатионкатегори
description: Категория, которая может быть применена к назначениям.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bf5ee33ec7d217c0bc4c6e4d35666d6e9f34dadb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340604"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="589a2-103">Тип ресурса Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="589a2-103">educationCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="589a2-104">Категория, которая может быть применена к назначениям.</span><span class="sxs-lookup"><span data-stu-id="589a2-104">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="589a2-105">Методы</span><span class="sxs-lookup"><span data-stu-id="589a2-105">Methods</span></span>

| <span data-ttu-id="589a2-106">Метод</span><span class="sxs-lookup"><span data-stu-id="589a2-106">Method</span></span>           | <span data-ttu-id="589a2-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="589a2-107">Return Type</span></span>    |<span data-ttu-id="589a2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="589a2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="589a2-109">Получение Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="589a2-109">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="589a2-110">Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="589a2-110">educationCategory</span></span>](educationCategory.md) | <span data-ttu-id="589a2-111">Получение существующего **едукатионкатегори**.</span><span class="sxs-lookup"><span data-stu-id="589a2-111">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="589a2-112">Удаление категории</span><span class="sxs-lookup"><span data-stu-id="589a2-112">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="589a2-113">Нет</span><span class="sxs-lookup"><span data-stu-id="589a2-113">None</span></span> | <span data-ttu-id="589a2-114">Удаление **едукатионкатегори**.</span><span class="sxs-lookup"><span data-stu-id="589a2-114">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="589a2-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="589a2-115">Properties</span></span>
| <span data-ttu-id="589a2-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="589a2-116">Property</span></span>     | <span data-ttu-id="589a2-117">Тип</span><span class="sxs-lookup"><span data-stu-id="589a2-117">Type</span></span>   |<span data-ttu-id="589a2-118">Описание</span><span class="sxs-lookup"><span data-stu-id="589a2-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="589a2-119">id</span><span class="sxs-lookup"><span data-stu-id="589a2-119">id</span></span>|<span data-ttu-id="589a2-120">String</span><span class="sxs-lookup"><span data-stu-id="589a2-120">String</span></span>|<span data-ttu-id="589a2-121">Уникальный идентификатор для категории.</span><span class="sxs-lookup"><span data-stu-id="589a2-121">Unique identifier for the category.</span></span>|
|<span data-ttu-id="589a2-122">displayName</span><span class="sxs-lookup"><span data-stu-id="589a2-122">displayName</span></span>|<span data-ttu-id="589a2-123">String</span><span class="sxs-lookup"><span data-stu-id="589a2-123">String</span></span>|<span data-ttu-id="589a2-124">Уникальный идентификатор для категории.</span><span class="sxs-lookup"><span data-stu-id="589a2-124">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="589a2-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="589a2-125">JSON representation</span></span>

<span data-ttu-id="589a2-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="589a2-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCategory"
}-->

```json
{
  "id": "String (timestamp)",
  "displayName": "String (timestamp)",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
