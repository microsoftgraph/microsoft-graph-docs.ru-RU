---
title: Тип ресурса Висуалинфо
description: Сложный тип для представления свойства **висуалелементс** в объекте Activity.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: edf02c7318f45f711da3a27b03747aac94fd9706
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344069"
---
# <a name="visualinfo-resource-type"></a><span data-ttu-id="baca9-103">Тип ресурса Висуалинфо</span><span class="sxs-lookup"><span data-stu-id="baca9-103">visualInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baca9-104">Сложный тип для представления свойства **висуалелементс** в объекте [Activity](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="baca9-104">A complex type for representing the **visualElements** property in the [activity](../resources/projectrome-activity.md) object.</span></span>

<span data-ttu-id="baca9-105">Каждое действие пользователя будет отображаться на временной шкале в качестве адаптивной карты.</span><span class="sxs-lookup"><span data-stu-id="baca9-105">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="baca9-106">Разработчикам приложений рекомендуется предоставить настраиваемую карту, которая захватывает суть действия, которое было принято в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="baca9-106">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="baca9-107">Это возможно благодаря созданию настраиваемой карты JSON в свойстве Content.</span><span class="sxs-lookup"><span data-stu-id="baca9-107">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="baca9-108">В дополнение к визуальным метаданным с помощью адаптивной карточки приложение может указывать метаданные содержимого — данные, которые используются для построения выработок в действиях пользователя, чтобы обеспечить новые действия для будущего повторного задействования.</span><span class="sxs-lookup"><span data-stu-id="baca9-108">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="baca9-109">Это возможно благодаря использованию свойства Контентинфо действия для предоставления объекта JSON, который использует свойства schema.org для описания содержимого.</span><span class="sxs-lookup"><span data-stu-id="baca9-109">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="baca9-110">Если настраиваемая карточка не указана, будет создана простая карточка с использованием свойств Дисплайтекст и Description.</span><span class="sxs-lookup"><span data-stu-id="baca9-110">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="baca9-111">Для демонстрации лучшего контента в приложении рекомендуется использовать настраиваемые карточки.</span><span class="sxs-lookup"><span data-stu-id="baca9-111">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="baca9-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="baca9-112">Properties</span></span>

|<span data-ttu-id="baca9-113">Имя</span><span class="sxs-lookup"><span data-stu-id="baca9-113">Name</span></span> | <span data-ttu-id="baca9-114">Тип</span><span class="sxs-lookup"><span data-stu-id="baca9-114">Type</span></span> | <span data-ttu-id="baca9-115">Описание</span><span class="sxs-lookup"><span data-stu-id="baca9-115">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="baca9-116">Дисплайтекст</span><span class="sxs-lookup"><span data-stu-id="baca9-116">displayText</span></span> | <span data-ttu-id="baca9-117">String</span><span class="sxs-lookup"><span data-stu-id="baca9-117">String</span></span> | <span data-ttu-id="baca9-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="baca9-118">Required.</span></span> <span data-ttu-id="baca9-119">Краткое текстовое описание уникального действия пользователя (например, имя документа в тех случаях, когда действие относится к созданию документа)</span><span class="sxs-lookup"><span data-stu-id="baca9-119">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="baca9-120">description</span><span class="sxs-lookup"><span data-stu-id="baca9-120">description</span></span> | <span data-ttu-id="baca9-121">String</span><span class="sxs-lookup"><span data-stu-id="baca9-121">String</span></span> | <span data-ttu-id="baca9-122">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="baca9-122">Optional.</span></span> <span data-ttu-id="baca9-123">Длинное текстовое описание уникального действия пользователя (пример: имя документа, первое предложение и/или метаданные)</span><span class="sxs-lookup"><span data-stu-id="baca9-123">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="baca9-124">Баккграундколор</span><span class="sxs-lookup"><span data-stu-id="baca9-124">backgroundColor</span></span> | <span data-ttu-id="baca9-125">String</span><span class="sxs-lookup"><span data-stu-id="baca9-125">String</span></span> | <span data-ttu-id="baca9-126">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="baca9-126">Optional.</span></span> <span data-ttu-id="baca9-127">Цвет фона, используемый для отображения активности в цвете ПОЛЬЗОВАТЕЛЬСКОГО интерфейса для источника действия приложения.</span><span class="sxs-lookup"><span data-stu-id="baca9-127">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="baca9-128">Должно быть допустимым шестнадцатеричным цветом</span><span class="sxs-lookup"><span data-stu-id="baca9-128">Must be a valid hex color</span></span>|
|<span data-ttu-id="baca9-129">содержимое</span><span class="sxs-lookup"><span data-stu-id="baca9-129">content</span></span> | <span data-ttu-id="baca9-130">Нетипизированный объект JSON</span><span class="sxs-lookup"><span data-stu-id="baca9-130">Untyped JSON object</span></span> | <span data-ttu-id="baca9-131">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="baca9-131">Optional.</span></span> <span data-ttu-id="baca9-132">Настраиваемый фрагмент объекта data: JSON, используемый для предоставления настраиваемого содержимого для отображения действий в ПОЛЬЗОВАТЕЛЬСКОМ ИНТЕРФЕЙСе оболочки Windows</span><span class="sxs-lookup"><span data-stu-id="baca9-132">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="baca9-133">Attribution</span><span class="sxs-lookup"><span data-stu-id="baca9-133">attribution</span></span> | [<span data-ttu-id="baca9-134">Имажеинфо</span><span class="sxs-lookup"><span data-stu-id="baca9-134">imageInfo</span></span>](../resources/projectrome-imageinfo.md) | <span data-ttu-id="baca9-135">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="baca9-135">Optional.</span></span> <span data-ttu-id="baca9-136">Объект JSON, используемый для представления значка, представляющего приложение, используемое для создания действия</span><span class="sxs-lookup"><span data-stu-id="baca9-136">JSON object used to represent an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="baca9-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="baca9-137">JSON Representation</span></span>

<span data-ttu-id="baca9-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="baca9-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@data.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@data.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
