---
title: Тип ресурса Аддконтенсеадерактион
description: Представляет действие, задающее сведения о заголовке контента, которые будут добавлены к данным (если это возможно).
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 341af43f03d8a319c7aaec535681f21db0a7f7f4
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939109"
---
# <a name="addcontentheaderaction-resource-type"></a><span data-ttu-id="eea06-103">Тип ресурса Аддконтенсеадерактион</span><span class="sxs-lookup"><span data-stu-id="eea06-103">addContentHeaderAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eea06-104">Представляет действие, задающее сведения о заголовке контента, которые будут добавлены к данным (если это возможно).</span><span class="sxs-lookup"><span data-stu-id="eea06-104">Represents an action that specifies the details on the content header to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="eea06-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="eea06-105">Properties</span></span>

| <span data-ttu-id="eea06-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="eea06-106">Property</span></span>      | <span data-ttu-id="eea06-107">Тип</span><span class="sxs-lookup"><span data-stu-id="eea06-107">Type</span></span>   | <span data-ttu-id="eea06-108">Описание</span><span class="sxs-lookup"><span data-stu-id="eea06-108">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="eea06-109">alignment</span><span class="sxs-lookup"><span data-stu-id="eea06-109">alignment</span></span>     | <span data-ttu-id="eea06-110">Строка</span><span class="sxs-lookup"><span data-stu-id="eea06-110">String</span></span> | <span data-ttu-id="eea06-111">Возможные значения: `left`, `right`, `center`.</span><span class="sxs-lookup"><span data-stu-id="eea06-111">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="eea06-112">фонтколор</span><span class="sxs-lookup"><span data-stu-id="eea06-112">fontColor</span></span>     | <span data-ttu-id="eea06-113">Строка</span><span class="sxs-lookup"><span data-stu-id="eea06-113">String</span></span> | <span data-ttu-id="eea06-114">Цвет шрифта, который будет использоваться для заголовка.</span><span class="sxs-lookup"><span data-stu-id="eea06-114">Color of the font to use for the header.</span></span>                      |
| <span data-ttu-id="eea06-115">fontName</span><span class="sxs-lookup"><span data-stu-id="eea06-115">fontName</span></span>      | <span data-ttu-id="eea06-116">Строка</span><span class="sxs-lookup"><span data-stu-id="eea06-116">String</span></span> | <span data-ttu-id="eea06-117">Имя шрифта, используемого для заголовка.</span><span class="sxs-lookup"><span data-stu-id="eea06-117">Name of the font to use for the header.</span></span>                       |
| <span data-ttu-id="eea06-118">fontSize</span><span class="sxs-lookup"><span data-stu-id="eea06-118">fontSize</span></span>      | <span data-ttu-id="eea06-119">Int32</span><span class="sxs-lookup"><span data-stu-id="eea06-119">Int32</span></span>  | <span data-ttu-id="eea06-120">Размер шрифта, используемый для заголовка.</span><span class="sxs-lookup"><span data-stu-id="eea06-120">Font size to use for the header.</span></span>                              |
| <span data-ttu-id="eea06-121">поля</span><span class="sxs-lookup"><span data-stu-id="eea06-121">margin</span></span>        | <span data-ttu-id="eea06-122">Int32</span><span class="sxs-lookup"><span data-stu-id="eea06-122">Int32</span></span>  | <span data-ttu-id="eea06-123">Поле заголовка, начиная с верхнего края документа.</span><span class="sxs-lookup"><span data-stu-id="eea06-123">The margin of the header from the top of the document.</span></span>        |
| <span data-ttu-id="eea06-124">текст</span><span class="sxs-lookup"><span data-stu-id="eea06-124">text</span></span>          | <span data-ttu-id="eea06-125">Строка</span><span class="sxs-lookup"><span data-stu-id="eea06-125">String</span></span> | <span data-ttu-id="eea06-126">Содержимое самого верхнего колонтитула.</span><span class="sxs-lookup"><span data-stu-id="eea06-126">The contents of the header itself.</span></span>                            |
| <span data-ttu-id="eea06-127">уиелементнаме</span><span class="sxs-lookup"><span data-stu-id="eea06-127">uiElementName</span></span> | <span data-ttu-id="eea06-128">Строка</span><span class="sxs-lookup"><span data-stu-id="eea06-128">String</span></span> | <span data-ttu-id="eea06-129">Имя элемента пользовательского интерфейса, в котором следует поместить заголовок.</span><span class="sxs-lookup"><span data-stu-id="eea06-129">The name of the UI element where the header should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eea06-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eea06-130">JSON representation</span></span>

<span data-ttu-id="eea06-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eea06-131">The following is a JSON representation of the resource.</span></span>

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