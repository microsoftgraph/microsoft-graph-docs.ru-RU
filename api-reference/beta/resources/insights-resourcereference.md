---
title: Тип ресурса Ресаурцереференце
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: fac5ec3b40467034a583933a6e09399e91badfe0
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427398"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="67163-103">Тип ресурса Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="67163-103">resourceReference resource type</span></span>

<span data-ttu-id="67163-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67163-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67163-105">Сложный тип, содержащий свойства [итеминсигхтс](iteminsights.md)</span><span class="sxs-lookup"><span data-stu-id="67163-105">Complex type containing properties of [itemInsights](iteminsights.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="67163-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67163-106">JSON representation</span></span>

<span data-ttu-id="67163-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="67163-107">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="67163-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="67163-108">Properties</span></span>

| <span data-ttu-id="67163-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="67163-109">Property</span></span>      | <span data-ttu-id="67163-110">Тип</span><span class="sxs-lookup"><span data-stu-id="67163-110">Type</span></span>      | <span data-ttu-id="67163-111">Описание</span><span class="sxs-lookup"><span data-stu-id="67163-111">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="67163-112">webUrl</span><span class="sxs-lookup"><span data-stu-id="67163-112">webUrl</span></span>        | <span data-ttu-id="67163-113">String</span><span class="sxs-lookup"><span data-stu-id="67163-113">String</span></span>    | <span data-ttu-id="67163-114">URL-адрес, ведущая к указанному элементу.</span><span class="sxs-lookup"><span data-stu-id="67163-114">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="67163-115">id</span><span class="sxs-lookup"><span data-stu-id="67163-115">id</span></span>            | <span data-ttu-id="67163-116">Строка</span><span class="sxs-lookup"><span data-stu-id="67163-116">String</span></span>    | <span data-ttu-id="67163-117">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="67163-117">The item's unique identifier.</span></span>           |
| <span data-ttu-id="67163-118">type</span><span class="sxs-lookup"><span data-stu-id="67163-118">type</span></span>          | <span data-ttu-id="67163-119">String</span><span class="sxs-lookup"><span data-stu-id="67163-119">String</span></span>    | <span data-ttu-id="67163-120">Строковое значение, которое может использоваться для классификации элемента, например "Microsoft. Graph. driveItem"</span><span class="sxs-lookup"><span data-stu-id="67163-120">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
