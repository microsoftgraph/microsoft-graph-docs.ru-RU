---
title: Тип ресурса Аддконтенсеадерактион
description: Представляет действие, задающее сведения о заголовке контента, которые будут добавлены к данным (если это возможно).
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d426252b6ab83557c3d3085ac4ffa7a530aae271
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508410"
---
# <a name="addcontentheaderaction-resource-type"></a><span data-ttu-id="ca908-103">Тип ресурса Аддконтенсеадерактион</span><span class="sxs-lookup"><span data-stu-id="ca908-103">addContentHeaderAction resource type</span></span>

<span data-ttu-id="ca908-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ca908-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca908-105">Представляет действие, задающее сведения о заголовке контента, которые будут добавлены к данным (если это возможно).</span><span class="sxs-lookup"><span data-stu-id="ca908-105">Represents an action that specifies the details on the content header to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="ca908-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca908-106">Properties</span></span>

| <span data-ttu-id="ca908-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca908-107">Property</span></span>      | <span data-ttu-id="ca908-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ca908-108">Type</span></span>   | <span data-ttu-id="ca908-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ca908-109">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="ca908-110">alignment</span><span class="sxs-lookup"><span data-stu-id="ca908-110">alignment</span></span>     | <span data-ttu-id="ca908-111">String</span><span class="sxs-lookup"><span data-stu-id="ca908-111">String</span></span> | <span data-ttu-id="ca908-112">Возможные значения: `left`, `right`, `center`.</span><span class="sxs-lookup"><span data-stu-id="ca908-112">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="ca908-113">фонтколор</span><span class="sxs-lookup"><span data-stu-id="ca908-113">fontColor</span></span>     | <span data-ttu-id="ca908-114">String</span><span class="sxs-lookup"><span data-stu-id="ca908-114">String</span></span> | <span data-ttu-id="ca908-115">Цвет шрифта, который будет использоваться для заголовка.</span><span class="sxs-lookup"><span data-stu-id="ca908-115">Color of the font to use for the header.</span></span>                      |
| <span data-ttu-id="ca908-116">fontName</span><span class="sxs-lookup"><span data-stu-id="ca908-116">fontName</span></span>      | <span data-ttu-id="ca908-117">String</span><span class="sxs-lookup"><span data-stu-id="ca908-117">String</span></span> | <span data-ttu-id="ca908-118">Имя шрифта, используемого для заголовка.</span><span class="sxs-lookup"><span data-stu-id="ca908-118">Name of the font to use for the header.</span></span>                       |
| <span data-ttu-id="ca908-119">fontSize</span><span class="sxs-lookup"><span data-stu-id="ca908-119">fontSize</span></span>      | <span data-ttu-id="ca908-120">Int32</span><span class="sxs-lookup"><span data-stu-id="ca908-120">Int32</span></span>  | <span data-ttu-id="ca908-121">Размер шрифта, используемый для заголовка.</span><span class="sxs-lookup"><span data-stu-id="ca908-121">Font size to use for the header.</span></span>                              |
| <span data-ttu-id="ca908-122">поля</span><span class="sxs-lookup"><span data-stu-id="ca908-122">margin</span></span>        | <span data-ttu-id="ca908-123">Int32</span><span class="sxs-lookup"><span data-stu-id="ca908-123">Int32</span></span>  | <span data-ttu-id="ca908-124">Поле заголовка, начиная с верхнего края документа.</span><span class="sxs-lookup"><span data-stu-id="ca908-124">The margin of the header from the top of the document.</span></span>        |
| <span data-ttu-id="ca908-125">текст</span><span class="sxs-lookup"><span data-stu-id="ca908-125">text</span></span>          | <span data-ttu-id="ca908-126">String</span><span class="sxs-lookup"><span data-stu-id="ca908-126">String</span></span> | <span data-ttu-id="ca908-127">Содержимое самого верхнего колонтитула.</span><span class="sxs-lookup"><span data-stu-id="ca908-127">The contents of the header itself.</span></span>                            |
| <span data-ttu-id="ca908-128">уиелементнаме</span><span class="sxs-lookup"><span data-stu-id="ca908-128">uiElementName</span></span> | <span data-ttu-id="ca908-129">String</span><span class="sxs-lookup"><span data-stu-id="ca908-129">String</span></span> | <span data-ttu-id="ca908-130">Имя элемента пользовательского интерфейса, в котором следует поместить заголовок.</span><span class="sxs-lookup"><span data-stu-id="ca908-130">The name of the UI element where the header should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ca908-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca908-131">JSON representation</span></span>

<span data-ttu-id="ca908-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca908-132">The following is a JSON representation of the resource.</span></span>

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