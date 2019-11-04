---
title: Тип ресурса Аддконтентфутерактион
description: Представляет действие, задающее сведения о нижнем колонтитуле контента, добавляемом к данным, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b1a2cb0f3e2ffbfb5554c4ae0323cf4fd028e0c8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939111"
---
# <a name="addcontentfooteraction-resource-type"></a><span data-ttu-id="0ca18-103">Тип ресурса Аддконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="0ca18-103">addContentFooterAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ca18-104">Представляет действие, задающее сведения о нижнем колонтитуле контента, добавляемом к данным, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="0ca18-104">Represents an action that specifies the details on the content footer to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="0ca18-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ca18-105">Properties</span></span>

| <span data-ttu-id="0ca18-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ca18-106">Property</span></span>      | <span data-ttu-id="0ca18-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0ca18-107">Type</span></span>   | <span data-ttu-id="0ca18-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0ca18-108">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="0ca18-109">alignment</span><span class="sxs-lookup"><span data-stu-id="0ca18-109">alignment</span></span>     | <span data-ttu-id="0ca18-110">Строка</span><span class="sxs-lookup"><span data-stu-id="0ca18-110">String</span></span> | <span data-ttu-id="0ca18-111">Возможные значения: `left`, `right`, `center`.</span><span class="sxs-lookup"><span data-stu-id="0ca18-111">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="0ca18-112">фонтколор</span><span class="sxs-lookup"><span data-stu-id="0ca18-112">fontColor</span></span>     | <span data-ttu-id="0ca18-113">Строка</span><span class="sxs-lookup"><span data-stu-id="0ca18-113">String</span></span> | <span data-ttu-id="0ca18-114">Цвет шрифта, который будет использоваться для нижнего колонтитула.</span><span class="sxs-lookup"><span data-stu-id="0ca18-114">Color of the font to use for the footer.</span></span>                      |
| <span data-ttu-id="0ca18-115">fontName</span><span class="sxs-lookup"><span data-stu-id="0ca18-115">fontName</span></span>      | <span data-ttu-id="0ca18-116">Строка</span><span class="sxs-lookup"><span data-stu-id="0ca18-116">String</span></span> | <span data-ttu-id="0ca18-117">Имя шрифта, который будет использоваться для нижнего колонтитула.</span><span class="sxs-lookup"><span data-stu-id="0ca18-117">Name of the font to use for the footer.</span></span>                       |
| <span data-ttu-id="0ca18-118">fontSize</span><span class="sxs-lookup"><span data-stu-id="0ca18-118">fontSize</span></span>      | <span data-ttu-id="0ca18-119">Int32</span><span class="sxs-lookup"><span data-stu-id="0ca18-119">Int32</span></span>  | <span data-ttu-id="0ca18-120">Размер шрифта, который будет использоваться для нижнего колонтитула.</span><span class="sxs-lookup"><span data-stu-id="0ca18-120">Font size to use for the footer.</span></span>                              |
| <span data-ttu-id="0ca18-121">поля</span><span class="sxs-lookup"><span data-stu-id="0ca18-121">margin</span></span>        | <span data-ttu-id="0ca18-122">Int32</span><span class="sxs-lookup"><span data-stu-id="0ca18-122">Int32</span></span>  | <span data-ttu-id="0ca18-123">Поле заголовка из нижней части документа.</span><span class="sxs-lookup"><span data-stu-id="0ca18-123">The margin of the header from the bottom of the document.</span></span>     |
| <span data-ttu-id="0ca18-124">текст</span><span class="sxs-lookup"><span data-stu-id="0ca18-124">text</span></span>          | <span data-ttu-id="0ca18-125">Строка</span><span class="sxs-lookup"><span data-stu-id="0ca18-125">String</span></span> | <span data-ttu-id="0ca18-126">Содержимое нижнего колонтитула.</span><span class="sxs-lookup"><span data-stu-id="0ca18-126">The contents of the footer itself.</span></span>                            |
| <span data-ttu-id="0ca18-127">уиелементнаме</span><span class="sxs-lookup"><span data-stu-id="0ca18-127">uiElementName</span></span> | <span data-ttu-id="0ca18-128">Строка</span><span class="sxs-lookup"><span data-stu-id="0ca18-128">String</span></span> | <span data-ttu-id="0ca18-129">Имя элемента пользовательского интерфейса, в котором следует поместить нижний колонтитул.</span><span class="sxs-lookup"><span data-stu-id="0ca18-129">The name of the UI element where the footer should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0ca18-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ca18-130">JSON representation</span></span>

<span data-ttu-id="0ca18-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ca18-131">The following is a JSON representation of the resource.</span></span>

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