---
title: Тип ресурса Ресаурцереференце
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c75eab84dea4e0f9134185fd9679770369073bf4
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844435"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="3c42c-103">Тип ресурса Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="3c42c-103">resourceReference resource type</span></span>

<span data-ttu-id="3c42c-104">Сложный тип, содержащий свойства [оффицеграфинсигхтс](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="3c42c-104">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c42c-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c42c-105">JSON representation</span></span>

<span data-ttu-id="3c42c-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="3c42c-106">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="3c42c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c42c-107">Properties</span></span>

| <span data-ttu-id="3c42c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c42c-108">Property</span></span>      | <span data-ttu-id="3c42c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3c42c-109">Type</span></span>      | <span data-ttu-id="3c42c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3c42c-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="3c42c-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="3c42c-111">webUrl</span></span>        | <span data-ttu-id="3c42c-112">String</span><span class="sxs-lookup"><span data-stu-id="3c42c-112">String</span></span>    | <span data-ttu-id="3c42c-113">URL-адрес, ведущая к указанному элементу.</span><span class="sxs-lookup"><span data-stu-id="3c42c-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="3c42c-114">id</span><span class="sxs-lookup"><span data-stu-id="3c42c-114">id</span></span>            | <span data-ttu-id="3c42c-115">Строка</span><span class="sxs-lookup"><span data-stu-id="3c42c-115">String</span></span>    | <span data-ttu-id="3c42c-116">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="3c42c-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="3c42c-117">type</span><span class="sxs-lookup"><span data-stu-id="3c42c-117">type</span></span>          | <span data-ttu-id="3c42c-118">String</span><span class="sxs-lookup"><span data-stu-id="3c42c-118">String</span></span>    | <span data-ttu-id="3c42c-119">Строковое значение, которое может использоваться для классификации элемента, например "Microsoft. Graph. driveItem"</span><span class="sxs-lookup"><span data-stu-id="3c42c-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
