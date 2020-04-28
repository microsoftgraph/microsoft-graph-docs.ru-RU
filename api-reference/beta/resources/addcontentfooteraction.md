---
title: Тип ресурса Аддконтентфутерактион
description: Представляет действие, задающее сведения о нижнем колонтитуле контента, добавляемом к данным, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 05bbd7ee4b2d4b2b9c4e772b19bd26c86d91cc69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508424"
---
# <a name="addcontentfooteraction-resource-type"></a><span data-ttu-id="b8da8-103">Тип ресурса Аддконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="b8da8-103">addContentFooterAction resource type</span></span>

<span data-ttu-id="b8da8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8da8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8da8-105">Представляет действие, задающее сведения о нижнем колонтитуле контента, добавляемом к данным, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="b8da8-105">Represents an action that specifies the details on the content footer to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="b8da8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8da8-106">Properties</span></span>

| <span data-ttu-id="b8da8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8da8-107">Property</span></span>      | <span data-ttu-id="b8da8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b8da8-108">Type</span></span>   | <span data-ttu-id="b8da8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b8da8-109">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="b8da8-110">alignment</span><span class="sxs-lookup"><span data-stu-id="b8da8-110">alignment</span></span>     | <span data-ttu-id="b8da8-111">String</span><span class="sxs-lookup"><span data-stu-id="b8da8-111">String</span></span> | <span data-ttu-id="b8da8-112">Возможные значения: `left`, `right`, `center`.</span><span class="sxs-lookup"><span data-stu-id="b8da8-112">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="b8da8-113">фонтколор</span><span class="sxs-lookup"><span data-stu-id="b8da8-113">fontColor</span></span>     | <span data-ttu-id="b8da8-114">String</span><span class="sxs-lookup"><span data-stu-id="b8da8-114">String</span></span> | <span data-ttu-id="b8da8-115">Цвет шрифта, который будет использоваться для нижнего колонтитула.</span><span class="sxs-lookup"><span data-stu-id="b8da8-115">Color of the font to use for the footer.</span></span>                      |
| <span data-ttu-id="b8da8-116">fontName</span><span class="sxs-lookup"><span data-stu-id="b8da8-116">fontName</span></span>      | <span data-ttu-id="b8da8-117">String</span><span class="sxs-lookup"><span data-stu-id="b8da8-117">String</span></span> | <span data-ttu-id="b8da8-118">Имя шрифта, который будет использоваться для нижнего колонтитула.</span><span class="sxs-lookup"><span data-stu-id="b8da8-118">Name of the font to use for the footer.</span></span>                       |
| <span data-ttu-id="b8da8-119">fontSize</span><span class="sxs-lookup"><span data-stu-id="b8da8-119">fontSize</span></span>      | <span data-ttu-id="b8da8-120">Int32</span><span class="sxs-lookup"><span data-stu-id="b8da8-120">Int32</span></span>  | <span data-ttu-id="b8da8-121">Размер шрифта, который будет использоваться для нижнего колонтитула.</span><span class="sxs-lookup"><span data-stu-id="b8da8-121">Font size to use for the footer.</span></span>                              |
| <span data-ttu-id="b8da8-122">поля</span><span class="sxs-lookup"><span data-stu-id="b8da8-122">margin</span></span>        | <span data-ttu-id="b8da8-123">Int32</span><span class="sxs-lookup"><span data-stu-id="b8da8-123">Int32</span></span>  | <span data-ttu-id="b8da8-124">Поле заголовка из нижней части документа.</span><span class="sxs-lookup"><span data-stu-id="b8da8-124">The margin of the header from the bottom of the document.</span></span>     |
| <span data-ttu-id="b8da8-125">текст</span><span class="sxs-lookup"><span data-stu-id="b8da8-125">text</span></span>          | <span data-ttu-id="b8da8-126">String</span><span class="sxs-lookup"><span data-stu-id="b8da8-126">String</span></span> | <span data-ttu-id="b8da8-127">Содержимое нижнего колонтитула.</span><span class="sxs-lookup"><span data-stu-id="b8da8-127">The contents of the footer itself.</span></span>                            |
| <span data-ttu-id="b8da8-128">уиелементнаме</span><span class="sxs-lookup"><span data-stu-id="b8da8-128">uiElementName</span></span> | <span data-ttu-id="b8da8-129">String</span><span class="sxs-lookup"><span data-stu-id="b8da8-129">String</span></span> | <span data-ttu-id="b8da8-130">Имя элемента пользовательского интерфейса, в котором следует поместить нижний колонтитул.</span><span class="sxs-lookup"><span data-stu-id="b8da8-130">The name of the UI element where the footer should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b8da8-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8da8-131">JSON representation</span></span>

<span data-ttu-id="b8da8-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8da8-132">The following is a JSON representation of the resource.</span></span>

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