---
title: Тип ресурса resourceReference
description: Сложный тип, содержащий свойства средствами.
ms.openlocfilehash: d171151a1c3547aa6863a7f70cc3a42ddec13e5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079616"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="4d948-103">Тип ресурса resourceReference</span><span class="sxs-lookup"><span data-stu-id="4d948-103">resourceReference resource type</span></span>

> <span data-ttu-id="4d948-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4d948-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d948-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d948-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d948-106">Сложный тип, содержащий свойства [средствами](insights.md).</span><span class="sxs-lookup"><span data-stu-id="4d948-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d948-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d948-107">JSON representation</span></span>

<span data-ttu-id="4d948-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="4d948-108">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="4d948-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d948-109">Properties</span></span>

| <span data-ttu-id="4d948-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d948-110">Property</span></span>      | <span data-ttu-id="4d948-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4d948-111">Type</span></span>      | <span data-ttu-id="4d948-112">Description</span><span class="sxs-lookup"><span data-stu-id="4d948-112">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="4d948-113">webUrl</span><span class="sxs-lookup"><span data-stu-id="4d948-113">webUrl</span></span>        | <span data-ttu-id="4d948-114">String</span><span class="sxs-lookup"><span data-stu-id="4d948-114">String</span></span>    | <span data-ttu-id="4d948-115">URL-адрес, приводя к указанного элемента.</span><span class="sxs-lookup"><span data-stu-id="4d948-115">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="4d948-116">id</span><span class="sxs-lookup"><span data-stu-id="4d948-116">id</span></span>            | <span data-ttu-id="4d948-117">String</span><span class="sxs-lookup"><span data-stu-id="4d948-117">String</span></span>    | <span data-ttu-id="4d948-118">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="4d948-118">The item's unique identifier.</span></span>           |
| <span data-ttu-id="4d948-119">type</span><span class="sxs-lookup"><span data-stu-id="4d948-119">type</span></span>          | <span data-ttu-id="4d948-120">String</span><span class="sxs-lookup"><span data-stu-id="4d948-120">String</span></span>    | <span data-ttu-id="4d948-121">Строковое значение, которое можно использовать для классификации элемента, например, «microsoft.graph.driveItem»</span><span class="sxs-lookup"><span data-stu-id="4d948-121">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |