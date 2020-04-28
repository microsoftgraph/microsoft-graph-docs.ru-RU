---
title: Тип ресурса Персонанниверсари
description: Тип ресурса Персонанниверсари
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: c8ea4e9bf7db268c5ec6bffad1c7d43cbbdd2439
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227733"
---
# <a name="personanniversary-resource-type"></a><span data-ttu-id="aeb0c-103">Тип ресурса Персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="aeb0c-103">personAnniversary resource type</span></span>

<span data-ttu-id="aeb0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aeb0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aeb0c-105">Представляет сведения о значимых датах, связанных с пользователем в [профиле](profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="aeb0c-105">Represents the details of meaningful dates associated with a person in a user's [profile](profile.md).</span></span>

<span data-ttu-id="aeb0c-106">Наследуется от [итемфацет](itemFacet.md).</span><span class="sxs-lookup"><span data-stu-id="aeb0c-106">Inherits from [itemFacet](itemFacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="aeb0c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="aeb0c-107">Methods</span></span>

| <span data-ttu-id="aeb0c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="aeb0c-108">Method</span></span>                                                   | <span data-ttu-id="aeb0c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="aeb0c-109">Return Type</span></span>                               | <span data-ttu-id="aeb0c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aeb0c-110">Description</span></span>                                                              |
|:---------------------------------------------------------|:------------------------------------------|:-------------------------------------------------------------------------|
| [<span data-ttu-id="aeb0c-111">Получение Персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="aeb0c-111">Get personAnniversary</span></span>](../api/personanniversary-get.md) | [<span data-ttu-id="aeb0c-112">персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="aeb0c-112">personAnniversary</span></span>](personanniversary.md) | <span data-ttu-id="aeb0c-113">Чтение свойств и связей объекта **персонанниверсари** .</span><span class="sxs-lookup"><span data-stu-id="aeb0c-113">Read the properties and relationships of a **personAnniversary** object.</span></span> |
| <span data-ttu-id="aeb0c-114">[обновление](../api/personanniversary-update.md).</span><span class="sxs-lookup"><span data-stu-id="aeb0c-114">[Update](../api/personanniversary-update.md)</span></span>             | [<span data-ttu-id="aeb0c-115">персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="aeb0c-115">personAnniversary</span></span>](personanniversary.md) | <span data-ttu-id="aeb0c-116">Обновление объекта **персонанниверсари** .</span><span class="sxs-lookup"><span data-stu-id="aeb0c-116">Update a **personAnniversary** object.</span></span>                                   |
| <span data-ttu-id="aeb0c-117">[удаление](../api/personanniversary-delete.md);</span><span class="sxs-lookup"><span data-stu-id="aeb0c-117">[Delete](../api/personanniversary-delete.md)</span></span>             | <span data-ttu-id="aeb0c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="aeb0c-118">None</span></span>                                      | <span data-ttu-id="aeb0c-119">Удаление объекта **персонанниверсари** .</span><span class="sxs-lookup"><span data-stu-id="aeb0c-119">Delete a **personAnniversary** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="aeb0c-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="aeb0c-120">Properties</span></span>

| <span data-ttu-id="aeb0c-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="aeb0c-121">Property</span></span>     | <span data-ttu-id="aeb0c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="aeb0c-122">Type</span></span>        | <span data-ttu-id="aeb0c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="aeb0c-123">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="aeb0c-124">date</span><span class="sxs-lookup"><span data-stu-id="aeb0c-124">date</span></span>          |<span data-ttu-id="aeb0c-125">Date</span><span class="sxs-lookup"><span data-stu-id="aeb0c-125">Date</span></span>         | <span data-ttu-id="aeb0c-126">Содержит дату, связанную с типом юбилея.</span><span class="sxs-lookup"><span data-stu-id="aeb0c-126">Contains the date associated with the anniversary type.</span></span>          |
|<span data-ttu-id="aeb0c-127">type</span><span class="sxs-lookup"><span data-stu-id="aeb0c-127">type</span></span>          |<span data-ttu-id="aeb0c-128">string</span><span class="sxs-lookup"><span data-stu-id="aeb0c-128">string</span></span>       | <span data-ttu-id="aeb0c-129">Возможные значения: `birthday`, `wedding`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="aeb0c-129">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aeb0c-130">Связи</span><span class="sxs-lookup"><span data-stu-id="aeb0c-130">Relationships</span></span>

<span data-ttu-id="aeb0c-131">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="aeb0c-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aeb0c-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="aeb0c-132">JSON representation</span></span>

<span data-ttu-id="aeb0c-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aeb0c-133">The following is a JSON representation of the resource.</span></span>

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
