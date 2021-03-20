---
title: тип ресурса labelDetails
description: Представляет сведения метки защиты информации.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 214589dfcb26497b5271008f8a358d06a4fb700f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950312"
---
# <a name="labeldetails-resource-type"></a><span data-ttu-id="977ec-103">тип ресурса labelDetails</span><span class="sxs-lookup"><span data-stu-id="977ec-103">labelDetails resource type</span></span>

<span data-ttu-id="977ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="977ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="977ec-105">Представляет сведения метки защиты информации.</span><span class="sxs-lookup"><span data-stu-id="977ec-105">Represents the label details of an information protection label.</span></span> <span data-ttu-id="977ec-106">**LabelDetails предоставляет** сведения о единой мете защиты информации.</span><span class="sxs-lookup"><span data-stu-id="977ec-106">**labelDetails** provides information about a single information protection label.</span></span> <span data-ttu-id="977ec-107">Можно вернуть по [оценкеRemoval,](../api/informationprotectionlabel-evaluateremoval.md) [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)и [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span><span class="sxs-lookup"><span data-stu-id="977ec-107">Can be returned by [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="977ec-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="977ec-108">Properties</span></span>

| <span data-ttu-id="977ec-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="977ec-109">Property</span></span>    | <span data-ttu-id="977ec-110">Тип</span><span class="sxs-lookup"><span data-stu-id="977ec-110">Type</span></span>    | <span data-ttu-id="977ec-111">Описание</span><span class="sxs-lookup"><span data-stu-id="977ec-111">Description</span></span>                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="977ec-112">color</span><span class="sxs-lookup"><span data-stu-id="977ec-112">color</span></span>       | <span data-ttu-id="977ec-113">String</span><span class="sxs-lookup"><span data-stu-id="977ec-113">String</span></span>  | <span data-ttu-id="977ec-114">Цвет, который должен отображаться в пользовательском интерфейсе для метки, если настроен.</span><span class="sxs-lookup"><span data-stu-id="977ec-114">The color that the user interface should display for the label, if configured.</span></span>                               |
| <span data-ttu-id="977ec-115">description</span><span class="sxs-lookup"><span data-stu-id="977ec-115">description</span></span> | <span data-ttu-id="977ec-116">Строка</span><span class="sxs-lookup"><span data-stu-id="977ec-116">String</span></span>  | <span data-ttu-id="977ec-117">Описание метки, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="977ec-117">The admin-defined description for the label.</span></span>                                                                 |
| <span data-ttu-id="977ec-118">id</span><span class="sxs-lookup"><span data-stu-id="977ec-118">id</span></span>          | <span data-ttu-id="977ec-119">Строка</span><span class="sxs-lookup"><span data-stu-id="977ec-119">String</span></span>  | <span data-ttu-id="977ec-120">Идентификатор метки — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="977ec-120">The label ID is a globally unique identifier (GUID).</span></span>                                                          |
| <span data-ttu-id="977ec-121">isActive</span><span class="sxs-lookup"><span data-stu-id="977ec-121">isActive</span></span>    | <span data-ttu-id="977ec-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="977ec-122">Boolean</span></span> | <span data-ttu-id="977ec-123">Указывает, активна метка или нет.</span><span class="sxs-lookup"><span data-stu-id="977ec-123">Indicates whether the label is active or not.</span></span> <span data-ttu-id="977ec-124">Активные метки должны быть скрыты или отключены в пользовательских интерфейсах.</span><span class="sxs-lookup"><span data-stu-id="977ec-124">Active labels should be hidden or disabled in user interfaces.</span></span> |
| <span data-ttu-id="977ec-125">name</span><span class="sxs-lookup"><span data-stu-id="977ec-125">name</span></span>        | <span data-ttu-id="977ec-126">String</span><span class="sxs-lookup"><span data-stu-id="977ec-126">String</span></span>  | <span data-ttu-id="977ec-127">Простое имя метки.</span><span class="sxs-lookup"><span data-stu-id="977ec-127">The plaintext name of the label.</span></span>                                                                             |
| <span data-ttu-id="977ec-128">sensitivity</span><span class="sxs-lookup"><span data-stu-id="977ec-128">sensitivity</span></span> | <span data-ttu-id="977ec-129">Int32</span><span class="sxs-lookup"><span data-stu-id="977ec-129">Int32</span></span>   | <span data-ttu-id="977ec-130">Значение чувствительности метки, где более низкий уровень менее чувствителен.</span><span class="sxs-lookup"><span data-stu-id="977ec-130">The sensitivity value of the label, where lower is less sensitive.</span></span>                                           |
| <span data-ttu-id="977ec-131">tooltip</span><span class="sxs-lookup"><span data-stu-id="977ec-131">tooltip</span></span>     | <span data-ttu-id="977ec-132">Строка</span><span class="sxs-lookup"><span data-stu-id="977ec-132">String</span></span>  | <span data-ttu-id="977ec-133">Инструмент, который должен отображаться для метки в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="977ec-133">The tooltip that should be displayed for the label in a user interface.</span></span>                                      |

## <a name="json-representation"></a><span data-ttu-id="977ec-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="977ec-134">JSON representation</span></span>

<span data-ttu-id="977ec-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="977ec-135">The following is a JSON representation of the resource.</span></span>

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

