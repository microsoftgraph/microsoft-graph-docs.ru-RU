---
title: Тип ресурса resourceReference
description: Сложный тип, содержащий свойства средствами.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 23a05a362ea57c84dceecbd9523c2620edc21fbf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966288"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="b83a0-103">Тип ресурса resourceReference</span><span class="sxs-lookup"><span data-stu-id="b83a0-103">resourceReference resource type</span></span>

> <span data-ttu-id="b83a0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b83a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b83a0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b83a0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b83a0-106">Сложный тип, содержащий свойства [средствами](insights.md).</span><span class="sxs-lookup"><span data-stu-id="b83a0-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b83a0-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b83a0-107">JSON representation</span></span>

<span data-ttu-id="b83a0-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="b83a0-108">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="b83a0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b83a0-109">Properties</span></span>

| <span data-ttu-id="b83a0-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b83a0-110">Property</span></span>      | <span data-ttu-id="b83a0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b83a0-111">Type</span></span>      | <span data-ttu-id="b83a0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b83a0-112">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="b83a0-113">webUrl</span><span class="sxs-lookup"><span data-stu-id="b83a0-113">webUrl</span></span>        | <span data-ttu-id="b83a0-114">Строка</span><span class="sxs-lookup"><span data-stu-id="b83a0-114">String</span></span>    | <span data-ttu-id="b83a0-115">URL-адрес, приводя к указанного элемента.</span><span class="sxs-lookup"><span data-stu-id="b83a0-115">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="b83a0-116">id</span><span class="sxs-lookup"><span data-stu-id="b83a0-116">id</span></span>            | <span data-ttu-id="b83a0-117">Строка</span><span class="sxs-lookup"><span data-stu-id="b83a0-117">String</span></span>    | <span data-ttu-id="b83a0-118">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="b83a0-118">The item's unique identifier.</span></span>           |
| <span data-ttu-id="b83a0-119">type</span><span class="sxs-lookup"><span data-stu-id="b83a0-119">type</span></span>          | <span data-ttu-id="b83a0-120">Строка</span><span class="sxs-lookup"><span data-stu-id="b83a0-120">String</span></span>    | <span data-ttu-id="b83a0-121">Строковое значение, которое можно использовать для классификации элемента, например, «microsoft.graph.driveItem»</span><span class="sxs-lookup"><span data-stu-id="b83a0-121">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
