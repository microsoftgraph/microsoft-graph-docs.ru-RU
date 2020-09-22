---
title: Тип ресурса Ресаурцереференце
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 56f1cc992deaa74623930074ea75b6cb0fa9e0ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054842"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="dec2d-103">Тип ресурса Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="dec2d-103">resourceReference resource type</span></span>

<span data-ttu-id="dec2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dec2d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dec2d-105">Сложный тип, содержащий свойства [оффицеграфинсигхтс](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="dec2d-105">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="dec2d-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dec2d-106">JSON representation</span></span>

<span data-ttu-id="dec2d-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="dec2d-107">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="dec2d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="dec2d-108">Properties</span></span>

| <span data-ttu-id="dec2d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dec2d-109">Property</span></span>      | <span data-ttu-id="dec2d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dec2d-110">Type</span></span>      | <span data-ttu-id="dec2d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dec2d-111">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="dec2d-112">webUrl</span><span class="sxs-lookup"><span data-stu-id="dec2d-112">webUrl</span></span>        | <span data-ttu-id="dec2d-113">String</span><span class="sxs-lookup"><span data-stu-id="dec2d-113">String</span></span>    | <span data-ttu-id="dec2d-114">URL-адрес, ведущая к указанному элементу.</span><span class="sxs-lookup"><span data-stu-id="dec2d-114">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="dec2d-115">id</span><span class="sxs-lookup"><span data-stu-id="dec2d-115">id</span></span>            | <span data-ttu-id="dec2d-116">String</span><span class="sxs-lookup"><span data-stu-id="dec2d-116">String</span></span>    | <span data-ttu-id="dec2d-117">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="dec2d-117">The item's unique identifier.</span></span>           |
| <span data-ttu-id="dec2d-118">type</span><span class="sxs-lookup"><span data-stu-id="dec2d-118">type</span></span>          | <span data-ttu-id="dec2d-119">String</span><span class="sxs-lookup"><span data-stu-id="dec2d-119">String</span></span>    | <span data-ttu-id="dec2d-120">Строковое значение, которое может использоваться для классификации элемента, например "Microsoft. Graph. driveItem"</span><span class="sxs-lookup"><span data-stu-id="dec2d-120">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |

