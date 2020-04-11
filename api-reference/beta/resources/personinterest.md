---
title: Тип ресурса Персонинтерест
description: Тип ресурса Персонинтерест
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: d10ea81f3648be1896637ca866d0185c2a674097
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227738"
---
# <a name="personinterest-resource-type"></a><span data-ttu-id="23b70-103">Тип ресурса Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="23b70-103">personInterest resource type</span></span>

<span data-ttu-id="23b70-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23b70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23b70-105">Предоставляет подробные сведения о интересах, которые пользователь связал с собственными службами в различных службах.</span><span class="sxs-lookup"><span data-stu-id="23b70-105">Provides detailed information about interests the user has associated with themselves in various services.</span></span>

<span data-ttu-id="23b70-106">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="23b70-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="23b70-107">Методы</span><span class="sxs-lookup"><span data-stu-id="23b70-107">Methods</span></span>

| <span data-ttu-id="23b70-108">Метод</span><span class="sxs-lookup"><span data-stu-id="23b70-108">Method</span></span>                                                    | <span data-ttu-id="23b70-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="23b70-109">Return Type</span></span>                         | <span data-ttu-id="23b70-110">Описание</span><span class="sxs-lookup"><span data-stu-id="23b70-110">Description</span></span>                                                           |
|:----------------------------------------------------------|:------------------------------------|:----------------------------------------------------------------------|
| [<span data-ttu-id="23b70-111">Получение Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="23b70-111">Get personInterest</span></span>](../api/personinterest-get.md)        | [<span data-ttu-id="23b70-112">персонинтерест</span><span class="sxs-lookup"><span data-stu-id="23b70-112">personInterest</span></span>](personinterest.md) | <span data-ttu-id="23b70-113">Чтение свойств и связей объекта **персонинтерест** .</span><span class="sxs-lookup"><span data-stu-id="23b70-113">Read the properties and relationships of a **personInterest** object.</span></span> |
| [<span data-ttu-id="23b70-114">Обновление Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="23b70-114">Update personInterest</span></span>](../api/personinterest-update.md)  | [<span data-ttu-id="23b70-115">персонинтерест</span><span class="sxs-lookup"><span data-stu-id="23b70-115">personInterest</span></span>](personinterest.md) | <span data-ttu-id="23b70-116">Обновление объекта **персонинтерест** .</span><span class="sxs-lookup"><span data-stu-id="23b70-116">Update a **personInterest** object.</span></span>                                   |
| [<span data-ttu-id="23b70-117">Удаление Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="23b70-117">Delete personInterest</span></span>](../api/personinterest-delete.md)  | <span data-ttu-id="23b70-118">Нет</span><span class="sxs-lookup"><span data-stu-id="23b70-118">None</span></span>                                | <span data-ttu-id="23b70-119">Удаление объекта **персонинтерест** .</span><span class="sxs-lookup"><span data-stu-id="23b70-119">Delete a **personInterest** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="23b70-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="23b70-120">Properties</span></span>

| <span data-ttu-id="23b70-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="23b70-121">Property</span></span>     | <span data-ttu-id="23b70-122">Тип</span><span class="sxs-lookup"><span data-stu-id="23b70-122">Type</span></span>             | <span data-ttu-id="23b70-123">Описание</span><span class="sxs-lookup"><span data-stu-id="23b70-123">Description</span></span>                                                                                    |
|:-------------|:-----------------|:-----------------------------------------------------------------------------------------------|
|<span data-ttu-id="23b70-124">categories</span><span class="sxs-lookup"><span data-stu-id="23b70-124">categories</span></span>    |<span data-ttu-id="23b70-125">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="23b70-125">String collection</span></span> | <span data-ttu-id="23b70-126">Содержит категории, которые пользователь связал с интересом (например, персональный, реЦипиес).</span><span class="sxs-lookup"><span data-stu-id="23b70-126">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="23b70-127">description</span><span class="sxs-lookup"><span data-stu-id="23b70-127">description</span></span>   |<span data-ttu-id="23b70-128">String</span><span class="sxs-lookup"><span data-stu-id="23b70-128">String</span></span>            | <span data-ttu-id="23b70-129">Содержит описание интереса.</span><span class="sxs-lookup"><span data-stu-id="23b70-129">Contains a description of the interest.</span></span>                                                        |
|<span data-ttu-id="23b70-130">displayName</span><span class="sxs-lookup"><span data-stu-id="23b70-130">displayName</span></span>   |<span data-ttu-id="23b70-131">Строка</span><span class="sxs-lookup"><span data-stu-id="23b70-131">String</span></span>            | <span data-ttu-id="23b70-132">Содержит понятное имя для интереса.</span><span class="sxs-lookup"><span data-stu-id="23b70-132">Contains a friendly name for the interest.</span></span>                                                     |
|<span data-ttu-id="23b70-133">webUrl</span><span class="sxs-lookup"><span data-stu-id="23b70-133">webUrl</span></span>        |<span data-ttu-id="23b70-134">String</span><span class="sxs-lookup"><span data-stu-id="23b70-134">String</span></span>            | <span data-ttu-id="23b70-135">Содержит ссылку на веб-страницу или ресурс, представляющие интерес.</span><span class="sxs-lookup"><span data-stu-id="23b70-135">Contains a link to a web page or resource about the interest.</span></span>                                  |

## <a name="relationships"></a><span data-ttu-id="23b70-136">Связи</span><span class="sxs-lookup"><span data-stu-id="23b70-136">Relationships</span></span>

<span data-ttu-id="23b70-137">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="23b70-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23b70-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="23b70-138">JSON representation</span></span>

<span data-ttu-id="23b70-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23b70-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personInterest",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "description": "String",
  "displayName": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personInterest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
