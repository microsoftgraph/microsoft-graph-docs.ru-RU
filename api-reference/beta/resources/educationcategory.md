---
title: Тип ресурса Едукатионкатегори
description: Категория, которая может быть применена к назначениям.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 82ad4f009ca76625c148e8a42e58385195466fbb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095543"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="63bf1-103">Тип ресурса Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="63bf1-103">educationCategory resource type</span></span>

<span data-ttu-id="63bf1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63bf1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63bf1-105">Категория, которая может быть применена к назначениям.</span><span class="sxs-lookup"><span data-stu-id="63bf1-105">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="63bf1-106">Методы</span><span class="sxs-lookup"><span data-stu-id="63bf1-106">Methods</span></span>

| <span data-ttu-id="63bf1-107">Метод</span><span class="sxs-lookup"><span data-stu-id="63bf1-107">Method</span></span>           | <span data-ttu-id="63bf1-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="63bf1-108">Return Type</span></span>    |<span data-ttu-id="63bf1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="63bf1-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="63bf1-110">Создание категории</span><span class="sxs-lookup"><span data-stu-id="63bf1-110">Create category</span></span>](../api/educationclass-post-category.md) | [<span data-ttu-id="63bf1-111">едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="63bf1-111">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="63bf1-112">Создание нового **едукатионкатегори**.</span><span class="sxs-lookup"><span data-stu-id="63bf1-112">Create a new **educationCategory**.</span></span>|
|[<span data-ttu-id="63bf1-113">Получение Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="63bf1-113">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="63bf1-114">едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="63bf1-114">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="63bf1-115">Получение существующего **едукатионкатегори**.</span><span class="sxs-lookup"><span data-stu-id="63bf1-115">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="63bf1-116">Удаление категории</span><span class="sxs-lookup"><span data-stu-id="63bf1-116">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="63bf1-117">Нет</span><span class="sxs-lookup"><span data-stu-id="63bf1-117">None</span></span> | <span data-ttu-id="63bf1-118">Удаление **едукатионкатегори**.</span><span class="sxs-lookup"><span data-stu-id="63bf1-118">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="63bf1-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="63bf1-119">Properties</span></span>
| <span data-ttu-id="63bf1-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="63bf1-120">Property</span></span>     | <span data-ttu-id="63bf1-121">Тип</span><span class="sxs-lookup"><span data-stu-id="63bf1-121">Type</span></span>   |<span data-ttu-id="63bf1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="63bf1-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63bf1-123">id</span><span class="sxs-lookup"><span data-stu-id="63bf1-123">id</span></span>|<span data-ttu-id="63bf1-124">Строка</span><span class="sxs-lookup"><span data-stu-id="63bf1-124">String</span></span>|<span data-ttu-id="63bf1-125">Уникальный идентификатор для категории.</span><span class="sxs-lookup"><span data-stu-id="63bf1-125">Unique identifier for the category.</span></span>|
|<span data-ttu-id="63bf1-126">displayName</span><span class="sxs-lookup"><span data-stu-id="63bf1-126">displayName</span></span>|<span data-ttu-id="63bf1-127">Строка</span><span class="sxs-lookup"><span data-stu-id="63bf1-127">String</span></span>|<span data-ttu-id="63bf1-128">Уникальный идентификатор для категории.</span><span class="sxs-lookup"><span data-stu-id="63bf1-128">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63bf1-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="63bf1-129">JSON representation</span></span>

<span data-ttu-id="63bf1-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63bf1-130">The following is a JSON representation of the resource.</span></span>

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


