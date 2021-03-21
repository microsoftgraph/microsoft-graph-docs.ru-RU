---
title: тип ресурса addContentFooterAction
description: Представляет действие, которое указывает сведения на подножке контента, которая должна быть добавлена в сведения, если это применимо.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 20debce7dc408bd10d4f62b905efa55156d4d4ca
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962142"
---
# <a name="addcontentfooteraction-resource-type"></a><span data-ttu-id="955d8-103">тип ресурса addContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="955d8-103">addContentFooterAction resource type</span></span>

<span data-ttu-id="955d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="955d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="955d8-105">Представляет действие, которое указывает сведения на подножке контента, которая должна быть добавлена в сведения, если это применимо.</span><span class="sxs-lookup"><span data-stu-id="955d8-105">Represents an action that specifies the details on the content footer to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="955d8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="955d8-106">Properties</span></span>

| <span data-ttu-id="955d8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="955d8-107">Property</span></span>      | <span data-ttu-id="955d8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="955d8-108">Type</span></span>   | <span data-ttu-id="955d8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="955d8-109">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="955d8-110">alignment</span><span class="sxs-lookup"><span data-stu-id="955d8-110">alignment</span></span>     | <span data-ttu-id="955d8-111">Строка</span><span class="sxs-lookup"><span data-stu-id="955d8-111">String</span></span> | <span data-ttu-id="955d8-112">Возможные значения: `left`, `right`, `center`.</span><span class="sxs-lookup"><span data-stu-id="955d8-112">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="955d8-113">fontColor</span><span class="sxs-lookup"><span data-stu-id="955d8-113">fontColor</span></span>     | <span data-ttu-id="955d8-114">Строка</span><span class="sxs-lookup"><span data-stu-id="955d8-114">String</span></span> | <span data-ttu-id="955d8-115">Цвет шрифта, используемого для подножки.</span><span class="sxs-lookup"><span data-stu-id="955d8-115">Color of the font to use for the footer.</span></span>                      |
| <span data-ttu-id="955d8-116">fontName</span><span class="sxs-lookup"><span data-stu-id="955d8-116">fontName</span></span>      | <span data-ttu-id="955d8-117">Строка</span><span class="sxs-lookup"><span data-stu-id="955d8-117">String</span></span> | <span data-ttu-id="955d8-118">Имя шрифта, используемого для подножки.</span><span class="sxs-lookup"><span data-stu-id="955d8-118">Name of the font to use for the footer.</span></span>                       |
| <span data-ttu-id="955d8-119">fontSize</span><span class="sxs-lookup"><span data-stu-id="955d8-119">fontSize</span></span>      | <span data-ttu-id="955d8-120">Int32</span><span class="sxs-lookup"><span data-stu-id="955d8-120">Int32</span></span>  | <span data-ttu-id="955d8-121">Размер шрифта для использования для подножки.</span><span class="sxs-lookup"><span data-stu-id="955d8-121">Font size to use for the footer.</span></span>                              |
| <span data-ttu-id="955d8-122">margin</span><span class="sxs-lookup"><span data-stu-id="955d8-122">margin</span></span>        | <span data-ttu-id="955d8-123">Int32</span><span class="sxs-lookup"><span data-stu-id="955d8-123">Int32</span></span>  | <span data-ttu-id="955d8-124">Поле заглавной строки из нижней части документа.</span><span class="sxs-lookup"><span data-stu-id="955d8-124">The margin of the header from the bottom of the document.</span></span>     |
| <span data-ttu-id="955d8-125">текст</span><span class="sxs-lookup"><span data-stu-id="955d8-125">text</span></span>          | <span data-ttu-id="955d8-126">Строка</span><span class="sxs-lookup"><span data-stu-id="955d8-126">String</span></span> | <span data-ttu-id="955d8-127">Содержимое самого подножки.</span><span class="sxs-lookup"><span data-stu-id="955d8-127">The contents of the footer itself.</span></span>                            |
| <span data-ttu-id="955d8-128">uiElementName</span><span class="sxs-lookup"><span data-stu-id="955d8-128">uiElementName</span></span> | <span data-ttu-id="955d8-129">Строка</span><span class="sxs-lookup"><span data-stu-id="955d8-129">String</span></span> | <span data-ttu-id="955d8-130">Имя элемента пользовательского интерфейса, в котором должен размещаться подножка.</span><span class="sxs-lookup"><span data-stu-id="955d8-130">The name of the UI element where the footer should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="955d8-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="955d8-131">JSON representation</span></span>

<span data-ttu-id="955d8-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="955d8-132">The following is a JSON representation of the resource.</span></span>

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

