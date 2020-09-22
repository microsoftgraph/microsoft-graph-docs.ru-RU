---
title: Тип ресурса Аддконтентфутерактион
description: Представляет действие, задающее сведения о нижнем колонтитуле контента, добавляемом к данным, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5b4e9edf4007d7bc5d4028e4f9202e09647ca863
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024521"
---
# <a name="addcontentfooteraction-resource-type"></a><span data-ttu-id="0e2ba-103">Тип ресурса Аддконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="0e2ba-103">addContentFooterAction resource type</span></span>

<span data-ttu-id="0e2ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e2ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e2ba-105">Представляет действие, задающее сведения о нижнем колонтитуле контента, добавляемом к данным, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="0e2ba-105">Represents an action that specifies the details on the content footer to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="0e2ba-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e2ba-106">Properties</span></span>

| <span data-ttu-id="0e2ba-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e2ba-107">Property</span></span>      | <span data-ttu-id="0e2ba-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0e2ba-108">Type</span></span>   | <span data-ttu-id="0e2ba-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0e2ba-109">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="0e2ba-110">alignment</span><span class="sxs-lookup"><span data-stu-id="0e2ba-110">alignment</span></span>     | <span data-ttu-id="0e2ba-111">String</span><span class="sxs-lookup"><span data-stu-id="0e2ba-111">String</span></span> | <span data-ttu-id="0e2ba-112">Возможные значения: `left`, `right`, `center`.</span><span class="sxs-lookup"><span data-stu-id="0e2ba-112">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="0e2ba-113">фонтколор</span><span class="sxs-lookup"><span data-stu-id="0e2ba-113">fontColor</span></span>     | <span data-ttu-id="0e2ba-114">String</span><span class="sxs-lookup"><span data-stu-id="0e2ba-114">String</span></span> | <span data-ttu-id="0e2ba-115">Цвет шрифта, который будет использоваться для нижнего колонтитула.</span><span class="sxs-lookup"><span data-stu-id="0e2ba-115">Color of the font to use for the footer.</span></span>                      |
| <span data-ttu-id="0e2ba-116">fontName</span><span class="sxs-lookup"><span data-stu-id="0e2ba-116">fontName</span></span>      | <span data-ttu-id="0e2ba-117">String</span><span class="sxs-lookup"><span data-stu-id="0e2ba-117">String</span></span> | <span data-ttu-id="0e2ba-118">Имя шрифта, который будет использоваться для нижнего колонтитула.</span><span class="sxs-lookup"><span data-stu-id="0e2ba-118">Name of the font to use for the footer.</span></span>                       |
| <span data-ttu-id="0e2ba-119">fontSize</span><span class="sxs-lookup"><span data-stu-id="0e2ba-119">fontSize</span></span>      | <span data-ttu-id="0e2ba-120">Int32</span><span class="sxs-lookup"><span data-stu-id="0e2ba-120">Int32</span></span>  | <span data-ttu-id="0e2ba-121">Размер шрифта, который будет использоваться для нижнего колонтитула.</span><span class="sxs-lookup"><span data-stu-id="0e2ba-121">Font size to use for the footer.</span></span>                              |
| <span data-ttu-id="0e2ba-122">margin</span><span class="sxs-lookup"><span data-stu-id="0e2ba-122">margin</span></span>        | <span data-ttu-id="0e2ba-123">Int32</span><span class="sxs-lookup"><span data-stu-id="0e2ba-123">Int32</span></span>  | <span data-ttu-id="0e2ba-124">Поле заголовка из нижней части документа.</span><span class="sxs-lookup"><span data-stu-id="0e2ba-124">The margin of the header from the bottom of the document.</span></span>     |
| <span data-ttu-id="0e2ba-125">текст</span><span class="sxs-lookup"><span data-stu-id="0e2ba-125">text</span></span>          | <span data-ttu-id="0e2ba-126">String</span><span class="sxs-lookup"><span data-stu-id="0e2ba-126">String</span></span> | <span data-ttu-id="0e2ba-127">Содержимое нижнего колонтитула.</span><span class="sxs-lookup"><span data-stu-id="0e2ba-127">The contents of the footer itself.</span></span>                            |
| <span data-ttu-id="0e2ba-128">уиелементнаме</span><span class="sxs-lookup"><span data-stu-id="0e2ba-128">uiElementName</span></span> | <span data-ttu-id="0e2ba-129">String</span><span class="sxs-lookup"><span data-stu-id="0e2ba-129">String</span></span> | <span data-ttu-id="0e2ba-130">Имя элемента пользовательского интерфейса, в котором следует поместить нижний колонтитул.</span><span class="sxs-lookup"><span data-stu-id="0e2ba-130">The name of the UI element where the footer should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0e2ba-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0e2ba-131">JSON representation</span></span>

<span data-ttu-id="0e2ba-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e2ba-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addContentFooterAction",
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
  "description": "addContentFooterAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

