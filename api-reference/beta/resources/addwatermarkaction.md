---
title: Тип ресурса Аддватермаркактион
description: Представляет действие, задающее сведения о подложке контента, которую необходимо добавить к сведениям, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2a94f517fe9f5da207febf9e776643a7c17c18d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508403"
---
# <a name="addwatermarkaction-resource-type"></a><span data-ttu-id="b0f7f-103">Тип ресурса Аддватермаркактион</span><span class="sxs-lookup"><span data-stu-id="b0f7f-103">addWatermarkAction resource type</span></span>

<span data-ttu-id="b0f7f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b0f7f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0f7f-105">Представляет действие, задающее сведения о подложке контента, которую необходимо добавить к сведениям, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="b0f7f-105">Represents an action that specifies the details on the content watermark to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="b0f7f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0f7f-106">Properties</span></span>

| <span data-ttu-id="b0f7f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0f7f-107">Property</span></span>      | <span data-ttu-id="b0f7f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b0f7f-108">Type</span></span>   | <span data-ttu-id="b0f7f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b0f7f-109">Description</span></span>                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| <span data-ttu-id="b0f7f-110">фонтколор</span><span class="sxs-lookup"><span data-stu-id="b0f7f-110">fontColor</span></span>     | <span data-ttu-id="b0f7f-111">String</span><span class="sxs-lookup"><span data-stu-id="b0f7f-111">String</span></span> | <span data-ttu-id="b0f7f-112">Цвет шрифта, который будет использоваться для водяного знака.</span><span class="sxs-lookup"><span data-stu-id="b0f7f-112">Color of the font to use for the watermark.</span></span>                      |
| <span data-ttu-id="b0f7f-113">fontName</span><span class="sxs-lookup"><span data-stu-id="b0f7f-113">fontName</span></span>      | <span data-ttu-id="b0f7f-114">String</span><span class="sxs-lookup"><span data-stu-id="b0f7f-114">String</span></span> | <span data-ttu-id="b0f7f-115">Имя шрифта, который будет использоваться для водяного знака.</span><span class="sxs-lookup"><span data-stu-id="b0f7f-115">Name of the font to use for the watermark.</span></span>                       |
| <span data-ttu-id="b0f7f-116">fontSize</span><span class="sxs-lookup"><span data-stu-id="b0f7f-116">fontSize</span></span>      | <span data-ttu-id="b0f7f-117">Int32</span><span class="sxs-lookup"><span data-stu-id="b0f7f-117">Int32</span></span>  | <span data-ttu-id="b0f7f-118">Размер шрифта, используемый для водяного знака.</span><span class="sxs-lookup"><span data-stu-id="b0f7f-118">Font size to use for the watermark.</span></span>                              |
| <span data-ttu-id="b0f7f-119">макет</span><span class="sxs-lookup"><span data-stu-id="b0f7f-119">layout</span></span>        | <span data-ttu-id="b0f7f-120">String</span><span class="sxs-lookup"><span data-stu-id="b0f7f-120">String</span></span> | <span data-ttu-id="b0f7f-121">Возможные значения: `horizontal`, `diagonal`.</span><span class="sxs-lookup"><span data-stu-id="b0f7f-121">Possible values are: `horizontal`, `diagonal`.</span></span>                   |
| <span data-ttu-id="b0f7f-122">текст</span><span class="sxs-lookup"><span data-stu-id="b0f7f-122">text</span></span>          | <span data-ttu-id="b0f7f-123">String</span><span class="sxs-lookup"><span data-stu-id="b0f7f-123">String</span></span> | <span data-ttu-id="b0f7f-124">Содержимое водяного знака.</span><span class="sxs-lookup"><span data-stu-id="b0f7f-124">The contents of the watermark itself.</span></span>                            |
| <span data-ttu-id="b0f7f-125">уиелементнаме</span><span class="sxs-lookup"><span data-stu-id="b0f7f-125">uiElementName</span></span> | <span data-ttu-id="b0f7f-126">String</span><span class="sxs-lookup"><span data-stu-id="b0f7f-126">String</span></span> | <span data-ttu-id="b0f7f-127">Имя элемента пользовательского интерфейса, в котором следует поместить водяной знак.</span><span class="sxs-lookup"><span data-stu-id="b0f7f-127">The name of the UI element where the watermark should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b0f7f-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0f7f-128">JSON representation</span></span>

<span data-ttu-id="b0f7f-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0f7f-129">The following is a JSON representation of the resource.</span></span>

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