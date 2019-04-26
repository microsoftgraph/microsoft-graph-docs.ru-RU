---
title: Тип ресурса Ресаурцереференце
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: accd2b0b12f8068ea990fbd611b46053f66d6de4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340008"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="b1211-103">Тип ресурса Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="b1211-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1211-104">Сложный тип, содержащий свойства [аналитики](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="b1211-104">Complex type containing properties of [insights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1211-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1211-105">JSON representation</span></span>

<span data-ttu-id="b1211-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="b1211-106">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="b1211-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1211-107">Properties</span></span>

| <span data-ttu-id="b1211-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1211-108">Property</span></span>      | <span data-ttu-id="b1211-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b1211-109">Type</span></span>      | <span data-ttu-id="b1211-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b1211-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="b1211-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="b1211-111">webUrl</span></span>        | <span data-ttu-id="b1211-112">String</span><span class="sxs-lookup"><span data-stu-id="b1211-112">String</span></span>    | <span data-ttu-id="b1211-113">URL-адрес, ведущая к указанному элементу.</span><span class="sxs-lookup"><span data-stu-id="b1211-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="b1211-114">id</span><span class="sxs-lookup"><span data-stu-id="b1211-114">id</span></span>            | <span data-ttu-id="b1211-115">Строка</span><span class="sxs-lookup"><span data-stu-id="b1211-115">String</span></span>    | <span data-ttu-id="b1211-116">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="b1211-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="b1211-117">type</span><span class="sxs-lookup"><span data-stu-id="b1211-117">type</span></span>          | <span data-ttu-id="b1211-118">String</span><span class="sxs-lookup"><span data-stu-id="b1211-118">String</span></span>    | <span data-ttu-id="b1211-119">Строковое значение, которое может использоваться для классификации элемента, например "Microsoft. Graph. driveItem"</span><span class="sxs-lookup"><span data-stu-id="b1211-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
