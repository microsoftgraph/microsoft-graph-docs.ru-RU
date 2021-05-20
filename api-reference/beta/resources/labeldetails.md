---
title: тип ресурса labelDetails
description: Представляет сведения метки защиты информации.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: eb66e395d18b7887942753abdebd91d398844290
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579302"
---
# <a name="labeldetails-resource-type"></a><span data-ttu-id="9bd7e-103">тип ресурса labelDetails</span><span class="sxs-lookup"><span data-stu-id="9bd7e-103">labelDetails resource type</span></span>

<span data-ttu-id="9bd7e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bd7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bd7e-105">Представляет сведения метки защиты информации.</span><span class="sxs-lookup"><span data-stu-id="9bd7e-105">Represents the label details of an information protection label.</span></span> <span data-ttu-id="9bd7e-106">**LabelDetails предоставляет** сведения о единой мете защиты информации.</span><span class="sxs-lookup"><span data-stu-id="9bd7e-106">**labelDetails** provides information about a single information protection label.</span></span> <span data-ttu-id="9bd7e-107">Наследует от [parentLabelDetails](parentlabeldetails.md).</span><span class="sxs-lookup"><span data-stu-id="9bd7e-107">Inherits from the [parentLabelDetails](parentlabeldetails.md).</span></span> <span data-ttu-id="9bd7e-108">Можно вернуть по [оценкеRemoval,](../api/informationprotectionlabel-evaluateremoval.md) [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)и [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span><span class="sxs-lookup"><span data-stu-id="9bd7e-108">Can be returned by [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9bd7e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9bd7e-109">Properties</span></span>

| <span data-ttu-id="9bd7e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bd7e-110">Property</span></span>    | <span data-ttu-id="9bd7e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9bd7e-111">Type</span></span>                                         | <span data-ttu-id="9bd7e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9bd7e-112">Description</span></span>                                                                                                  |
| :---------- | :------------------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9bd7e-113">color</span><span class="sxs-lookup"><span data-stu-id="9bd7e-113">color</span></span>       | <span data-ttu-id="9bd7e-114">String</span><span class="sxs-lookup"><span data-stu-id="9bd7e-114">String</span></span>                                       | <span data-ttu-id="9bd7e-115">Цвет, который должен отображаться в пользовательском интерфейсе для метки, если настроен.</span><span class="sxs-lookup"><span data-stu-id="9bd7e-115">The color that the user interface should display for the label, if configured.</span></span>                               |
| <span data-ttu-id="9bd7e-116">description</span><span class="sxs-lookup"><span data-stu-id="9bd7e-116">description</span></span> | <span data-ttu-id="9bd7e-117">Строка</span><span class="sxs-lookup"><span data-stu-id="9bd7e-117">String</span></span>                                       | <span data-ttu-id="9bd7e-118">Описание метки, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="9bd7e-118">The admin-defined description for the label.</span></span>                                                                 |
| <span data-ttu-id="9bd7e-119">id</span><span class="sxs-lookup"><span data-stu-id="9bd7e-119">id</span></span>          | <span data-ttu-id="9bd7e-120">Строка</span><span class="sxs-lookup"><span data-stu-id="9bd7e-120">String</span></span>                                       | <span data-ttu-id="9bd7e-121">Идентификатор метки — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="9bd7e-121">The label ID is a globally unique identifier (GUID).</span></span>                                                         |
| <span data-ttu-id="9bd7e-122">isActive</span><span class="sxs-lookup"><span data-stu-id="9bd7e-122">isActive</span></span>    | <span data-ttu-id="9bd7e-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bd7e-123">Boolean</span></span>                                      | <span data-ttu-id="9bd7e-124">Указывает, активна метка или нет.</span><span class="sxs-lookup"><span data-stu-id="9bd7e-124">Indicates whether the label is active or not.</span></span> <span data-ttu-id="9bd7e-125">Активные метки должны быть скрыты или отключены в пользовательских интерфейсах.</span><span class="sxs-lookup"><span data-stu-id="9bd7e-125">Active labels should be hidden or disabled in user interfaces.</span></span> |
| <span data-ttu-id="9bd7e-126">name</span><span class="sxs-lookup"><span data-stu-id="9bd7e-126">name</span></span>        | <span data-ttu-id="9bd7e-127">String</span><span class="sxs-lookup"><span data-stu-id="9bd7e-127">String</span></span>                                       | <span data-ttu-id="9bd7e-128">Простое имя метки.</span><span class="sxs-lookup"><span data-stu-id="9bd7e-128">The plaintext name of the label.</span></span>                                                                             |
| <span data-ttu-id="9bd7e-129">sensitivity</span><span class="sxs-lookup"><span data-stu-id="9bd7e-129">sensitivity</span></span> | <span data-ttu-id="9bd7e-130">Int32</span><span class="sxs-lookup"><span data-stu-id="9bd7e-130">Int32</span></span>                                        | <span data-ttu-id="9bd7e-131">Значение чувствительности метки, где более низкий уровень менее чувствителен.</span><span class="sxs-lookup"><span data-stu-id="9bd7e-131">The sensitivity value of the label, where lower is less sensitive.</span></span>                                           |
| <span data-ttu-id="9bd7e-132">tooltip</span><span class="sxs-lookup"><span data-stu-id="9bd7e-132">tooltip</span></span>     | <span data-ttu-id="9bd7e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9bd7e-133">String</span></span>                                       | <span data-ttu-id="9bd7e-134">Инструмент, который должен отображаться для метки в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="9bd7e-134">The tooltip that should be displayed for the label in a user interface.</span></span>                                      |
| <span data-ttu-id="9bd7e-135">родитель</span><span class="sxs-lookup"><span data-stu-id="9bd7e-135">parent</span></span>      | <span data-ttu-id="9bd7e-136">parentLabelDetails</span><span class="sxs-lookup"><span data-stu-id="9bd7e-136">parentLabelDetails</span></span> | <span data-ttu-id="9bd7e-137">Родительская метка, связанная с детской меткой.</span><span class="sxs-lookup"><span data-stu-id="9bd7e-137">The parent label associated with a child label.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="9bd7e-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9bd7e-138">JSON representation</span></span>

<span data-ttu-id="9bd7e-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9bd7e-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.labelDetails",
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
  "description": "labelDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

