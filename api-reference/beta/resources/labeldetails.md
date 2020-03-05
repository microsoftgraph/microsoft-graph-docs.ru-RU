---
title: Тип ресурса Лабелдетаилс
description: Представляет сведения о метке метки защиты информации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cf031459004e0c0d56b5b09145ed897a9f960142
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523011"
---
# <a name="labeldetails-resource-type"></a><span data-ttu-id="bcd82-103">Тип ресурса Лабелдетаилс</span><span class="sxs-lookup"><span data-stu-id="bcd82-103">labelDetails resource type</span></span>

<span data-ttu-id="bcd82-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bcd82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcd82-105">Представляет сведения о метке метки защиты информации.</span><span class="sxs-lookup"><span data-stu-id="bcd82-105">Represents the label details of an information protection label.</span></span> <span data-ttu-id="bcd82-106">**лабелдетаилс** предоставляет сведения об отдельной метке защиты информации.</span><span class="sxs-lookup"><span data-stu-id="bcd82-106">**labelDetails** provides information about a single information protection label.</span></span> <span data-ttu-id="bcd82-107">Могут возвращаться [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md), [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md)и [екстрактлабел](../api/informationprotectionlabel-extractLabel.md)</span><span class="sxs-lookup"><span data-stu-id="bcd82-107">Can be returned by [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bcd82-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bcd82-108">Properties</span></span>

| <span data-ttu-id="bcd82-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bcd82-109">Property</span></span>    | <span data-ttu-id="bcd82-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bcd82-110">Type</span></span>    | <span data-ttu-id="bcd82-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bcd82-111">Description</span></span>                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="bcd82-112">color</span><span class="sxs-lookup"><span data-stu-id="bcd82-112">color</span></span>       | <span data-ttu-id="bcd82-113">String</span><span class="sxs-lookup"><span data-stu-id="bcd82-113">String</span></span>  | <span data-ttu-id="bcd82-114">Цвет, который должен отображаться в пользовательском интерфейсе для метки, если она настроена.</span><span class="sxs-lookup"><span data-stu-id="bcd82-114">The color that the user interface should display for the label, if configured.</span></span>                               |
| <span data-ttu-id="bcd82-115">description</span><span class="sxs-lookup"><span data-stu-id="bcd82-115">description</span></span> | <span data-ttu-id="bcd82-116">String</span><span class="sxs-lookup"><span data-stu-id="bcd82-116">String</span></span>  | <span data-ttu-id="bcd82-117">Заданное администратором описание метки.</span><span class="sxs-lookup"><span data-stu-id="bcd82-117">The admin-defined description for the label.</span></span>                                                                 |
| <span data-ttu-id="bcd82-118">id</span><span class="sxs-lookup"><span data-stu-id="bcd82-118">id</span></span>          | <span data-ttu-id="bcd82-119">Строка</span><span class="sxs-lookup"><span data-stu-id="bcd82-119">String</span></span>  | <span data-ttu-id="bcd82-120">ИДЕНТИФИКАТОР метки является глобальным уникальным идентификатором (GUID).</span><span class="sxs-lookup"><span data-stu-id="bcd82-120">The label ID is a globally unique identifier (GUID).</span></span>                                                          |
| <span data-ttu-id="bcd82-121">isActive</span><span class="sxs-lookup"><span data-stu-id="bcd82-121">isActive</span></span>    | <span data-ttu-id="bcd82-122">Логический</span><span class="sxs-lookup"><span data-stu-id="bcd82-122">Boolean</span></span> | <span data-ttu-id="bcd82-123">Указывает, активна ли метка.</span><span class="sxs-lookup"><span data-stu-id="bcd82-123">Indicates whether the label is active or not.</span></span> <span data-ttu-id="bcd82-124">Активные метки должны быть скрыты или отключены в пользовательских интерфейсах.</span><span class="sxs-lookup"><span data-stu-id="bcd82-124">Active labels should be hidden or disabled in user interfaces.</span></span> |
| <span data-ttu-id="bcd82-125">name</span><span class="sxs-lookup"><span data-stu-id="bcd82-125">name</span></span>        | <span data-ttu-id="bcd82-126">String</span><span class="sxs-lookup"><span data-stu-id="bcd82-126">String</span></span>  | <span data-ttu-id="bcd82-127">Имя в виде открытого текста метки.</span><span class="sxs-lookup"><span data-stu-id="bcd82-127">The plaintext name of the label.</span></span>                                                                             |
| <span data-ttu-id="bcd82-128">sensitivity</span><span class="sxs-lookup"><span data-stu-id="bcd82-128">sensitivity</span></span> | <span data-ttu-id="bcd82-129">Int32</span><span class="sxs-lookup"><span data-stu-id="bcd82-129">Int32</span></span>   | <span data-ttu-id="bcd82-130">Значение чувствительности метки, где меньше конфиденциально.</span><span class="sxs-lookup"><span data-stu-id="bcd82-130">The sensitivity value of the label, where lower is less sensitive.</span></span>                                           |
| <span data-ttu-id="bcd82-131">tooltip</span><span class="sxs-lookup"><span data-stu-id="bcd82-131">tooltip</span></span>     | <span data-ttu-id="bcd82-132">String</span><span class="sxs-lookup"><span data-stu-id="bcd82-132">String</span></span>  | <span data-ttu-id="bcd82-133">Всплывающая подсказка, отображаемая для метки в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="bcd82-133">The tooltip that should be displayed for the label in a user interface.</span></span>                                      |

## <a name="json-representation"></a><span data-ttu-id="bcd82-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bcd82-134">JSON representation</span></span>

<span data-ttu-id="bcd82-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bcd82-135">The following is a JSON representation of the resource.</span></span>

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