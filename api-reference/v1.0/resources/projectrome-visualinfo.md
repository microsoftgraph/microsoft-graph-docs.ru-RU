---
title: Тип ресурса Висуалинфо
description: Сложный тип для представления свойства **висуалелементс** в объекте Activity.
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: resourcePageType
ms.openlocfilehash: e97e7d295d9a228d44adf355b510adb90a0b3f96
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447047"
---
# <a name="visualinfo-resource-type"></a><span data-ttu-id="514f1-103">Тип ресурса Висуалинфо</span><span class="sxs-lookup"><span data-stu-id="514f1-103">visualInfo resource type</span></span>

<span data-ttu-id="514f1-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="514f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="514f1-105">Сложный тип для представления свойства **висуалелементс** в объекте [Activity](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="514f1-105">A complex type for representing the **visualElements** property in the [activity](../resources/projectrome-activity.md) object.</span></span>

<span data-ttu-id="514f1-106">Каждое действие пользователя будет отображаться на временной шкале в качестве адаптивной карты.</span><span class="sxs-lookup"><span data-stu-id="514f1-106">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="514f1-107">Разработчикам приложений рекомендуется предоставить настраиваемую карту, которая захватывает суть действия, которое было принято в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="514f1-107">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="514f1-108">Это возможно благодаря созданию настраиваемой карты JSON в свойстве Content.</span><span class="sxs-lookup"><span data-stu-id="514f1-108">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="514f1-109">В дополнение к визуальным метаданным с помощью адаптивной карточки приложение может указывать метаданные содержимого — данные, которые используются для построения выработок в действиях пользователя, чтобы обеспечить новые действия для будущего повторного задействования.</span><span class="sxs-lookup"><span data-stu-id="514f1-109">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="514f1-110">Это возможно благодаря использованию свойства Контентинфо действия для предоставления объекта JSON, который использует свойства schema.org для описания содержимого.</span><span class="sxs-lookup"><span data-stu-id="514f1-110">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="514f1-111">Если настраиваемая карточка не указана, будет создана простая карточка с использованием свойств Дисплайтекст и Description.</span><span class="sxs-lookup"><span data-stu-id="514f1-111">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="514f1-112">Для демонстрации лучшего контента в приложении рекомендуется использовать настраиваемые карточки.</span><span class="sxs-lookup"><span data-stu-id="514f1-112">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="514f1-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="514f1-113">Properties</span></span>

|<span data-ttu-id="514f1-114">Имя</span><span class="sxs-lookup"><span data-stu-id="514f1-114">Name</span></span> | <span data-ttu-id="514f1-115">Тип</span><span class="sxs-lookup"><span data-stu-id="514f1-115">Type</span></span> | <span data-ttu-id="514f1-116">Описание</span><span class="sxs-lookup"><span data-stu-id="514f1-116">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="514f1-117">дисплайтекст</span><span class="sxs-lookup"><span data-stu-id="514f1-117">displayText</span></span> | <span data-ttu-id="514f1-118">String</span><span class="sxs-lookup"><span data-stu-id="514f1-118">String</span></span> | <span data-ttu-id="514f1-119">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="514f1-119">Required.</span></span> <span data-ttu-id="514f1-120">Краткое текстовое описание уникального действия пользователя (например, имя документа в тех случаях, когда действие относится к созданию документа)</span><span class="sxs-lookup"><span data-stu-id="514f1-120">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="514f1-121">description</span><span class="sxs-lookup"><span data-stu-id="514f1-121">description</span></span> | <span data-ttu-id="514f1-122">String</span><span class="sxs-lookup"><span data-stu-id="514f1-122">String</span></span> | <span data-ttu-id="514f1-123">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="514f1-123">Optional.</span></span> <span data-ttu-id="514f1-124">Длинное текстовое описание уникального действия пользователя (пример: имя документа, первое предложение и/или метаданные)</span><span class="sxs-lookup"><span data-stu-id="514f1-124">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="514f1-125">баккграундколор</span><span class="sxs-lookup"><span data-stu-id="514f1-125">backgroundColor</span></span> | <span data-ttu-id="514f1-126">String</span><span class="sxs-lookup"><span data-stu-id="514f1-126">String</span></span> | <span data-ttu-id="514f1-127">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="514f1-127">Optional.</span></span> <span data-ttu-id="514f1-128">Цвет фона, используемый для отображения активности в цвете пользовательского интерфейса для источника действия приложения.</span><span class="sxs-lookup"><span data-stu-id="514f1-128">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="514f1-129">Должно быть допустимым шестнадцатеричным цветом</span><span class="sxs-lookup"><span data-stu-id="514f1-129">Must be a valid hex color</span></span>|
|<span data-ttu-id="514f1-130">содержимое</span><span class="sxs-lookup"><span data-stu-id="514f1-130">content</span></span> | <span data-ttu-id="514f1-131">Нетипизированный объект JSON</span><span class="sxs-lookup"><span data-stu-id="514f1-131">Untyped JSON object</span></span> | <span data-ttu-id="514f1-132">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="514f1-132">Optional.</span></span> <span data-ttu-id="514f1-133">Настраиваемый фрагмент объекта data: JSON, используемый для предоставления настраиваемого содержимого для отображения действий в пользовательском интерфейсе оболочки Windows</span><span class="sxs-lookup"><span data-stu-id="514f1-133">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="514f1-134">Attribution</span><span class="sxs-lookup"><span data-stu-id="514f1-134">attribution</span></span> | [<span data-ttu-id="514f1-135">имажеинфо</span><span class="sxs-lookup"><span data-stu-id="514f1-135">imageInfo</span></span>](../resources/projectrome-imageinfo.md) | <span data-ttu-id="514f1-136">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="514f1-136">Optional.</span></span> <span data-ttu-id="514f1-137">Объект JSON, используемый для представления значка, представляющего приложение, используемое для создания действия</span><span class="sxs-lookup"><span data-stu-id="514f1-137">JSON object used to represent an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="514f1-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="514f1-138">JSON Representation</span></span>

<span data-ttu-id="514f1-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="514f1-139">The following is a JSON representation of the resource.</span></span>

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
    "@odata.type": "microsoft.graph.visualInfo",
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
        "@odata.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
