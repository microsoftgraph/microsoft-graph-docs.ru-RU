---
title: Тип ресурса imageInfo
description: Сложный тип для представления свойство **атрибуты** в части visualInfo объекта активности.
localization_priority: Normal
ms.openlocfilehash: 9df93e24c2019f246fc9da269b40ab690ae81aa4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828569"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="a0e68-103">Тип ресурса imageInfo</span><span class="sxs-lookup"><span data-stu-id="a0e68-103">imageInfo resource type</span></span>

> <span data-ttu-id="a0e68-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a0e68-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0e68-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0e68-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0e68-106">Сложный тип для представления свойство **атрибуты** в части [visualInfo](../resources/projectrome-visualinfo.md) объекта [активности](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="a0e68-106">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="a0e68-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0e68-107">Properties</span></span>

|<span data-ttu-id="a0e68-108">Имя</span><span class="sxs-lookup"><span data-stu-id="a0e68-108">Name</span></span> | <span data-ttu-id="a0e68-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a0e68-109">Type</span></span> | <span data-ttu-id="a0e68-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a0e68-110">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="a0e68-111">iconUrl</span><span class="sxs-lookup"><span data-stu-id="a0e68-111">iconUrl</span></span> | <span data-ttu-id="a0e68-112">Строка</span><span class="sxs-lookup"><span data-stu-id="a0e68-112">String</span></span> | <span data-ttu-id="a0e68-113">Необязательный; URI, указывающий на значок, представляющий приложение, используемый для создания операции</span><span class="sxs-lookup"><span data-stu-id="a0e68-113">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="a0e68-114">alternateText</span><span class="sxs-lookup"><span data-stu-id="a0e68-114">alternateText</span></span> | <span data-ttu-id="a0e68-115">Строка</span><span class="sxs-lookup"><span data-stu-id="a0e68-115">String</span></span> | <span data-ttu-id="a0e68-116">Необязательный; Замещающий текст доступного содержимого для образа</span><span class="sxs-lookup"><span data-stu-id="a0e68-116">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="a0e68-117">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="a0e68-117">addImageQuery</span></span> | <span data-ttu-id="a0e68-118">Логический</span><span class="sxs-lookup"><span data-stu-id="a0e68-118">Boolean</span></span> | <span data-ttu-id="a0e68-119">Необязательный; параметр служит для указания сервера может отобразить изображение динамически в ответ на параметризации.</span><span class="sxs-lookup"><span data-stu-id="a0e68-119">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="a0e68-120">Для примера — изображение высокой контрастности</span><span class="sxs-lookup"><span data-stu-id="a0e68-120">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0e68-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0e68-121">JSON Representation</span></span>

<span data-ttu-id="a0e68-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0e68-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
