---
title: тип ресурса parentLabelDetails
description: Представляет сведения метки родительской метки защиты информации.
localization_priority: Normal
author: tommoser
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8f1ebe58c3968e0f912806eb6f339bcfd499b57a
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679906"
---
# <a name="parentlabeldetails-resource-type"></a><span data-ttu-id="d3d80-103">тип ресурса parentLabelDetails</span><span class="sxs-lookup"><span data-stu-id="d3d80-103">parentLabelDetails resource type</span></span>

<span data-ttu-id="d3d80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3d80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3d80-105">Представляет сведения метки родительской метки защиты информации.</span><span class="sxs-lookup"><span data-stu-id="d3d80-105">Represents the label details of an information protection parent label.</span></span> <span data-ttu-id="d3d80-106">**parentLabelDetails предоставляет** сведения о единой мете защиты информации.</span><span class="sxs-lookup"><span data-stu-id="d3d80-106">**parentLabelDetails** provides information about a single information protection label.</span></span> <span data-ttu-id="d3d80-107">Можно вернуть по [оценкеRemoval,](../api/informationprotectionlabel-evaluateremoval.md) [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)и [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span><span class="sxs-lookup"><span data-stu-id="d3d80-107">Can be returned by [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d3d80-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3d80-108">Properties</span></span>

| <span data-ttu-id="d3d80-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3d80-109">Property</span></span>    | <span data-ttu-id="d3d80-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d3d80-110">Type</span></span>    | <span data-ttu-id="d3d80-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d3d80-111">Description</span></span>                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d3d80-112">color</span><span class="sxs-lookup"><span data-stu-id="d3d80-112">color</span></span>       | <span data-ttu-id="d3d80-113">String</span><span class="sxs-lookup"><span data-stu-id="d3d80-113">String</span></span>  | <span data-ttu-id="d3d80-114">Цвет, который должен отображаться в пользовательском интерфейсе для метки, если настроен.</span><span class="sxs-lookup"><span data-stu-id="d3d80-114">The color that the user interface should display for the label, if configured.</span></span>                               |
| <span data-ttu-id="d3d80-115">description</span><span class="sxs-lookup"><span data-stu-id="d3d80-115">description</span></span> | <span data-ttu-id="d3d80-116">String</span><span class="sxs-lookup"><span data-stu-id="d3d80-116">String</span></span>  | <span data-ttu-id="d3d80-117">Описание метки, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="d3d80-117">The admin-defined description for the label.</span></span>                                                                 |
| <span data-ttu-id="d3d80-118">id</span><span class="sxs-lookup"><span data-stu-id="d3d80-118">id</span></span>          | <span data-ttu-id="d3d80-119">String</span><span class="sxs-lookup"><span data-stu-id="d3d80-119">String</span></span>  | <span data-ttu-id="d3d80-120">Идентификатор метки — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="d3d80-120">The label ID is a globally unique identifier (GUID).</span></span>                                                          |
| <span data-ttu-id="d3d80-121">isActive</span><span class="sxs-lookup"><span data-stu-id="d3d80-121">isActive</span></span>    | <span data-ttu-id="d3d80-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3d80-122">Boolean</span></span> | <span data-ttu-id="d3d80-123">Указывает, активна метка или нет.</span><span class="sxs-lookup"><span data-stu-id="d3d80-123">Indicates whether the label is active or not.</span></span> <span data-ttu-id="d3d80-124">Активные метки должны быть скрыты или отключены в пользовательских интерфейсах.</span><span class="sxs-lookup"><span data-stu-id="d3d80-124">Active labels should be hidden or disabled in user interfaces.</span></span> |
| <span data-ttu-id="d3d80-125">name</span><span class="sxs-lookup"><span data-stu-id="d3d80-125">name</span></span>        | <span data-ttu-id="d3d80-126">String</span><span class="sxs-lookup"><span data-stu-id="d3d80-126">String</span></span>  | <span data-ttu-id="d3d80-127">Простое имя метки.</span><span class="sxs-lookup"><span data-stu-id="d3d80-127">The plaintext name of the label.</span></span>                                                                             |
| <span data-ttu-id="d3d80-128">sensitivity</span><span class="sxs-lookup"><span data-stu-id="d3d80-128">sensitivity</span></span> | <span data-ttu-id="d3d80-129">Int32</span><span class="sxs-lookup"><span data-stu-id="d3d80-129">Int32</span></span>   | <span data-ttu-id="d3d80-130">Значение чувствительности метки, где более низкий уровень менее чувствителен.</span><span class="sxs-lookup"><span data-stu-id="d3d80-130">The sensitivity value of the label, where lower is less sensitive.</span></span>                                           |
| <span data-ttu-id="d3d80-131">tooltip</span><span class="sxs-lookup"><span data-stu-id="d3d80-131">tooltip</span></span>     | <span data-ttu-id="d3d80-132">String</span><span class="sxs-lookup"><span data-stu-id="d3d80-132">String</span></span>  | <span data-ttu-id="d3d80-133">Инструмент, который должен отображаться для метки в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="d3d80-133">The tooltip that should be displayed for the label in a user interface.</span></span>                                      |

## <a name="json-representation"></a><span data-ttu-id="d3d80-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3d80-134">JSON representation</span></span>

<span data-ttu-id="d3d80-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3d80-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.parentLabelDetails",
  "baseType": null
}-->

```json
{
  "color": "String",
  "description": "String",
  "id": "String",
  "isActive": true,
  "name": "String",
  "sensitivity": 1024,
  "tooltip": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "parentLabelDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->