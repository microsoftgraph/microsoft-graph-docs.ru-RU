---
title: Тип ресурса Лабелдетаилс
description: Представляет сведения о метке метки защиты информации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6b475c96b3ecbc2caa0aa147e3fc8fd0253ac243
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084039"
---
# <a name="labeldetails-resource-type"></a><span data-ttu-id="d9ee9-103">Тип ресурса Лабелдетаилс</span><span class="sxs-lookup"><span data-stu-id="d9ee9-103">labelDetails resource type</span></span>

<span data-ttu-id="d9ee9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9ee9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9ee9-105">Представляет сведения о метке метки защиты информации.</span><span class="sxs-lookup"><span data-stu-id="d9ee9-105">Represents the label details of an information protection label.</span></span> <span data-ttu-id="d9ee9-106">**лабелдетаилс** предоставляет сведения об отдельной метке защиты информации.</span><span class="sxs-lookup"><span data-stu-id="d9ee9-106">**labelDetails** provides information about a single information protection label.</span></span> <span data-ttu-id="d9ee9-107">Могут возвращаться [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md), [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md)и [екстрактлабел](../api/informationprotectionlabel-extractLabel.md)</span><span class="sxs-lookup"><span data-stu-id="d9ee9-107">Can be returned by [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d9ee9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9ee9-108">Properties</span></span>

| <span data-ttu-id="d9ee9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9ee9-109">Property</span></span>    | <span data-ttu-id="d9ee9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d9ee9-110">Type</span></span>    | <span data-ttu-id="d9ee9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d9ee9-111">Description</span></span>                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d9ee9-112">color</span><span class="sxs-lookup"><span data-stu-id="d9ee9-112">color</span></span>       | <span data-ttu-id="d9ee9-113">String</span><span class="sxs-lookup"><span data-stu-id="d9ee9-113">String</span></span>  | <span data-ttu-id="d9ee9-114">Цвет, который должен отображаться в пользовательском интерфейсе для метки, если она настроена.</span><span class="sxs-lookup"><span data-stu-id="d9ee9-114">The color that the user interface should display for the label, if configured.</span></span>                               |
| <span data-ttu-id="d9ee9-115">description</span><span class="sxs-lookup"><span data-stu-id="d9ee9-115">description</span></span> | <span data-ttu-id="d9ee9-116">Строка</span><span class="sxs-lookup"><span data-stu-id="d9ee9-116">String</span></span>  | <span data-ttu-id="d9ee9-117">Заданное администратором описание метки.</span><span class="sxs-lookup"><span data-stu-id="d9ee9-117">The admin-defined description for the label.</span></span>                                                                 |
| <span data-ttu-id="d9ee9-118">id</span><span class="sxs-lookup"><span data-stu-id="d9ee9-118">id</span></span>          | <span data-ttu-id="d9ee9-119">Строка</span><span class="sxs-lookup"><span data-stu-id="d9ee9-119">String</span></span>  | <span data-ttu-id="d9ee9-120">ИДЕНТИФИКАТОР метки является глобальным уникальным идентификатором (GUID).</span><span class="sxs-lookup"><span data-stu-id="d9ee9-120">The label ID is a globally unique identifier (GUID).</span></span>                                                          |
| <span data-ttu-id="d9ee9-121">isActive</span><span class="sxs-lookup"><span data-stu-id="d9ee9-121">isActive</span></span>    | <span data-ttu-id="d9ee9-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9ee9-122">Boolean</span></span> | <span data-ttu-id="d9ee9-123">Указывает, активна ли метка.</span><span class="sxs-lookup"><span data-stu-id="d9ee9-123">Indicates whether the label is active or not.</span></span> <span data-ttu-id="d9ee9-124">Активные метки должны быть скрыты или отключены в пользовательских интерфейсах.</span><span class="sxs-lookup"><span data-stu-id="d9ee9-124">Active labels should be hidden or disabled in user interfaces.</span></span> |
| <span data-ttu-id="d9ee9-125">name</span><span class="sxs-lookup"><span data-stu-id="d9ee9-125">name</span></span>        | <span data-ttu-id="d9ee9-126">String</span><span class="sxs-lookup"><span data-stu-id="d9ee9-126">String</span></span>  | <span data-ttu-id="d9ee9-127">Имя в виде открытого текста метки.</span><span class="sxs-lookup"><span data-stu-id="d9ee9-127">The plaintext name of the label.</span></span>                                                                             |
| <span data-ttu-id="d9ee9-128">sensitivity</span><span class="sxs-lookup"><span data-stu-id="d9ee9-128">sensitivity</span></span> | <span data-ttu-id="d9ee9-129">Int32</span><span class="sxs-lookup"><span data-stu-id="d9ee9-129">Int32</span></span>   | <span data-ttu-id="d9ee9-130">Значение чувствительности метки, где меньше конфиденциально.</span><span class="sxs-lookup"><span data-stu-id="d9ee9-130">The sensitivity value of the label, where lower is less sensitive.</span></span>                                           |
| <span data-ttu-id="d9ee9-131">tooltip</span><span class="sxs-lookup"><span data-stu-id="d9ee9-131">tooltip</span></span>     | <span data-ttu-id="d9ee9-132">Строка</span><span class="sxs-lookup"><span data-stu-id="d9ee9-132">String</span></span>  | <span data-ttu-id="d9ee9-133">Всплывающая подсказка, отображаемая для метки в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="d9ee9-133">The tooltip that should be displayed for the label in a user interface.</span></span>                                      |

## <a name="json-representation"></a><span data-ttu-id="d9ee9-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d9ee9-134">JSON representation</span></span>

<span data-ttu-id="d9ee9-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9ee9-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.labelDetails",
  "baseType": null
}-->

```json
{
  "color": "String",
  "description": "String",
  "id": "String",
  "isActive": true,
  "name": "String",
  "sensitivity": 1024,
  "tooltip": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "labelDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

