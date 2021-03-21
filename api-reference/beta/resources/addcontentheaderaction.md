---
title: тип ресурса addContentHeaderAction
description: Представляет действие, которое указывает сведения о загонщике контента, который будет добавлен в сведения, если это применимо.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 65754bffc034611fd319403cd81d931addfea9f0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962139"
---
# <a name="addcontentheaderaction-resource-type"></a><span data-ttu-id="b53b2-103">тип ресурса addContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="b53b2-103">addContentHeaderAction resource type</span></span>

<span data-ttu-id="b53b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b53b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b53b2-105">Представляет действие, которое указывает сведения о загонщике контента, который будет добавлен в сведения, если это применимо.</span><span class="sxs-lookup"><span data-stu-id="b53b2-105">Represents an action that specifies the details on the content header to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="b53b2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b53b2-106">Properties</span></span>

| <span data-ttu-id="b53b2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b53b2-107">Property</span></span>      | <span data-ttu-id="b53b2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b53b2-108">Type</span></span>   | <span data-ttu-id="b53b2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b53b2-109">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="b53b2-110">alignment</span><span class="sxs-lookup"><span data-stu-id="b53b2-110">alignment</span></span>     | <span data-ttu-id="b53b2-111">Строка</span><span class="sxs-lookup"><span data-stu-id="b53b2-111">String</span></span> | <span data-ttu-id="b53b2-112">Возможные значения: `left`, `right`, `center`.</span><span class="sxs-lookup"><span data-stu-id="b53b2-112">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="b53b2-113">fontColor</span><span class="sxs-lookup"><span data-stu-id="b53b2-113">fontColor</span></span>     | <span data-ttu-id="b53b2-114">Строка</span><span class="sxs-lookup"><span data-stu-id="b53b2-114">String</span></span> | <span data-ttu-id="b53b2-115">Цвет шрифта, используемого для загона.</span><span class="sxs-lookup"><span data-stu-id="b53b2-115">Color of the font to use for the header.</span></span>                      |
| <span data-ttu-id="b53b2-116">fontName</span><span class="sxs-lookup"><span data-stu-id="b53b2-116">fontName</span></span>      | <span data-ttu-id="b53b2-117">Строка</span><span class="sxs-lookup"><span data-stu-id="b53b2-117">String</span></span> | <span data-ttu-id="b53b2-118">Имя шрифта, используемого для загона.</span><span class="sxs-lookup"><span data-stu-id="b53b2-118">Name of the font to use for the header.</span></span>                       |
| <span data-ttu-id="b53b2-119">fontSize</span><span class="sxs-lookup"><span data-stu-id="b53b2-119">fontSize</span></span>      | <span data-ttu-id="b53b2-120">Int32</span><span class="sxs-lookup"><span data-stu-id="b53b2-120">Int32</span></span>  | <span data-ttu-id="b53b2-121">Размер шрифта, который можно использовать для загона.</span><span class="sxs-lookup"><span data-stu-id="b53b2-121">Font size to use for the header.</span></span>                              |
| <span data-ttu-id="b53b2-122">margin</span><span class="sxs-lookup"><span data-stu-id="b53b2-122">margin</span></span>        | <span data-ttu-id="b53b2-123">Int32</span><span class="sxs-lookup"><span data-stu-id="b53b2-123">Int32</span></span>  | <span data-ttu-id="b53b2-124">Поле загонщика в верхней части документа.</span><span class="sxs-lookup"><span data-stu-id="b53b2-124">The margin of the header from the top of the document.</span></span>        |
| <span data-ttu-id="b53b2-125">текст</span><span class="sxs-lookup"><span data-stu-id="b53b2-125">text</span></span>          | <span data-ttu-id="b53b2-126">Строка</span><span class="sxs-lookup"><span data-stu-id="b53b2-126">String</span></span> | <span data-ttu-id="b53b2-127">Содержимое самого загона.</span><span class="sxs-lookup"><span data-stu-id="b53b2-127">The contents of the header itself.</span></span>                            |
| <span data-ttu-id="b53b2-128">uiElementName</span><span class="sxs-lookup"><span data-stu-id="b53b2-128">uiElementName</span></span> | <span data-ttu-id="b53b2-129">Строка</span><span class="sxs-lookup"><span data-stu-id="b53b2-129">String</span></span> | <span data-ttu-id="b53b2-130">Имя элемента пользовательского интерфейса, в котором должен быть размещен заголовщик.</span><span class="sxs-lookup"><span data-stu-id="b53b2-130">The name of the UI element where the header should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b53b2-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b53b2-131">JSON representation</span></span>

<span data-ttu-id="b53b2-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b53b2-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addContentHeaderAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "alignment": "String",
  "fontColor": "String",
  "fontName": "String",
  "fontSize": 1024,
  "margin": 1024,
  "text": "String",
  "uiElementName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addContentHeaderAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

