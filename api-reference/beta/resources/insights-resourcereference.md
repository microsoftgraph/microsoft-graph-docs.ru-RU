---
title: Тип ресурса Ресаурцереференце
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 2992895b2fbc426d4177dd86074dcf5cb8d784ab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495867"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="b488b-103">Тип ресурса Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="b488b-103">resourceReference resource type</span></span>

<span data-ttu-id="b488b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b488b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b488b-105">Сложный тип, содержащий свойства [оффицеграфинсигхтс](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="b488b-105">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b488b-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b488b-106">JSON representation</span></span>

<span data-ttu-id="b488b-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="b488b-107">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="b488b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b488b-108">Properties</span></span>

| <span data-ttu-id="b488b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b488b-109">Property</span></span>      | <span data-ttu-id="b488b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b488b-110">Type</span></span>      | <span data-ttu-id="b488b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b488b-111">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="b488b-112">webUrl</span><span class="sxs-lookup"><span data-stu-id="b488b-112">webUrl</span></span>        | <span data-ttu-id="b488b-113">String</span><span class="sxs-lookup"><span data-stu-id="b488b-113">String</span></span>    | <span data-ttu-id="b488b-114">URL-адрес, ведущая к указанному элементу.</span><span class="sxs-lookup"><span data-stu-id="b488b-114">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="b488b-115">id</span><span class="sxs-lookup"><span data-stu-id="b488b-115">id</span></span>            | <span data-ttu-id="b488b-116">Строка</span><span class="sxs-lookup"><span data-stu-id="b488b-116">String</span></span>    | <span data-ttu-id="b488b-117">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="b488b-117">The item's unique identifier.</span></span>           |
| <span data-ttu-id="b488b-118">type</span><span class="sxs-lookup"><span data-stu-id="b488b-118">type</span></span>          | <span data-ttu-id="b488b-119">String</span><span class="sxs-lookup"><span data-stu-id="b488b-119">String</span></span>    | <span data-ttu-id="b488b-120">Строковое значение, которое может использоваться для классификации элемента, например "Microsoft. Graph. driveItem"</span><span class="sxs-lookup"><span data-stu-id="b488b-120">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
