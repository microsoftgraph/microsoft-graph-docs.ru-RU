---
title: Тип ресурса mediaStream
description: Тип mediaStream.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4867675da3427beb790beb240cd7bc0b86f04317
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519964"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="9eec1-103">Тип ресурса mediaStream</span><span class="sxs-lookup"><span data-stu-id="9eec1-103">mediaStream resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9eec1-104">Тип mediaStream.</span><span class="sxs-lookup"><span data-stu-id="9eec1-104">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="9eec1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9eec1-105">Properties</span></span>

| <span data-ttu-id="9eec1-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9eec1-106">Property</span></span>    | <span data-ttu-id="9eec1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9eec1-107">Type</span></span>    | <span data-ttu-id="9eec1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9eec1-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="9eec1-109">Direction</span><span class="sxs-lookup"><span data-stu-id="9eec1-109">direction</span></span>   | <span data-ttu-id="9eec1-110">String</span><span class="sxs-lookup"><span data-stu-id="9eec1-110">String</span></span>  | <span data-ttu-id="9eec1-111">Направление.</span><span class="sxs-lookup"><span data-stu-id="9eec1-111">The direction.</span></span> <span data-ttu-id="9eec1-112">Возможные значения: `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span><span class="sxs-lookup"><span data-stu-id="9eec1-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="9eec1-113">label</span><span class="sxs-lookup"><span data-stu-id="9eec1-113">label</span></span>       | <span data-ttu-id="9eec1-114">String</span><span class="sxs-lookup"><span data-stu-id="9eec1-114">String</span></span>  | <span data-ttu-id="9eec1-115">Метка потока мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="9eec1-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="9eec1-116">MediaType</span><span class="sxs-lookup"><span data-stu-id="9eec1-116">mediaType</span></span>   | <span data-ttu-id="9eec1-117">String</span><span class="sxs-lookup"><span data-stu-id="9eec1-117">String</span></span>  | <span data-ttu-id="9eec1-118">Тип носителя.</span><span class="sxs-lookup"><span data-stu-id="9eec1-118">The media type.</span></span> <span data-ttu-id="9eec1-119">Возможное значение — `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="9eec1-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="9eec1-120">serverMuted</span><span class="sxs-lookup"><span data-stu-id="9eec1-120">serverMuted</span></span> | <span data-ttu-id="9eec1-121">Логическое</span><span class="sxs-lookup"><span data-stu-id="9eec1-121">Boolean</span></span> | <span data-ttu-id="9eec1-122">Если мультимедиа отключен на сервере.</span><span class="sxs-lookup"><span data-stu-id="9eec1-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="9eec1-123">SourceId</span><span class="sxs-lookup"><span data-stu-id="9eec1-123">sourceId</span></span>    | <span data-ttu-id="9eec1-124">String</span><span class="sxs-lookup"><span data-stu-id="9eec1-124">String</span></span>  | <span data-ttu-id="9eec1-125">Исходный код.</span><span class="sxs-lookup"><span data-stu-id="9eec1-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="9eec1-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9eec1-126">JSON representation</span></span>

<span data-ttu-id="9eec1-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9eec1-127">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="9eec1-128">Пример</span><span class="sxs-lookup"><span data-stu-id="9eec1-128">Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mediastream.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
