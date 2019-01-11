---
title: Тип ресурса resourceReference
description: Сложный тип, содержащий свойства средствами.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 8ab2a79d66db6a45ecf3df748cf8f5740721ef80
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874328"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="e8732-103">Тип ресурса resourceReference</span><span class="sxs-lookup"><span data-stu-id="e8732-103">resourceReference resource type</span></span>

> <span data-ttu-id="e8732-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e8732-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8732-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8732-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8732-106">Сложный тип, содержащий свойства [средствами](insights.md).</span><span class="sxs-lookup"><span data-stu-id="e8732-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8732-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8732-107">JSON representation</span></span>

<span data-ttu-id="e8732-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e8732-108">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="e8732-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8732-109">Properties</span></span>

| <span data-ttu-id="e8732-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8732-110">Property</span></span>      | <span data-ttu-id="e8732-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e8732-111">Type</span></span>      | <span data-ttu-id="e8732-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e8732-112">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="e8732-113">webUrl</span><span class="sxs-lookup"><span data-stu-id="e8732-113">webUrl</span></span>        | <span data-ttu-id="e8732-114">Строка</span><span class="sxs-lookup"><span data-stu-id="e8732-114">String</span></span>    | <span data-ttu-id="e8732-115">URL-адрес, приводя к указанного элемента.</span><span class="sxs-lookup"><span data-stu-id="e8732-115">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="e8732-116">id</span><span class="sxs-lookup"><span data-stu-id="e8732-116">id</span></span>            | <span data-ttu-id="e8732-117">Строка</span><span class="sxs-lookup"><span data-stu-id="e8732-117">String</span></span>    | <span data-ttu-id="e8732-118">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="e8732-118">The item's unique identifier.</span></span>           |
| <span data-ttu-id="e8732-119">type</span><span class="sxs-lookup"><span data-stu-id="e8732-119">type</span></span>          | <span data-ttu-id="e8732-120">Строка</span><span class="sxs-lookup"><span data-stu-id="e8732-120">String</span></span>    | <span data-ttu-id="e8732-121">Строковое значение, которое можно использовать для классификации элемента, например, «microsoft.graph.driveItem»</span><span class="sxs-lookup"><span data-stu-id="e8732-121">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
