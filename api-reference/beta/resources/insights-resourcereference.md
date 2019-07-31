---
title: Тип ресурса Ресаурцереференце
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 06a8d99ba01a8a3fd3d171b800345f81b0819de0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005725"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="7ba64-103">Тип ресурса Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="7ba64-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ba64-104">Сложный тип, содержащий свойства [аналитики](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="7ba64-104">Complex type containing properties of [insights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ba64-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ba64-105">JSON representation</span></span>

<span data-ttu-id="7ba64-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="7ba64-106">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.resourceReference"
}-->
```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="7ba64-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ba64-107">Properties</span></span>

| <span data-ttu-id="7ba64-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ba64-108">Property</span></span>      | <span data-ttu-id="7ba64-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7ba64-109">Type</span></span>      | <span data-ttu-id="7ba64-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7ba64-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="7ba64-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="7ba64-111">webUrl</span></span>        | <span data-ttu-id="7ba64-112">String</span><span class="sxs-lookup"><span data-stu-id="7ba64-112">String</span></span>    | <span data-ttu-id="7ba64-113">URL-адрес, ведущая к указанному элементу.</span><span class="sxs-lookup"><span data-stu-id="7ba64-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="7ba64-114">id</span><span class="sxs-lookup"><span data-stu-id="7ba64-114">id</span></span>            | <span data-ttu-id="7ba64-115">Строка</span><span class="sxs-lookup"><span data-stu-id="7ba64-115">String</span></span>    | <span data-ttu-id="7ba64-116">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="7ba64-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="7ba64-117">type</span><span class="sxs-lookup"><span data-stu-id="7ba64-117">type</span></span>          | <span data-ttu-id="7ba64-118">String</span><span class="sxs-lookup"><span data-stu-id="7ba64-118">String</span></span>    | <span data-ttu-id="7ba64-119">Строковое значение, которое может использоваться для классификации элемента, например "Microsoft. Graph. driveItem"</span><span class="sxs-lookup"><span data-stu-id="7ba64-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
