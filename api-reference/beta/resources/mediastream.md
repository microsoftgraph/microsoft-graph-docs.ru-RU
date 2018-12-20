---
title: Тип ресурса mediaStream
description: Тип mediaStream.
author: VinodRavichandran
ms.openlocfilehash: f870611700289f0254272b78e18e344d02dd123e
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380298"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="40570-103">Тип ресурса mediaStream</span><span class="sxs-lookup"><span data-stu-id="40570-103">mediaStream resource type</span></span>

> <span data-ttu-id="40570-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="40570-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40570-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40570-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="40570-106">Тип mediaStream.</span><span class="sxs-lookup"><span data-stu-id="40570-106">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="40570-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="40570-107">Properties</span></span>

| <span data-ttu-id="40570-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="40570-108">Property</span></span>    | <span data-ttu-id="40570-109">Тип</span><span class="sxs-lookup"><span data-stu-id="40570-109">Type</span></span>    | <span data-ttu-id="40570-110">Описание</span><span class="sxs-lookup"><span data-stu-id="40570-110">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="40570-111">Направление</span><span class="sxs-lookup"><span data-stu-id="40570-111">direction</span></span>   | <span data-ttu-id="40570-112">String</span><span class="sxs-lookup"><span data-stu-id="40570-112">String</span></span>  | <span data-ttu-id="40570-113">Направление.</span><span class="sxs-lookup"><span data-stu-id="40570-113">The direction.</span></span> <span data-ttu-id="40570-114">Возможные значения: `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span><span class="sxs-lookup"><span data-stu-id="40570-114">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="40570-115">label</span><span class="sxs-lookup"><span data-stu-id="40570-115">label</span></span>       | <span data-ttu-id="40570-116">Строка</span><span class="sxs-lookup"><span data-stu-id="40570-116">String</span></span>  | <span data-ttu-id="40570-117">Метка потока мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="40570-117">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="40570-118">Тип носителя</span><span class="sxs-lookup"><span data-stu-id="40570-118">mediaType</span></span>   | <span data-ttu-id="40570-119">String</span><span class="sxs-lookup"><span data-stu-id="40570-119">String</span></span>  | <span data-ttu-id="40570-120">Тип носителя.</span><span class="sxs-lookup"><span data-stu-id="40570-120">The media type.</span></span> <span data-ttu-id="40570-121">Возможное значение — `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="40570-121">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="40570-122">serverMuted</span><span class="sxs-lookup"><span data-stu-id="40570-122">serverMuted</span></span> | <span data-ttu-id="40570-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="40570-123">Boolean</span></span> | <span data-ttu-id="40570-124">Если мультимедиа отключен на сервере.</span><span class="sxs-lookup"><span data-stu-id="40570-124">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="40570-125">sourceId</span><span class="sxs-lookup"><span data-stu-id="40570-125">sourceId</span></span>    | <span data-ttu-id="40570-126">String</span><span class="sxs-lookup"><span data-stu-id="40570-126">String</span></span>  | <span data-ttu-id="40570-127">Исходный код.</span><span class="sxs-lookup"><span data-stu-id="40570-127">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="40570-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40570-128">JSON representation</span></span>

<span data-ttu-id="40570-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40570-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="40570-130">Пример</span><span class="sxs-lookup"><span data-stu-id="40570-130">Example</span></span>

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
