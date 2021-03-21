---
title: тип ресурса addWatermarkAction
description: Представляет действие, которое указывает сведения о водяном знаке контента, который будет добавлен в сведения, если это применимо.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: db493c57d6de7c840e5f0606743392698cb475b6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962128"
---
# <a name="addwatermarkaction-resource-type"></a><span data-ttu-id="4842f-103">тип ресурса addWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="4842f-103">addWatermarkAction resource type</span></span>

<span data-ttu-id="4842f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4842f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4842f-105">Представляет действие, которое указывает сведения о водяном знаке контента, который будет добавлен в сведения, если это применимо.</span><span class="sxs-lookup"><span data-stu-id="4842f-105">Represents an action that specifies the details on the content watermark to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="4842f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4842f-106">Properties</span></span>

| <span data-ttu-id="4842f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4842f-107">Property</span></span>      | <span data-ttu-id="4842f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4842f-108">Type</span></span>   | <span data-ttu-id="4842f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4842f-109">Description</span></span>                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| <span data-ttu-id="4842f-110">fontColor</span><span class="sxs-lookup"><span data-stu-id="4842f-110">fontColor</span></span>     | <span data-ttu-id="4842f-111">Строка</span><span class="sxs-lookup"><span data-stu-id="4842f-111">String</span></span> | <span data-ttu-id="4842f-112">Цвет шрифта, используемого для водяного знака.</span><span class="sxs-lookup"><span data-stu-id="4842f-112">Color of the font to use for the watermark.</span></span>                      |
| <span data-ttu-id="4842f-113">fontName</span><span class="sxs-lookup"><span data-stu-id="4842f-113">fontName</span></span>      | <span data-ttu-id="4842f-114">Строка</span><span class="sxs-lookup"><span data-stu-id="4842f-114">String</span></span> | <span data-ttu-id="4842f-115">Имя шрифта, используемого для водяного знака.</span><span class="sxs-lookup"><span data-stu-id="4842f-115">Name of the font to use for the watermark.</span></span>                       |
| <span data-ttu-id="4842f-116">fontSize</span><span class="sxs-lookup"><span data-stu-id="4842f-116">fontSize</span></span>      | <span data-ttu-id="4842f-117">Int32</span><span class="sxs-lookup"><span data-stu-id="4842f-117">Int32</span></span>  | <span data-ttu-id="4842f-118">Размер шрифта для водяного знака.</span><span class="sxs-lookup"><span data-stu-id="4842f-118">Font size to use for the watermark.</span></span>                              |
| <span data-ttu-id="4842f-119">макет</span><span class="sxs-lookup"><span data-stu-id="4842f-119">layout</span></span>        | <span data-ttu-id="4842f-120">String</span><span class="sxs-lookup"><span data-stu-id="4842f-120">String</span></span> | <span data-ttu-id="4842f-121">Возможные значения: `horizontal`, `diagonal`.</span><span class="sxs-lookup"><span data-stu-id="4842f-121">Possible values are: `horizontal`, `diagonal`.</span></span>                   |
| <span data-ttu-id="4842f-122">текст</span><span class="sxs-lookup"><span data-stu-id="4842f-122">text</span></span>          | <span data-ttu-id="4842f-123">Строка</span><span class="sxs-lookup"><span data-stu-id="4842f-123">String</span></span> | <span data-ttu-id="4842f-124">Содержимое самого водяного знака.</span><span class="sxs-lookup"><span data-stu-id="4842f-124">The contents of the watermark itself.</span></span>                            |
| <span data-ttu-id="4842f-125">uiElementName</span><span class="sxs-lookup"><span data-stu-id="4842f-125">uiElementName</span></span> | <span data-ttu-id="4842f-126">Строка</span><span class="sxs-lookup"><span data-stu-id="4842f-126">String</span></span> | <span data-ttu-id="4842f-127">Имя элемента пользовательского интерфейса, в котором должен быть размещен водяной знак.</span><span class="sxs-lookup"><span data-stu-id="4842f-127">The name of the UI element where the watermark should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4842f-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4842f-128">JSON representation</span></span>

<span data-ttu-id="4842f-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4842f-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addWatermarkAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "fontColor": "String",
  "fontName": "String",
  "fontSize": 1024,
  "layout": "String",
  "text": "String",
  "uiElementName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addWatermarkAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

