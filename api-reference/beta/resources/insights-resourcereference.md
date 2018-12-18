---
title: Тип ресурса resourceReference
description: Сложный тип, содержащий свойства средствами.
author: simonhult
ms.openlocfilehash: 2f1a44412eebbb7a74895c12db9a07696d6ee409
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363622"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="7c989-103">Тип ресурса resourceReference</span><span class="sxs-lookup"><span data-stu-id="7c989-103">resourceReference resource type</span></span>

> <span data-ttu-id="7c989-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7c989-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c989-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c989-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7c989-106">Сложный тип, содержащий свойства [средствами](insights.md).</span><span class="sxs-lookup"><span data-stu-id="7c989-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c989-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c989-107">JSON representation</span></span>

<span data-ttu-id="7c989-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="7c989-108">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="7c989-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c989-109">Properties</span></span>

| <span data-ttu-id="7c989-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c989-110">Property</span></span>      | <span data-ttu-id="7c989-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7c989-111">Type</span></span>      | <span data-ttu-id="7c989-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7c989-112">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="7c989-113">webUrl</span><span class="sxs-lookup"><span data-stu-id="7c989-113">webUrl</span></span>        | <span data-ttu-id="7c989-114">Строка</span><span class="sxs-lookup"><span data-stu-id="7c989-114">String</span></span>    | <span data-ttu-id="7c989-115">URL-адрес, приводя к указанного элемента.</span><span class="sxs-lookup"><span data-stu-id="7c989-115">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="7c989-116">id</span><span class="sxs-lookup"><span data-stu-id="7c989-116">id</span></span>            | <span data-ttu-id="7c989-117">Строка</span><span class="sxs-lookup"><span data-stu-id="7c989-117">String</span></span>    | <span data-ttu-id="7c989-118">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="7c989-118">The item's unique identifier.</span></span>           |
| <span data-ttu-id="7c989-119">type</span><span class="sxs-lookup"><span data-stu-id="7c989-119">type</span></span>          | <span data-ttu-id="7c989-120">Строка</span><span class="sxs-lookup"><span data-stu-id="7c989-120">String</span></span>    | <span data-ttu-id="7c989-121">Строковое значение, которое можно использовать для классификации элемента, например, «microsoft.graph.driveItem»</span><span class="sxs-lookup"><span data-stu-id="7c989-121">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |