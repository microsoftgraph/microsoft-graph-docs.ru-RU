---
title: Тип ресурса Медиастреам
description: Тип Медиастреам.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6751d00a89bb4ca024f069a69213ebd2d76b7ef7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447432"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="32c29-103">Тип ресурса Медиастреам</span><span class="sxs-lookup"><span data-stu-id="32c29-103">mediaStream resource type</span></span>

<span data-ttu-id="32c29-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="32c29-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="32c29-105">Содержит сведения о канале мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="32c29-105">This contains information about the media channel.</span></span>

## <a name="properties"></a><span data-ttu-id="32c29-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="32c29-106">Properties</span></span>

| <span data-ttu-id="32c29-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="32c29-107">Property</span></span>    | <span data-ttu-id="32c29-108">Тип</span><span class="sxs-lookup"><span data-stu-id="32c29-108">Type</span></span>    | <span data-ttu-id="32c29-109">Описание</span><span class="sxs-lookup"><span data-stu-id="32c29-109">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="32c29-110">direction</span><span class="sxs-lookup"><span data-stu-id="32c29-110">direction</span></span>   | <span data-ttu-id="32c29-111">String</span><span class="sxs-lookup"><span data-stu-id="32c29-111">String</span></span>  | <span data-ttu-id="32c29-112">Направление.</span><span class="sxs-lookup"><span data-stu-id="32c29-112">The direction.</span></span> <span data-ttu-id="32c29-113">`inactive`Возможные значения: `sendOnly`,, `receiveOnly`,. `sendReceive`</span><span class="sxs-lookup"><span data-stu-id="32c29-113">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="32c29-114">label</span><span class="sxs-lookup"><span data-stu-id="32c29-114">label</span></span>       | <span data-ttu-id="32c29-115">String</span><span class="sxs-lookup"><span data-stu-id="32c29-115">String</span></span>  | <span data-ttu-id="32c29-116">Метка потока мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="32c29-116">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="32c29-117">mediaType</span><span class="sxs-lookup"><span data-stu-id="32c29-117">mediaType</span></span>   | <span data-ttu-id="32c29-118">String</span><span class="sxs-lookup"><span data-stu-id="32c29-118">String</span></span>  | <span data-ttu-id="32c29-119">Тип мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="32c29-119">The media type.</span></span> <span data-ttu-id="32c29-120">Возможные `unknown`значения:, `audio` `video`,, `videoBasedScreenSharing`,. `data`</span><span class="sxs-lookup"><span data-stu-id="32c29-120">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="32c29-121">сервермутед</span><span class="sxs-lookup"><span data-stu-id="32c29-121">serverMuted</span></span> | <span data-ttu-id="32c29-122">Логический</span><span class="sxs-lookup"><span data-stu-id="32c29-122">Boolean</span></span> | <span data-ttu-id="32c29-123">Если сервер отключен на носителе.</span><span class="sxs-lookup"><span data-stu-id="32c29-123">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="32c29-124">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="32c29-124">sourceId</span></span>    | <span data-ttu-id="32c29-125">String</span><span class="sxs-lookup"><span data-stu-id="32c29-125">String</span></span>  | <span data-ttu-id="32c29-126">Идентификатор источника.</span><span class="sxs-lookup"><span data-stu-id="32c29-126">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="32c29-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32c29-127">JSON representation</span></span>

<span data-ttu-id="32c29-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32c29-128">The following is a JSON representation of the resource.</span></span>

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
