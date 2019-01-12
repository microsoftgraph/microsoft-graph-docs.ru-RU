---
title: Тип ресурса visualInfo
description: Сложный тип для представления свойство **visualElements** в объекте активности.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 416109bb1bb6625330ddfbbb32b8fb688b223134
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962648"
---
# <a name="visualinfo-resource-type"></a><span data-ttu-id="27287-103">Тип ресурса visualInfo</span><span class="sxs-lookup"><span data-stu-id="27287-103">visualInfo resource type</span></span>

<span data-ttu-id="27287-104">Сложный тип для представления свойство **visualElements** в объекте [активности](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="27287-104">A complex type for representing the **visualElements** property in the [activity](../resources/projectrome-activity.md) object.</span></span>

<span data-ttu-id="27287-105">Каждое действие пользователя отображаются на шкале как адаптивный карточки.</span><span class="sxs-lookup"><span data-stu-id="27287-105">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="27287-106">Разработчики приложений, рекомендуется для предоставления настраиваемых карточку, которая записывает только операции, которая выполнялась в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="27287-106">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="27287-107">Это можно сделать с указанием настраиваемых карточки JSON в свойстве контента.</span><span class="sxs-lookup"><span data-stu-id="27287-107">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="27287-108">В дополнение к visual метаданных с адаптивный карточки приложение может указать контента метаданных — данные, которые являются используются для формирования вывод на действие пользователя, чтобы предлагать новые действия для оказания будущих повторно.</span><span class="sxs-lookup"><span data-stu-id="27287-108">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="27287-109">Это можно сделать с помощью свойства contentInfo действия для предоставления объект JSON, который использует свойства schema.org для описания содержимого.</span><span class="sxs-lookup"><span data-stu-id="27287-109">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="27287-110">Если этот параметр не указан настраиваемых карточки простой карточки будут создаваться с использованием отображаемый текст и описание свойств.</span><span class="sxs-lookup"><span data-stu-id="27287-110">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="27287-111">Настраиваемые карточки, рекомендуется использовать для демонстрации наиболее содержимого из в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="27287-111">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="27287-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="27287-112">Properties</span></span>

|<span data-ttu-id="27287-113">Имя</span><span class="sxs-lookup"><span data-stu-id="27287-113">Name</span></span> | <span data-ttu-id="27287-114">Тип</span><span class="sxs-lookup"><span data-stu-id="27287-114">Type</span></span> | <span data-ttu-id="27287-115">Описание</span><span class="sxs-lookup"><span data-stu-id="27287-115">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="27287-116">отображаемый текст</span><span class="sxs-lookup"><span data-stu-id="27287-116">displayText</span></span> | <span data-ttu-id="27287-117">Строка</span><span class="sxs-lookup"><span data-stu-id="27287-117">String</span></span> | <span data-ttu-id="27287-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27287-118">Required.</span></span> <span data-ttu-id="27287-119">Короткая текстовое описание уникальное действие пользователя (например, имя документа в тех случаях, где действие относится к создания документов)</span><span class="sxs-lookup"><span data-stu-id="27287-119">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="27287-120">описание</span><span class="sxs-lookup"><span data-stu-id="27287-120">description</span></span> | <span data-ttu-id="27287-121">String</span><span class="sxs-lookup"><span data-stu-id="27287-121">String</span></span> | <span data-ttu-id="27287-122">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="27287-122">Optional.</span></span> <span data-ttu-id="27287-123">Больше текстовое описание уникальный активности пользователя (пример: документа имя, первое предложение и/или метаданные)</span><span class="sxs-lookup"><span data-stu-id="27287-123">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="27287-124">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="27287-124">backgroundColor</span></span> | <span data-ttu-id="27287-125">String</span><span class="sxs-lookup"><span data-stu-id="27287-125">String</span></span> | <span data-ttu-id="27287-126">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="27287-126">Optional.</span></span> <span data-ttu-id="27287-127">Цвет фона, используемого для отображения активности в пользовательском Интерфейсе - торговая марка цвет для исходного приложения действия.</span><span class="sxs-lookup"><span data-stu-id="27287-127">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="27287-128">Должен быть допустимый шестнадцатеричный цвет</span><span class="sxs-lookup"><span data-stu-id="27287-128">Must be a valid hex color</span></span>|
|<span data-ttu-id="27287-129">content</span><span class="sxs-lookup"><span data-stu-id="27287-129">content</span></span> | <span data-ttu-id="27287-130">Объектный JSON</span><span class="sxs-lookup"><span data-stu-id="27287-130">Untyped JSON object</span></span> | <span data-ttu-id="27287-131">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="27287-131">Optional.</span></span> <span data-ttu-id="27287-132">Настраиваемые части данных — объект JSON, используется для предоставления пользовательского контента для отображения активности в пользовательском Интерфейсе командной консоли Windows</span><span class="sxs-lookup"><span data-stu-id="27287-132">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="27287-133">атрибуты</span><span class="sxs-lookup"><span data-stu-id="27287-133">attribution</span></span> | [<span data-ttu-id="27287-134">imageInfo</span><span class="sxs-lookup"><span data-stu-id="27287-134">imageInfo</span></span>](../resources/projectrome-imageinfo.md) | <span data-ttu-id="27287-135">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="27287-135">Optional.</span></span> <span data-ttu-id="27287-136">Объект JSON, используемый для представления значок, представляющий приложение, используемый для создания операции</span><span class="sxs-lookup"><span data-stu-id="27287-136">JSON object used to represent an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27287-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27287-137">JSON Representation</span></span>

<span data-ttu-id="27287-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27287-138">The following is a JSON representation of the resource.</span></span>

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
