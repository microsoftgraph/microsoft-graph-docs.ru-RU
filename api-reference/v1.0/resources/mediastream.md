---
title: Тип ресурса Медиастреам
description: Тип Медиастреам.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d1158dfb01b9e92c5dc97f34bef3bb3661da51b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088491"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="d808c-103">Тип ресурса Медиастреам</span><span class="sxs-lookup"><span data-stu-id="d808c-103">mediaStream resource type</span></span>

<span data-ttu-id="d808c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d808c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d808c-105">Содержит сведения о канале мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="d808c-105">This contains information about the media channel.</span></span>

## <a name="properties"></a><span data-ttu-id="d808c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d808c-106">Properties</span></span>

| <span data-ttu-id="d808c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d808c-107">Property</span></span>    | <span data-ttu-id="d808c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d808c-108">Type</span></span>    | <span data-ttu-id="d808c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d808c-109">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="d808c-110">direction</span><span class="sxs-lookup"><span data-stu-id="d808c-110">direction</span></span>   | <span data-ttu-id="d808c-111">String</span><span class="sxs-lookup"><span data-stu-id="d808c-111">String</span></span>  | <span data-ttu-id="d808c-112">Направление.</span><span class="sxs-lookup"><span data-stu-id="d808c-112">The direction.</span></span> <span data-ttu-id="d808c-113">Возможные значения: `inactive` ,, `sendOnly` `receiveOnly` , `sendReceive` .</span><span class="sxs-lookup"><span data-stu-id="d808c-113">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="d808c-114">label</span><span class="sxs-lookup"><span data-stu-id="d808c-114">label</span></span>       | <span data-ttu-id="d808c-115">Строка</span><span class="sxs-lookup"><span data-stu-id="d808c-115">String</span></span>  | <span data-ttu-id="d808c-116">Метка потока мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="d808c-116">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="d808c-117">MediaType</span><span class="sxs-lookup"><span data-stu-id="d808c-117">mediaType</span></span>   | <span data-ttu-id="d808c-118">Строка</span><span class="sxs-lookup"><span data-stu-id="d808c-118">String</span></span>  | <span data-ttu-id="d808c-119">Тип мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="d808c-119">The media type.</span></span> <span data-ttu-id="d808c-120">Возможные значения:,,, `unknown` `audio` `video` `videoBasedScreenSharing` , `data` .</span><span class="sxs-lookup"><span data-stu-id="d808c-120">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="d808c-121">сервермутед</span><span class="sxs-lookup"><span data-stu-id="d808c-121">serverMuted</span></span> | <span data-ttu-id="d808c-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="d808c-122">Boolean</span></span> | <span data-ttu-id="d808c-123">Если сервер отключен на носителе.</span><span class="sxs-lookup"><span data-stu-id="d808c-123">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="d808c-124">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="d808c-124">sourceId</span></span>    | <span data-ttu-id="d808c-125">Строка</span><span class="sxs-lookup"><span data-stu-id="d808c-125">String</span></span>  | <span data-ttu-id="d808c-126">Идентификатор источника.</span><span class="sxs-lookup"><span data-stu-id="d808c-126">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="d808c-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d808c-127">JSON representation</span></span>

<span data-ttu-id="d808c-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d808c-128">The following is a JSON representation of the resource.</span></span>

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

