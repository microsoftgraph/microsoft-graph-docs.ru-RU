---
title: Тип ресурса Ресаурцереференце
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a353eb07c1aeb2fd904b9f97c8307ed0b5190470
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021856"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="edaf4-103">Тип ресурса Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="edaf4-103">resourceReference resource type</span></span>

<span data-ttu-id="edaf4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edaf4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edaf4-105">Сложный тип, содержащий свойства [итеминсигхтс](iteminsights.md)</span><span class="sxs-lookup"><span data-stu-id="edaf4-105">Complex type containing properties of [itemInsights](iteminsights.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="edaf4-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="edaf4-106">JSON representation</span></span>

<span data-ttu-id="edaf4-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="edaf4-107">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="edaf4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="edaf4-108">Properties</span></span>

| <span data-ttu-id="edaf4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="edaf4-109">Property</span></span>      | <span data-ttu-id="edaf4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="edaf4-110">Type</span></span>      | <span data-ttu-id="edaf4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="edaf4-111">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="edaf4-112">webUrl</span><span class="sxs-lookup"><span data-stu-id="edaf4-112">webUrl</span></span>        | <span data-ttu-id="edaf4-113">String</span><span class="sxs-lookup"><span data-stu-id="edaf4-113">String</span></span>    | <span data-ttu-id="edaf4-114">URL-адрес, ведущая к указанному элементу.</span><span class="sxs-lookup"><span data-stu-id="edaf4-114">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="edaf4-115">id</span><span class="sxs-lookup"><span data-stu-id="edaf4-115">id</span></span>            | <span data-ttu-id="edaf4-116">String</span><span class="sxs-lookup"><span data-stu-id="edaf4-116">String</span></span>    | <span data-ttu-id="edaf4-117">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="edaf4-117">The item's unique identifier.</span></span>           |
| <span data-ttu-id="edaf4-118">type</span><span class="sxs-lookup"><span data-stu-id="edaf4-118">type</span></span>          | <span data-ttu-id="edaf4-119">String</span><span class="sxs-lookup"><span data-stu-id="edaf4-119">String</span></span>    | <span data-ttu-id="edaf4-120">Строковое значение, которое может использоваться для классификации элемента, например "Microsoft. Graph. driveItem"</span><span class="sxs-lookup"><span data-stu-id="edaf4-120">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |


