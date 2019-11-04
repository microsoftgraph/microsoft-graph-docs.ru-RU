---
title: Тип ресурса Аддватермаркактион
description: Представляет действие, задающее сведения о подложке контента, которую необходимо добавить к сведениям, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4ba3bd679d01d31aec779071a766ab804761e614
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939168"
---
# <a name="addwatermarkaction-resource-type"></a><span data-ttu-id="a4952-103">Тип ресурса Аддватермаркактион</span><span class="sxs-lookup"><span data-stu-id="a4952-103">addWatermarkAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4952-104">Представляет действие, задающее сведения о подложке контента, которую необходимо добавить к сведениям, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="a4952-104">Represents an action that specifies the details on the content watermark to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="a4952-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4952-105">Properties</span></span>

| <span data-ttu-id="a4952-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4952-106">Property</span></span>      | <span data-ttu-id="a4952-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a4952-107">Type</span></span>   | <span data-ttu-id="a4952-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a4952-108">Description</span></span>                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| <span data-ttu-id="a4952-109">фонтколор</span><span class="sxs-lookup"><span data-stu-id="a4952-109">fontColor</span></span>     | <span data-ttu-id="a4952-110">Строка</span><span class="sxs-lookup"><span data-stu-id="a4952-110">String</span></span> | <span data-ttu-id="a4952-111">Цвет шрифта, который будет использоваться для водяного знака.</span><span class="sxs-lookup"><span data-stu-id="a4952-111">Color of the font to use for the watermark.</span></span>                      |
| <span data-ttu-id="a4952-112">fontName</span><span class="sxs-lookup"><span data-stu-id="a4952-112">fontName</span></span>      | <span data-ttu-id="a4952-113">Строка</span><span class="sxs-lookup"><span data-stu-id="a4952-113">String</span></span> | <span data-ttu-id="a4952-114">Имя шрифта, который будет использоваться для водяного знака.</span><span class="sxs-lookup"><span data-stu-id="a4952-114">Name of the font to use for the watermark.</span></span>                       |
| <span data-ttu-id="a4952-115">fontSize</span><span class="sxs-lookup"><span data-stu-id="a4952-115">fontSize</span></span>      | <span data-ttu-id="a4952-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a4952-116">Int32</span></span>  | <span data-ttu-id="a4952-117">Размер шрифта, используемый для водяного знака.</span><span class="sxs-lookup"><span data-stu-id="a4952-117">Font size to use for the watermark.</span></span>                              |
| <span data-ttu-id="a4952-118">макет</span><span class="sxs-lookup"><span data-stu-id="a4952-118">layout</span></span>        | <span data-ttu-id="a4952-119">String</span><span class="sxs-lookup"><span data-stu-id="a4952-119">String</span></span> | <span data-ttu-id="a4952-120">Возможные значения: `horizontal`, `diagonal`.</span><span class="sxs-lookup"><span data-stu-id="a4952-120">Possible values are: `horizontal`, `diagonal`.</span></span>                   |
| <span data-ttu-id="a4952-121">текст</span><span class="sxs-lookup"><span data-stu-id="a4952-121">text</span></span>          | <span data-ttu-id="a4952-122">Строка</span><span class="sxs-lookup"><span data-stu-id="a4952-122">String</span></span> | <span data-ttu-id="a4952-123">Содержимое водяного знака.</span><span class="sxs-lookup"><span data-stu-id="a4952-123">The contents of the watermark itself.</span></span>                            |
| <span data-ttu-id="a4952-124">уиелементнаме</span><span class="sxs-lookup"><span data-stu-id="a4952-124">uiElementName</span></span> | <span data-ttu-id="a4952-125">Строка</span><span class="sxs-lookup"><span data-stu-id="a4952-125">String</span></span> | <span data-ttu-id="a4952-126">Имя элемента пользовательского интерфейса, в котором следует поместить водяной знак.</span><span class="sxs-lookup"><span data-stu-id="a4952-126">The name of the UI element where the watermark should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a4952-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4952-127">JSON representation</span></span>

<span data-ttu-id="a4952-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4952-128">The following is a JSON representation of the resource.</span></span>

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