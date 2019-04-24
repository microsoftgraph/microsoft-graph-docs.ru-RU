---
title: Тип ресурса Едукатионкатегори
description: Категория, которая может быть применена к назначениям.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 928f37b4d29a4443c947bd92bf4a71f9f8a05f59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507320"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="a790b-103">Тип ресурса Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="a790b-103">educationCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a790b-104">Категория, которая может быть применена к назначениям.</span><span class="sxs-lookup"><span data-stu-id="a790b-104">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="a790b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="a790b-105">Methods</span></span>

| <span data-ttu-id="a790b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="a790b-106">Method</span></span>           | <span data-ttu-id="a790b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a790b-107">Return Type</span></span>    |<span data-ttu-id="a790b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a790b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a790b-109">Получение Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="a790b-109">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="a790b-110">Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="a790b-110">educationCategory</span></span>](educationCategory.md) | <span data-ttu-id="a790b-111">Получение существующего **едукатионкатегори**.</span><span class="sxs-lookup"><span data-stu-id="a790b-111">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="a790b-112">Удаление категории</span><span class="sxs-lookup"><span data-stu-id="a790b-112">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="a790b-113">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="a790b-113">None</span></span> | <span data-ttu-id="a790b-114">Удаление **едукатионкатегори**.</span><span class="sxs-lookup"><span data-stu-id="a790b-114">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="a790b-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="a790b-115">Properties</span></span>
| <span data-ttu-id="a790b-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="a790b-116">Property</span></span>     | <span data-ttu-id="a790b-117">Тип</span><span class="sxs-lookup"><span data-stu-id="a790b-117">Type</span></span>   |<span data-ttu-id="a790b-118">Описание</span><span class="sxs-lookup"><span data-stu-id="a790b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a790b-119">id</span><span class="sxs-lookup"><span data-stu-id="a790b-119">id</span></span>|<span data-ttu-id="a790b-120">String</span><span class="sxs-lookup"><span data-stu-id="a790b-120">String</span></span>|<span data-ttu-id="a790b-121">Уникальный идентификатор для категории.</span><span class="sxs-lookup"><span data-stu-id="a790b-121">Unique identifier for the category.</span></span>|
|<span data-ttu-id="a790b-122">displayName</span><span class="sxs-lookup"><span data-stu-id="a790b-122">displayName</span></span>|<span data-ttu-id="a790b-123">String</span><span class="sxs-lookup"><span data-stu-id="a790b-123">String</span></span>|<span data-ttu-id="a790b-124">Уникальный идентификатор для категории.</span><span class="sxs-lookup"><span data-stu-id="a790b-124">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a790b-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a790b-125">JSON representation</span></span>

<span data-ttu-id="a790b-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a790b-126">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationcategory.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
