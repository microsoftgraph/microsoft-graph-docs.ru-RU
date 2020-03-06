---
title: Тип ресурса Ресаурцереференце
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: aa00eb06ac239b4f93a200e72ecbe88c99d6189c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532870"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="4ffa8-103">Тип ресурса Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="4ffa8-103">resourceReference resource type</span></span>

<span data-ttu-id="4ffa8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ffa8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ffa8-105">Сложный тип, содержащий свойства [оффицеграфинсигхтс](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="4ffa8-105">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ffa8-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ffa8-106">JSON representation</span></span>

<span data-ttu-id="4ffa8-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="4ffa8-107">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="4ffa8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ffa8-108">Properties</span></span>

| <span data-ttu-id="4ffa8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ffa8-109">Property</span></span>      | <span data-ttu-id="4ffa8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4ffa8-110">Type</span></span>      | <span data-ttu-id="4ffa8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4ffa8-111">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="4ffa8-112">webUrl</span><span class="sxs-lookup"><span data-stu-id="4ffa8-112">webUrl</span></span>        | <span data-ttu-id="4ffa8-113">String</span><span class="sxs-lookup"><span data-stu-id="4ffa8-113">String</span></span>    | <span data-ttu-id="4ffa8-114">URL-адрес, ведущая к указанному элементу.</span><span class="sxs-lookup"><span data-stu-id="4ffa8-114">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="4ffa8-115">id</span><span class="sxs-lookup"><span data-stu-id="4ffa8-115">id</span></span>            | <span data-ttu-id="4ffa8-116">Строка</span><span class="sxs-lookup"><span data-stu-id="4ffa8-116">String</span></span>    | <span data-ttu-id="4ffa8-117">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="4ffa8-117">The item's unique identifier.</span></span>           |
| <span data-ttu-id="4ffa8-118">type</span><span class="sxs-lookup"><span data-stu-id="4ffa8-118">type</span></span>          | <span data-ttu-id="4ffa8-119">String</span><span class="sxs-lookup"><span data-stu-id="4ffa8-119">String</span></span>    | <span data-ttu-id="4ffa8-120">Строковое значение, которое может использоваться для классификации элемента, например "Microsoft. Graph. driveItem"</span><span class="sxs-lookup"><span data-stu-id="4ffa8-120">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
