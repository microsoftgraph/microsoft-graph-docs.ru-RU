---
title: Тип ресурса visualInfo
description: Сложный тип для представления свойство **visualElements** в объекте активности.
ms.openlocfilehash: ac895e854051cb487fa9afd0ff9ada972b97aa19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078911"
---
# <a name="visualinfo-resource-type"></a><span data-ttu-id="11212-103">Тип ресурса visualInfo</span><span class="sxs-lookup"><span data-stu-id="11212-103">visualInfo resource type</span></span>

> <span data-ttu-id="11212-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="11212-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11212-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11212-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="11212-106">Сложный тип для представления свойство **visualElements** в объекте [активности](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="11212-106">A complex type for representing the **visualElements** property in the [activity](../resources/projectrome-activity.md) object.</span></span>

<span data-ttu-id="11212-107">Каждое действие пользователя отображаются на шкале как адаптивный карточки.</span><span class="sxs-lookup"><span data-stu-id="11212-107">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="11212-108">Разработчики приложений, рекомендуется для предоставления настраиваемых карточку, которая записывает только операции, которая выполнялась в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="11212-108">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="11212-109">Это можно сделать с указанием настраиваемых карточки JSON в свойстве контента.</span><span class="sxs-lookup"><span data-stu-id="11212-109">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="11212-110">В дополнение к visual метаданных с адаптивный карточки приложение может указать контента метаданных — данные, которые являются используются для формирования вывод на действие пользователя, чтобы предлагать новые действия для оказания будущих повторно.</span><span class="sxs-lookup"><span data-stu-id="11212-110">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="11212-111">Это можно сделать с помощью свойства contentInfo действия для предоставления объект JSON, который использует свойства schema.org для описания содержимого.</span><span class="sxs-lookup"><span data-stu-id="11212-111">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="11212-112">Если этот параметр не указан настраиваемых карточки простой карточки будут создаваться с использованием отображаемый текст и описание свойств.</span><span class="sxs-lookup"><span data-stu-id="11212-112">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="11212-113">Настраиваемые карточки, рекомендуется использовать для демонстрации наиболее содержимого из в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="11212-113">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="11212-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="11212-114">Properties</span></span>

|<span data-ttu-id="11212-115">Имя</span><span class="sxs-lookup"><span data-stu-id="11212-115">Name</span></span> | <span data-ttu-id="11212-116">Тип</span><span class="sxs-lookup"><span data-stu-id="11212-116">Type</span></span> | <span data-ttu-id="11212-117">Description</span><span class="sxs-lookup"><span data-stu-id="11212-117">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="11212-118">отображаемый текст</span><span class="sxs-lookup"><span data-stu-id="11212-118">displayText</span></span> | <span data-ttu-id="11212-119">Строка</span><span class="sxs-lookup"><span data-stu-id="11212-119">String</span></span> | <span data-ttu-id="11212-120">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="11212-120">Required.</span></span> <span data-ttu-id="11212-121">Короткая текстовое описание уникальное действие пользователя (например, имя документа в тех случаях, где действие относится к создания документов)</span><span class="sxs-lookup"><span data-stu-id="11212-121">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="11212-122">описание</span><span class="sxs-lookup"><span data-stu-id="11212-122">description</span></span> | <span data-ttu-id="11212-123">String</span><span class="sxs-lookup"><span data-stu-id="11212-123">String</span></span> | <span data-ttu-id="11212-124">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="11212-124">Optional.</span></span> <span data-ttu-id="11212-125">Больше текстовое описание уникальный активности пользователя (пример: документа имя, первое предложение и/или метаданные)</span><span class="sxs-lookup"><span data-stu-id="11212-125">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="11212-126">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="11212-126">backgroundColor</span></span> | <span data-ttu-id="11212-127">String</span><span class="sxs-lookup"><span data-stu-id="11212-127">String</span></span> | <span data-ttu-id="11212-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="11212-128">Optional.</span></span> <span data-ttu-id="11212-129">Цвет фона, используемого для отображения активности в пользовательском Интерфейсе - торговая марка цвет для исходного приложения действия.</span><span class="sxs-lookup"><span data-stu-id="11212-129">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="11212-130">Должен быть допустимый шестнадцатеричный цвет</span><span class="sxs-lookup"><span data-stu-id="11212-130">Must be a valid hex color</span></span>|
|<span data-ttu-id="11212-131">content</span><span class="sxs-lookup"><span data-stu-id="11212-131">content</span></span> | <span data-ttu-id="11212-132">Объектный JSON</span><span class="sxs-lookup"><span data-stu-id="11212-132">Untyped JSON object</span></span> | <span data-ttu-id="11212-133">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="11212-133">Optional.</span></span> <span data-ttu-id="11212-134">Настраиваемые части данных — объект JSON, используется для предоставления пользовательского контента для отображения активности в пользовательском Интерфейсе командной консоли Windows</span><span class="sxs-lookup"><span data-stu-id="11212-134">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="11212-135">атрибуты</span><span class="sxs-lookup"><span data-stu-id="11212-135">attribution</span></span> | [<span data-ttu-id="11212-136">imageInfo</span><span class="sxs-lookup"><span data-stu-id="11212-136">imageInfo</span></span>](../resources/projectrome-imageinfo.md) | <span data-ttu-id="11212-137">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="11212-137">Optional.</span></span> <span data-ttu-id="11212-138">Объект JSON, используемый для представления значок, представляющий приложение, используемый для создания операции</span><span class="sxs-lookup"><span data-stu-id="11212-138">JSON object used to represent an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11212-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11212-139">JSON Representation</span></span>

<span data-ttu-id="11212-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11212-140">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
