---
title: Тип ресурса Персонанниверсари
description: Тип ресурса Персонанниверсари
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1ad4c5a1792ee0e75a31f165b0a8eebf6f0d2130
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949519"
---
# <a name="personanniversary-resource-type"></a><span data-ttu-id="1e536-103">Тип ресурса Персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="1e536-103">personAnniversary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e536-104">Представляет сведения о значимых датах, связанных с пользователем в [профиле](profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="1e536-104">Represents the details of meaningful dates associated with a person in a user's [profile](profile.md).</span></span>

<span data-ttu-id="1e536-105">Наследуется от [итемфацет](itemFacet.md).</span><span class="sxs-lookup"><span data-stu-id="1e536-105">Inherits from [itemFacet](itemFacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1e536-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1e536-106">Methods</span></span>

| <span data-ttu-id="1e536-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1e536-107">Method</span></span>                                                   | <span data-ttu-id="1e536-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1e536-108">Return Type</span></span>                               | <span data-ttu-id="1e536-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1e536-109">Description</span></span>                                                    |
|:---------------------------------------------------------|:------------------------------------------|:---------------------------------------------------------------|
| [<span data-ttu-id="1e536-110">Получение Персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="1e536-110">Get personAnniversary</span></span>](../api/personanniversary-get.md) | [<span data-ttu-id="1e536-111">персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="1e536-111">personAnniversary</span></span>](personanniversary.md) | <span data-ttu-id="1e536-112">Чтение свойств и связей объекта **персонанниверсари** .</span><span class="sxs-lookup"><span data-stu-id="1e536-112">Read the properties and relationships of a **personAnniversary** object.</span></span> |
| [<span data-ttu-id="1e536-113">Update</span><span class="sxs-lookup"><span data-stu-id="1e536-113">Update</span></span>](../api/personanniversary-update.md)             | [<span data-ttu-id="1e536-114">персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="1e536-114">personAnniversary</span></span>](personanniversary.md) | <span data-ttu-id="1e536-115">Обновление объекта **персонанниверсари** .</span><span class="sxs-lookup"><span data-stu-id="1e536-115">Update a **personAnniversary** object.</span></span>                               |
| [<span data-ttu-id="1e536-116">Delete</span><span class="sxs-lookup"><span data-stu-id="1e536-116">Delete</span></span>](../api/personanniversary-delete.md)             | <span data-ttu-id="1e536-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="1e536-117">None</span></span>                                      | <span data-ttu-id="1e536-118">Удаление объекта **персонанниверсари** .</span><span class="sxs-lookup"><span data-stu-id="1e536-118">Delete a **personAnniversary** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="1e536-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e536-119">Properties</span></span>

| <span data-ttu-id="1e536-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e536-120">Property</span></span>     | <span data-ttu-id="1e536-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1e536-121">Type</span></span>        | <span data-ttu-id="1e536-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1e536-122">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="1e536-123">date</span><span class="sxs-lookup"><span data-stu-id="1e536-123">date</span></span>          |<span data-ttu-id="1e536-124">Date</span><span class="sxs-lookup"><span data-stu-id="1e536-124">Date</span></span>         | <span data-ttu-id="1e536-125">Содержит дату, связанную с типом юбилея.</span><span class="sxs-lookup"><span data-stu-id="1e536-125">Contains the date associated with the anniversary type.</span></span>         |
|<span data-ttu-id="1e536-126">type</span><span class="sxs-lookup"><span data-stu-id="1e536-126">type</span></span>          |<span data-ttu-id="1e536-127">string</span><span class="sxs-lookup"><span data-stu-id="1e536-127">string</span></span>       | <span data-ttu-id="1e536-128">Возможные значения: `birthday`, `wedding`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1e536-128">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e536-129">Связи</span><span class="sxs-lookup"><span data-stu-id="1e536-129">Relationships</span></span>

<span data-ttu-id="1e536-130">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1e536-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e536-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1e536-131">JSON representation</span></span>

<span data-ttu-id="1e536-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e536-132">The following is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personAnniversary",
  "baseType": ""
}-->

```json
{
  "date": "String (timestamp)",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personAnniversary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
