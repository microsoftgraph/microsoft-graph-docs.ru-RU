---
title: Тип ресурса Едукатионкатегори
description: Категория, которая может быть применена к назначениям.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: dd9eccac3a1b6b1bdc3b0eca4c87b5e29e2135a9
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536178"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="eb381-103">Тип ресурса Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="eb381-103">educationCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb381-104">Категория, которая может быть применена к назначениям.</span><span class="sxs-lookup"><span data-stu-id="eb381-104">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="eb381-105">Методы</span><span class="sxs-lookup"><span data-stu-id="eb381-105">Methods</span></span>

| <span data-ttu-id="eb381-106">Метод</span><span class="sxs-lookup"><span data-stu-id="eb381-106">Method</span></span>           | <span data-ttu-id="eb381-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eb381-107">Return Type</span></span>    |<span data-ttu-id="eb381-108">Описание</span><span class="sxs-lookup"><span data-stu-id="eb381-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eb381-109">Получение Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="eb381-109">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="eb381-110">Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="eb381-110">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="eb381-111">Получение существующего **едукатионкатегори**.</span><span class="sxs-lookup"><span data-stu-id="eb381-111">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="eb381-112">Удаление категории</span><span class="sxs-lookup"><span data-stu-id="eb381-112">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="eb381-113">Нет</span><span class="sxs-lookup"><span data-stu-id="eb381-113">None</span></span> | <span data-ttu-id="eb381-114">Удаление **едукатионкатегори**.</span><span class="sxs-lookup"><span data-stu-id="eb381-114">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="eb381-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb381-115">Properties</span></span>
| <span data-ttu-id="eb381-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb381-116">Property</span></span>     | <span data-ttu-id="eb381-117">Тип</span><span class="sxs-lookup"><span data-stu-id="eb381-117">Type</span></span>   |<span data-ttu-id="eb381-118">Описание</span><span class="sxs-lookup"><span data-stu-id="eb381-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb381-119">id</span><span class="sxs-lookup"><span data-stu-id="eb381-119">id</span></span>|<span data-ttu-id="eb381-120">String</span><span class="sxs-lookup"><span data-stu-id="eb381-120">String</span></span>|<span data-ttu-id="eb381-121">Уникальный идентификатор для категории.</span><span class="sxs-lookup"><span data-stu-id="eb381-121">Unique identifier for the category.</span></span>|
|<span data-ttu-id="eb381-122">displayName</span><span class="sxs-lookup"><span data-stu-id="eb381-122">displayName</span></span>|<span data-ttu-id="eb381-123">Строка</span><span class="sxs-lookup"><span data-stu-id="eb381-123">String</span></span>|<span data-ttu-id="eb381-124">Уникальный идентификатор для категории.</span><span class="sxs-lookup"><span data-stu-id="eb381-124">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb381-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb381-125">JSON representation</span></span>

<span data-ttu-id="eb381-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb381-126">The following is a JSON representation of the resource.</span></span>

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
