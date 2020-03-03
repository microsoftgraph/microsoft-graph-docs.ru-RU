---
title: Тип ресурса мультимедиа
description: Тип мультимедиа
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1b996c34c3d12984cc512dbcc4d1113d54bd5f69
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394849"
---
# <a name="media-resource-type"></a><span data-ttu-id="0be37-103">Тип ресурса мультимедиа</span><span class="sxs-lookup"><span data-stu-id="0be37-103">media resource type</span></span>

<span data-ttu-id="0be37-104">Пространство имен: Microsoft. Graph. Каллрекордс</span><span class="sxs-lookup"><span data-stu-id="0be37-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0be37-105">Представляет мультимедиа (звук, видео, Видеообмен на экране и т. д.), используемые при вызове.</span><span class="sxs-lookup"><span data-stu-id="0be37-105">Represents the media (audio, video, video-based screen-sharing, etc.) used in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="0be37-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0be37-106">Properties</span></span>

| <span data-ttu-id="0be37-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0be37-107">Property</span></span>     | <span data-ttu-id="0be37-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0be37-108">Type</span></span>        | <span data-ttu-id="0be37-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0be37-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0be37-110">label</span><span class="sxs-lookup"><span data-stu-id="0be37-110">label</span></span>|<span data-ttu-id="0be37-111">String</span><span class="sxs-lookup"><span data-stu-id="0be37-111">String</span></span>|<span data-ttu-id="0be37-112">Способ идентификации мультимедиа во время этапа согласования мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="0be37-112">How the media was identified during media negotiation stage.</span></span>|
|<span data-ttu-id="0be37-113">каллердевице</span><span class="sxs-lookup"><span data-stu-id="0be37-113">callerDevice</span></span>|[<span data-ttu-id="0be37-114">Microsoft. Graph. Каллрекордс. Девицеинфо</span><span class="sxs-lookup"><span data-stu-id="0be37-114">microsoft.graph.callRecords.deviceInfo</span></span>](callrecords-deviceinfo.md)|<span data-ttu-id="0be37-115">Сведения об устройстве, связанные с конечной точкой абонента этого носителя.</span><span class="sxs-lookup"><span data-stu-id="0be37-115">Device information associated with the caller endpoint of this media.</span></span>|
|<span data-ttu-id="0be37-116">каллернетворк</span><span class="sxs-lookup"><span data-stu-id="0be37-116">callerNetwork</span></span>|[<span data-ttu-id="0be37-117">Microsoft. Graph. Каллрекордс. Нетворкинфо</span><span class="sxs-lookup"><span data-stu-id="0be37-117">microsoft.graph.callRecords.networkInfo</span></span>](callrecords-networkinfo.md)|<span data-ttu-id="0be37-118">Сведения о сети, связанные с конечной точкой абонента этого носителя.</span><span class="sxs-lookup"><span data-stu-id="0be37-118">Network information associated with the caller endpoint of this media.</span></span>|
|<span data-ttu-id="0be37-119">каллидевице</span><span class="sxs-lookup"><span data-stu-id="0be37-119">calleeDevice</span></span>|[<span data-ttu-id="0be37-120">Microsoft. Graph. Каллрекордс. Девицеинфо</span><span class="sxs-lookup"><span data-stu-id="0be37-120">microsoft.graph.callRecords.deviceInfo</span></span>](callrecords-deviceinfo.md)|<span data-ttu-id="0be37-121">Сведения об устройстве, связанные с конечной точкой вызываемого носителя.</span><span class="sxs-lookup"><span data-stu-id="0be37-121">Device information associated with the callee endpoint of this media.</span></span>|
|<span data-ttu-id="0be37-122">каллинетворк</span><span class="sxs-lookup"><span data-stu-id="0be37-122">calleeNetwork</span></span>|[<span data-ttu-id="0be37-123">Microsoft. Graph. Каллрекордс. Нетворкинфо</span><span class="sxs-lookup"><span data-stu-id="0be37-123">microsoft.graph.callRecords.networkInfo</span></span>](callrecords-networkinfo.md)|<span data-ttu-id="0be37-124">Сведения о сети, связанные с конечной точкой вызываемого носителя.</span><span class="sxs-lookup"><span data-stu-id="0be37-124">Network information associated with the callee endpoint of this media.</span></span>|
|<span data-ttu-id="0be37-125">представлений</span><span class="sxs-lookup"><span data-stu-id="0be37-125">streams</span></span>|<span data-ttu-id="0be37-126">Коллекция [Microsoft. Graph. каллрекордс. медиастреам](callrecords-mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="0be37-126">[microsoft.graph.callRecords.mediaStream](callrecords-mediastream.md) collection</span></span>|<span data-ttu-id="0be37-127">Сетевые потоки, связанные с этим носителем.</span><span class="sxs-lookup"><span data-stu-id="0be37-127">Network streams associated with this media.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0be37-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0be37-128">JSON representation</span></span>

<span data-ttu-id="0be37-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0be37-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.media",
  "baseType": null
}-->

```json
{
  "label": "String",
  "callerDevice": {"@odata.type": "microsoft.graph.callRecords.deviceInfo"},
  "callerNetwork": {"@odata.type": "microsoft.graph.callRecords.networkInfo"},
  "calleeDevice": {"@odata.type": "microsoft.graph.callRecords.deviceInfo"},
  "calleeNetwork": {"@odata.type": "microsoft.graph.callRecords.networkInfo"},
  "streams": [{"@odata.type": "microsoft.graph.callRecords.mediaStream"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "media resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->