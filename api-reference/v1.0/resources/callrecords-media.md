---
title: Тип ресурса мультимедиа
description: Тип мультимедиа
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2b720405e1420cdffc13655175a0575e1bf19170
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601344"
---
# <a name="media-resource-type"></a><span data-ttu-id="0b0a9-103">Тип ресурса мультимедиа</span><span class="sxs-lookup"><span data-stu-id="0b0a9-103">media resource type</span></span>

<span data-ttu-id="0b0a9-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="0b0a9-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="0b0a9-105">Представляет мультимедиа (звук, видео, Видеообмен на экране и т. д.), используемые при вызове.</span><span class="sxs-lookup"><span data-stu-id="0b0a9-105">Represents the media (audio, video, video-based screen-sharing, etc.) used in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="0b0a9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b0a9-106">Properties</span></span>

| <span data-ttu-id="0b0a9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b0a9-107">Property</span></span>     | <span data-ttu-id="0b0a9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0b0a9-108">Type</span></span>        | <span data-ttu-id="0b0a9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0b0a9-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0b0a9-110">label</span><span class="sxs-lookup"><span data-stu-id="0b0a9-110">label</span></span>|<span data-ttu-id="0b0a9-111">String</span><span class="sxs-lookup"><span data-stu-id="0b0a9-111">String</span></span>|<span data-ttu-id="0b0a9-112">Способ идентификации мультимедиа во время этапа согласования мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="0b0a9-112">How the media was identified during media negotiation stage.</span></span>|
|<span data-ttu-id="0b0a9-113">каллердевице</span><span class="sxs-lookup"><span data-stu-id="0b0a9-113">callerDevice</span></span>|[<span data-ttu-id="0b0a9-114">Microsoft. Graph. Каллрекордс. Девицеинфо</span><span class="sxs-lookup"><span data-stu-id="0b0a9-114">microsoft.graph.callRecords.deviceInfo</span></span>](callrecords-deviceinfo.md)|<span data-ttu-id="0b0a9-115">Сведения об устройстве, связанные с конечной точкой абонента этого носителя.</span><span class="sxs-lookup"><span data-stu-id="0b0a9-115">Device information associated with the caller endpoint of this media.</span></span>|
|<span data-ttu-id="0b0a9-116">каллернетворк</span><span class="sxs-lookup"><span data-stu-id="0b0a9-116">callerNetwork</span></span>|[<span data-ttu-id="0b0a9-117">Microsoft. Graph. Каллрекордс. Нетворкинфо</span><span class="sxs-lookup"><span data-stu-id="0b0a9-117">microsoft.graph.callRecords.networkInfo</span></span>](callrecords-networkinfo.md)|<span data-ttu-id="0b0a9-118">Сведения о сети, связанные с конечной точкой абонента этого носителя.</span><span class="sxs-lookup"><span data-stu-id="0b0a9-118">Network information associated with the caller endpoint of this media.</span></span>|
|<span data-ttu-id="0b0a9-119">каллидевице</span><span class="sxs-lookup"><span data-stu-id="0b0a9-119">calleeDevice</span></span>|[<span data-ttu-id="0b0a9-120">Microsoft. Graph. Каллрекордс. Девицеинфо</span><span class="sxs-lookup"><span data-stu-id="0b0a9-120">microsoft.graph.callRecords.deviceInfo</span></span>](callrecords-deviceinfo.md)|<span data-ttu-id="0b0a9-121">Сведения об устройстве, связанные с конечной точкой вызываемого носителя.</span><span class="sxs-lookup"><span data-stu-id="0b0a9-121">Device information associated with the callee endpoint of this media.</span></span>|
|<span data-ttu-id="0b0a9-122">каллинетворк</span><span class="sxs-lookup"><span data-stu-id="0b0a9-122">calleeNetwork</span></span>|[<span data-ttu-id="0b0a9-123">Microsoft. Graph. Каллрекордс. Нетворкинфо</span><span class="sxs-lookup"><span data-stu-id="0b0a9-123">microsoft.graph.callRecords.networkInfo</span></span>](callrecords-networkinfo.md)|<span data-ttu-id="0b0a9-124">Сведения о сети, связанные с конечной точкой вызываемого носителя.</span><span class="sxs-lookup"><span data-stu-id="0b0a9-124">Network information associated with the callee endpoint of this media.</span></span>|
|<span data-ttu-id="0b0a9-125">представлений</span><span class="sxs-lookup"><span data-stu-id="0b0a9-125">streams</span></span>|<span data-ttu-id="0b0a9-126">Коллекция [Microsoft. Graph. каллрекордс. медиастреам](callrecords-mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="0b0a9-126">[microsoft.graph.callRecords.mediaStream](callrecords-mediastream.md) collection</span></span>|<span data-ttu-id="0b0a9-127">Сетевые потоки, связанные с этим носителем.</span><span class="sxs-lookup"><span data-stu-id="0b0a9-127">Network streams associated with this media.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b0a9-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b0a9-128">JSON representation</span></span>

<span data-ttu-id="0b0a9-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b0a9-129">The following is a JSON representation of the resource.</span></span>

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
