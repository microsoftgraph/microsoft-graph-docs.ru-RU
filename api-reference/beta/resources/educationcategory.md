---
title: Тип ресурса Едукатионкатегори
description: Категория, которая может быть применена к назначениям.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4732bab700ab23869e0463437288b1aa8897aa0e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972791"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="adc3d-103">Тип ресурса Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="adc3d-103">educationCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adc3d-104">Категория, которая может быть применена к назначениям.</span><span class="sxs-lookup"><span data-stu-id="adc3d-104">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="adc3d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="adc3d-105">Methods</span></span>

| <span data-ttu-id="adc3d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="adc3d-106">Method</span></span>           | <span data-ttu-id="adc3d-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="adc3d-107">Return Type</span></span>    |<span data-ttu-id="adc3d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="adc3d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="adc3d-109">Получение Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="adc3d-109">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="adc3d-110">Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="adc3d-110">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="adc3d-111">Получение существующего **едукатионкатегори**.</span><span class="sxs-lookup"><span data-stu-id="adc3d-111">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="adc3d-112">Удаление категории</span><span class="sxs-lookup"><span data-stu-id="adc3d-112">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="adc3d-113">Нет</span><span class="sxs-lookup"><span data-stu-id="adc3d-113">None</span></span> | <span data-ttu-id="adc3d-114">Удаление **едукатионкатегори**.</span><span class="sxs-lookup"><span data-stu-id="adc3d-114">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="adc3d-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="adc3d-115">Properties</span></span>
| <span data-ttu-id="adc3d-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="adc3d-116">Property</span></span>     | <span data-ttu-id="adc3d-117">Тип</span><span class="sxs-lookup"><span data-stu-id="adc3d-117">Type</span></span>   |<span data-ttu-id="adc3d-118">Описание</span><span class="sxs-lookup"><span data-stu-id="adc3d-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adc3d-119">id</span><span class="sxs-lookup"><span data-stu-id="adc3d-119">id</span></span>|<span data-ttu-id="adc3d-120">String</span><span class="sxs-lookup"><span data-stu-id="adc3d-120">String</span></span>|<span data-ttu-id="adc3d-121">Уникальный идентификатор для категории.</span><span class="sxs-lookup"><span data-stu-id="adc3d-121">Unique identifier for the category.</span></span>|
|<span data-ttu-id="adc3d-122">displayName</span><span class="sxs-lookup"><span data-stu-id="adc3d-122">displayName</span></span>|<span data-ttu-id="adc3d-123">Строка</span><span class="sxs-lookup"><span data-stu-id="adc3d-123">String</span></span>|<span data-ttu-id="adc3d-124">Уникальный идентификатор для категории.</span><span class="sxs-lookup"><span data-stu-id="adc3d-124">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="adc3d-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="adc3d-125">JSON representation</span></span>

<span data-ttu-id="adc3d-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adc3d-126">The following is a JSON representation of the resource.</span></span>

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
