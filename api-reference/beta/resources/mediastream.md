---
title: Тип ресурса mediaStream
description: Тип mediaStream.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 7e56448c2c6d284e7a5904f1b0af414166782907
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889616"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="6fcc3-103">Тип ресурса mediaStream</span><span class="sxs-lookup"><span data-stu-id="6fcc3-103">mediaStream resource type</span></span>

> <span data-ttu-id="6fcc3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6fcc3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6fcc3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fcc3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6fcc3-106">Тип mediaStream.</span><span class="sxs-lookup"><span data-stu-id="6fcc3-106">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="6fcc3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6fcc3-107">Properties</span></span>

| <span data-ttu-id="6fcc3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fcc3-108">Property</span></span>    | <span data-ttu-id="6fcc3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6fcc3-109">Type</span></span>    | <span data-ttu-id="6fcc3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6fcc3-110">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="6fcc3-111">Направление</span><span class="sxs-lookup"><span data-stu-id="6fcc3-111">direction</span></span>   | <span data-ttu-id="6fcc3-112">Строка</span><span class="sxs-lookup"><span data-stu-id="6fcc3-112">String</span></span>  | <span data-ttu-id="6fcc3-113">Направление.</span><span class="sxs-lookup"><span data-stu-id="6fcc3-113">The direction.</span></span> <span data-ttu-id="6fcc3-114">Возможные значения: `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span><span class="sxs-lookup"><span data-stu-id="6fcc3-114">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="6fcc3-115">label</span><span class="sxs-lookup"><span data-stu-id="6fcc3-115">label</span></span>       | <span data-ttu-id="6fcc3-116">Строка</span><span class="sxs-lookup"><span data-stu-id="6fcc3-116">String</span></span>  | <span data-ttu-id="6fcc3-117">Метка потока мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="6fcc3-117">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="6fcc3-118">Тип носителя</span><span class="sxs-lookup"><span data-stu-id="6fcc3-118">mediaType</span></span>   | <span data-ttu-id="6fcc3-119">Строка</span><span class="sxs-lookup"><span data-stu-id="6fcc3-119">String</span></span>  | <span data-ttu-id="6fcc3-120">Тип носителя.</span><span class="sxs-lookup"><span data-stu-id="6fcc3-120">The media type.</span></span> <span data-ttu-id="6fcc3-121">Возможное значение — `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="6fcc3-121">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="6fcc3-122">serverMuted</span><span class="sxs-lookup"><span data-stu-id="6fcc3-122">serverMuted</span></span> | <span data-ttu-id="6fcc3-123">Логический</span><span class="sxs-lookup"><span data-stu-id="6fcc3-123">Boolean</span></span> | <span data-ttu-id="6fcc3-124">Если мультимедиа отключен на сервере.</span><span class="sxs-lookup"><span data-stu-id="6fcc3-124">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="6fcc3-125">sourceId</span><span class="sxs-lookup"><span data-stu-id="6fcc3-125">sourceId</span></span>    | <span data-ttu-id="6fcc3-126">Строка</span><span class="sxs-lookup"><span data-stu-id="6fcc3-126">String</span></span>  | <span data-ttu-id="6fcc3-127">Исходный код.</span><span class="sxs-lookup"><span data-stu-id="6fcc3-127">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="6fcc3-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6fcc3-128">JSON representation</span></span>

<span data-ttu-id="6fcc3-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fcc3-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted"
  ],
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "inactive | sendOnly | receiveOnly | sendReceive",
  "label": "String",
  "mediaType": "unknown | audio | video | videoBasedScreenSharing | data",
  "serverMuted": true,
  "sourceId": "String"
}
```

## <a name="example"></a><span data-ttu-id="6fcc3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6fcc3-130">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "sendReceive",
  "label": "main-audio",
  "mediaType": "audio",
  "serverMuted": false,
  "sourceId": "1024"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
