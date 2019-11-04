---
title: Тип ресурса Лабелдетаилс
description: Представляет сведения о метке метки защиты информации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7f2ff99f6f7548e9176358219d70cd55e1232a05
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939175"
---
# <a name="labeldetails-resource-type"></a><span data-ttu-id="97af3-103">Тип ресурса Лабелдетаилс</span><span class="sxs-lookup"><span data-stu-id="97af3-103">labelDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97af3-104">Представляет сведения о метке метки защиты информации.</span><span class="sxs-lookup"><span data-stu-id="97af3-104">Represents the label details of an information protection label.</span></span> <span data-ttu-id="97af3-105">**лабелдетаилс** предоставляет сведения об отдельной метке защиты информации.</span><span class="sxs-lookup"><span data-stu-id="97af3-105">**labelDetails** provides information about a single information protection label.</span></span> <span data-ttu-id="97af3-106">Могут возвращаться [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md), [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md)и [екстрактлабел](../api/informationprotectionlabel-extractLabel.md)</span><span class="sxs-lookup"><span data-stu-id="97af3-106">Can be returned by [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="97af3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="97af3-107">Properties</span></span>

| <span data-ttu-id="97af3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="97af3-108">Property</span></span>    | <span data-ttu-id="97af3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="97af3-109">Type</span></span>    | <span data-ttu-id="97af3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="97af3-110">Description</span></span>                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="97af3-111">color</span><span class="sxs-lookup"><span data-stu-id="97af3-111">color</span></span>       | <span data-ttu-id="97af3-112">String</span><span class="sxs-lookup"><span data-stu-id="97af3-112">String</span></span>  | <span data-ttu-id="97af3-113">Цвет, который должен отображаться в пользовательском интерфейсе для метки, если она настроена.</span><span class="sxs-lookup"><span data-stu-id="97af3-113">The color that the user interface should display for the label, if configured.</span></span>                               |
| <span data-ttu-id="97af3-114">description</span><span class="sxs-lookup"><span data-stu-id="97af3-114">description</span></span> | <span data-ttu-id="97af3-115">Строка</span><span class="sxs-lookup"><span data-stu-id="97af3-115">String</span></span>  | <span data-ttu-id="97af3-116">Заданное администратором описание метки.</span><span class="sxs-lookup"><span data-stu-id="97af3-116">The admin-defined description for the label.</span></span>                                                                 |
| <span data-ttu-id="97af3-117">id</span><span class="sxs-lookup"><span data-stu-id="97af3-117">id</span></span>          | <span data-ttu-id="97af3-118">Строка</span><span class="sxs-lookup"><span data-stu-id="97af3-118">String</span></span>  | <span data-ttu-id="97af3-119">ИДЕНТИФИКАТОР метки является глобальным уникальным идентификатором (GUID).</span><span class="sxs-lookup"><span data-stu-id="97af3-119">The label ID is a globally unique identifier (GUID).</span></span>                                                          |
| <span data-ttu-id="97af3-120">isActive</span><span class="sxs-lookup"><span data-stu-id="97af3-120">isActive</span></span>    | <span data-ttu-id="97af3-121">Логический</span><span class="sxs-lookup"><span data-stu-id="97af3-121">Boolean</span></span> | <span data-ttu-id="97af3-122">Указывает, активна ли метка.</span><span class="sxs-lookup"><span data-stu-id="97af3-122">Indicates whether the label is active or not.</span></span> <span data-ttu-id="97af3-123">Активные метки должны быть скрыты или отключены в пользовательских интерфейсах.</span><span class="sxs-lookup"><span data-stu-id="97af3-123">Active labels should be hidden or disabled in user interfaces.</span></span> |
| <span data-ttu-id="97af3-124">name</span><span class="sxs-lookup"><span data-stu-id="97af3-124">name</span></span>        | <span data-ttu-id="97af3-125">String</span><span class="sxs-lookup"><span data-stu-id="97af3-125">String</span></span>  | <span data-ttu-id="97af3-126">Имя в виде открытого текста метки.</span><span class="sxs-lookup"><span data-stu-id="97af3-126">The plaintext name of the label.</span></span>                                                                             |
| <span data-ttu-id="97af3-127">sensitivity</span><span class="sxs-lookup"><span data-stu-id="97af3-127">sensitivity</span></span> | <span data-ttu-id="97af3-128">Int32</span><span class="sxs-lookup"><span data-stu-id="97af3-128">Int32</span></span>   | <span data-ttu-id="97af3-129">Значение чувствительности метки, где меньше конфиденциально.</span><span class="sxs-lookup"><span data-stu-id="97af3-129">The sensitivity value of the label, where lower is less sensitive.</span></span>                                           |
| <span data-ttu-id="97af3-130">tooltip</span><span class="sxs-lookup"><span data-stu-id="97af3-130">tooltip</span></span>     | <span data-ttu-id="97af3-131">Строка</span><span class="sxs-lookup"><span data-stu-id="97af3-131">String</span></span>  | <span data-ttu-id="97af3-132">Всплывающая подсказка, отображаемая для метки в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="97af3-132">The tooltip that should be displayed for the label in a user interface.</span></span>                                      |

## <a name="json-representation"></a><span data-ttu-id="97af3-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97af3-133">JSON representation</span></span>

<span data-ttu-id="97af3-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97af3-134">The following is a JSON representation of the resource.</span></span>

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