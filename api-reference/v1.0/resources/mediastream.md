---
title: Тип ресурса Медиастреам
description: Тип Медиастреам.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ed564f4789a88092e34b8f8b4b0db8db63b48f2f
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913655"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="cb6c9-103">Тип ресурса Медиастреам</span><span class="sxs-lookup"><span data-stu-id="cb6c9-103">mediaStream resource type</span></span>

<span data-ttu-id="cb6c9-104">Содержит сведения о канале мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="cb6c9-104">This contains information about the media channel.</span></span>

## <a name="properties"></a><span data-ttu-id="cb6c9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb6c9-105">Properties</span></span>

| <span data-ttu-id="cb6c9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb6c9-106">Property</span></span>    | <span data-ttu-id="cb6c9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="cb6c9-107">Type</span></span>    | <span data-ttu-id="cb6c9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="cb6c9-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="cb6c9-109">direction</span><span class="sxs-lookup"><span data-stu-id="cb6c9-109">direction</span></span>   | <span data-ttu-id="cb6c9-110">String</span><span class="sxs-lookup"><span data-stu-id="cb6c9-110">String</span></span>  | <span data-ttu-id="cb6c9-111">Направление.</span><span class="sxs-lookup"><span data-stu-id="cb6c9-111">The direction.</span></span> <span data-ttu-id="cb6c9-112">`inactive`Возможные значения: `sendOnly`,, `receiveOnly`,. `sendReceive`</span><span class="sxs-lookup"><span data-stu-id="cb6c9-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="cb6c9-113">label</span><span class="sxs-lookup"><span data-stu-id="cb6c9-113">label</span></span>       | <span data-ttu-id="cb6c9-114">String</span><span class="sxs-lookup"><span data-stu-id="cb6c9-114">String</span></span>  | <span data-ttu-id="cb6c9-115">Метка потока мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="cb6c9-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="cb6c9-116">mediaType</span><span class="sxs-lookup"><span data-stu-id="cb6c9-116">mediaType</span></span>   | <span data-ttu-id="cb6c9-117">String</span><span class="sxs-lookup"><span data-stu-id="cb6c9-117">String</span></span>  | <span data-ttu-id="cb6c9-118">Тип мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="cb6c9-118">The media type.</span></span> <span data-ttu-id="cb6c9-119">Возможные `unknown`значения:, `audio` `video`,, `videoBasedScreenSharing`,. `data`</span><span class="sxs-lookup"><span data-stu-id="cb6c9-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="cb6c9-120">сервермутед</span><span class="sxs-lookup"><span data-stu-id="cb6c9-120">serverMuted</span></span> | <span data-ttu-id="cb6c9-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb6c9-121">Boolean</span></span> | <span data-ttu-id="cb6c9-122">Если сервер отключен на носителе.</span><span class="sxs-lookup"><span data-stu-id="cb6c9-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="cb6c9-123">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="cb6c9-123">sourceId</span></span>    | <span data-ttu-id="cb6c9-124">String</span><span class="sxs-lookup"><span data-stu-id="cb6c9-124">String</span></span>  | <span data-ttu-id="cb6c9-125">Идентификатор источника.</span><span class="sxs-lookup"><span data-stu-id="cb6c9-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="cb6c9-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb6c9-126">JSON representation</span></span>

<span data-ttu-id="cb6c9-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb6c9-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted",
    "label"
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
