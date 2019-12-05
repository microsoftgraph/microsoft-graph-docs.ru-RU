---
title: Тип ресурса Ресаурцереференце
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c15720ac3f2bda673d495fbe32dc6bae8d5898d7
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844500"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="4be89-103">Тип ресурса Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="4be89-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4be89-104">Сложный тип, содержащий свойства [оффицеграфинсигхтс](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="4be89-104">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="4be89-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4be89-105">JSON representation</span></span>

<span data-ttu-id="4be89-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="4be89-106">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="4be89-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4be89-107">Properties</span></span>

| <span data-ttu-id="4be89-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4be89-108">Property</span></span>      | <span data-ttu-id="4be89-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4be89-109">Type</span></span>      | <span data-ttu-id="4be89-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4be89-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="4be89-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="4be89-111">webUrl</span></span>        | <span data-ttu-id="4be89-112">String</span><span class="sxs-lookup"><span data-stu-id="4be89-112">String</span></span>    | <span data-ttu-id="4be89-113">URL-адрес, ведущая к указанному элементу.</span><span class="sxs-lookup"><span data-stu-id="4be89-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="4be89-114">id</span><span class="sxs-lookup"><span data-stu-id="4be89-114">id</span></span>            | <span data-ttu-id="4be89-115">Строка</span><span class="sxs-lookup"><span data-stu-id="4be89-115">String</span></span>    | <span data-ttu-id="4be89-116">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="4be89-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="4be89-117">type</span><span class="sxs-lookup"><span data-stu-id="4be89-117">type</span></span>          | <span data-ttu-id="4be89-118">String</span><span class="sxs-lookup"><span data-stu-id="4be89-118">String</span></span>    | <span data-ttu-id="4be89-119">Строковое значение, которое может использоваться для классификации элемента, например "Microsoft. Graph. driveItem"</span><span class="sxs-lookup"><span data-stu-id="4be89-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
