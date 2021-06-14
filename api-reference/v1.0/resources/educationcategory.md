---
title: тип ресурса educationCategory
description: Категория, которую можно применить к назначениям.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: dc18c74ba7720aed93d58ee974438857f967e23a
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912858"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="68231-103">тип ресурса educationCategory</span><span class="sxs-lookup"><span data-stu-id="68231-103">educationCategory resource type</span></span>

<span data-ttu-id="68231-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68231-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68231-105">Категория, которую можно применить к назначениям.</span><span class="sxs-lookup"><span data-stu-id="68231-105">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="68231-106">Методы</span><span class="sxs-lookup"><span data-stu-id="68231-106">Methods</span></span>

| <span data-ttu-id="68231-107">Метод</span><span class="sxs-lookup"><span data-stu-id="68231-107">Method</span></span>           | <span data-ttu-id="68231-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="68231-108">Return Type</span></span>    |<span data-ttu-id="68231-109">Описание</span><span class="sxs-lookup"><span data-stu-id="68231-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="68231-110">Создание категории</span><span class="sxs-lookup"><span data-stu-id="68231-110">Create category</span></span>](../api/educationclass-post-category.md) | [<span data-ttu-id="68231-111">educationCategory</span><span class="sxs-lookup"><span data-stu-id="68231-111">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="68231-112">Создание нового **образованияCategory**.</span><span class="sxs-lookup"><span data-stu-id="68231-112">Create a new **educationCategory**.</span></span>|
|[<span data-ttu-id="68231-113">Get educationCategory</span><span class="sxs-lookup"><span data-stu-id="68231-113">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="68231-114">educationCategory</span><span class="sxs-lookup"><span data-stu-id="68231-114">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="68231-115">Получите существующее **educationCategory**.</span><span class="sxs-lookup"><span data-stu-id="68231-115">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="68231-116">Удаление категории</span><span class="sxs-lookup"><span data-stu-id="68231-116">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="68231-117">Нет</span><span class="sxs-lookup"><span data-stu-id="68231-117">None</span></span> | <span data-ttu-id="68231-118">Удалить **educationCategory**.</span><span class="sxs-lookup"><span data-stu-id="68231-118">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="68231-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="68231-119">Properties</span></span>
| <span data-ttu-id="68231-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="68231-120">Property</span></span>     | <span data-ttu-id="68231-121">Тип</span><span class="sxs-lookup"><span data-stu-id="68231-121">Type</span></span>   |<span data-ttu-id="68231-122">Описание</span><span class="sxs-lookup"><span data-stu-id="68231-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68231-123">id</span><span class="sxs-lookup"><span data-stu-id="68231-123">id</span></span>|<span data-ttu-id="68231-124">String</span><span class="sxs-lookup"><span data-stu-id="68231-124">String</span></span>|<span data-ttu-id="68231-125">Уникальный идентификатор для категории.</span><span class="sxs-lookup"><span data-stu-id="68231-125">Unique identifier for the category.</span></span>|
|<span data-ttu-id="68231-126">displayName</span><span class="sxs-lookup"><span data-stu-id="68231-126">displayName</span></span>|<span data-ttu-id="68231-127">String</span><span class="sxs-lookup"><span data-stu-id="68231-127">String</span></span>|<span data-ttu-id="68231-128">Уникальный идентификатор для категории.</span><span class="sxs-lookup"><span data-stu-id="68231-128">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68231-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68231-129">JSON representation</span></span>

<span data-ttu-id="68231-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68231-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCategory"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
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


