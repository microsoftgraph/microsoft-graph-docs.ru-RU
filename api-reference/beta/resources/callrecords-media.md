---
title: Тип ресурса мультимедиа
description: Тип мультимедиа
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f550c898eda95026d5058c09d0e03f1064887509
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071587"
---
# <a name="media-resource-type"></a><span data-ttu-id="518da-103">Тип ресурса мультимедиа</span><span class="sxs-lookup"><span data-stu-id="518da-103">media resource type</span></span>

<span data-ttu-id="518da-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="518da-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="518da-105">Представляет мультимедиа (звук, видео, Видеообмен на экране и т. д.), используемые при вызове.</span><span class="sxs-lookup"><span data-stu-id="518da-105">Represents the media (audio, video, video-based screen-sharing, etc.) used in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="518da-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="518da-106">Properties</span></span>

| <span data-ttu-id="518da-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="518da-107">Property</span></span>     | <span data-ttu-id="518da-108">Тип</span><span class="sxs-lookup"><span data-stu-id="518da-108">Type</span></span>        | <span data-ttu-id="518da-109">Описание</span><span class="sxs-lookup"><span data-stu-id="518da-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="518da-110">label</span><span class="sxs-lookup"><span data-stu-id="518da-110">label</span></span>|<span data-ttu-id="518da-111">String</span><span class="sxs-lookup"><span data-stu-id="518da-111">String</span></span>|<span data-ttu-id="518da-112">Способ идентификации мультимедиа во время этапа согласования мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="518da-112">How the media was identified during media negotiation stage.</span></span>|
|<span data-ttu-id="518da-113">каллердевице</span><span class="sxs-lookup"><span data-stu-id="518da-113">callerDevice</span></span>|[<span data-ttu-id="518da-114">Microsoft. Graph. Каллрекордс. Девицеинфо</span><span class="sxs-lookup"><span data-stu-id="518da-114">microsoft.graph.callRecords.deviceInfo</span></span>](callrecords-deviceinfo.md)|<span data-ttu-id="518da-115">Сведения об устройстве, связанные с конечной точкой абонента этого носителя.</span><span class="sxs-lookup"><span data-stu-id="518da-115">Device information associated with the caller endpoint of this media.</span></span>|
|<span data-ttu-id="518da-116">каллернетворк</span><span class="sxs-lookup"><span data-stu-id="518da-116">callerNetwork</span></span>|[<span data-ttu-id="518da-117">Microsoft. Graph. Каллрекордс. Нетворкинфо</span><span class="sxs-lookup"><span data-stu-id="518da-117">microsoft.graph.callRecords.networkInfo</span></span>](callrecords-networkinfo.md)|<span data-ttu-id="518da-118">Сведения о сети, связанные с конечной точкой абонента этого носителя.</span><span class="sxs-lookup"><span data-stu-id="518da-118">Network information associated with the caller endpoint of this media.</span></span>|
|<span data-ttu-id="518da-119">каллидевице</span><span class="sxs-lookup"><span data-stu-id="518da-119">calleeDevice</span></span>|[<span data-ttu-id="518da-120">Microsoft. Graph. Каллрекордс. Девицеинфо</span><span class="sxs-lookup"><span data-stu-id="518da-120">microsoft.graph.callRecords.deviceInfo</span></span>](callrecords-deviceinfo.md)|<span data-ttu-id="518da-121">Сведения об устройстве, связанные с конечной точкой вызываемого носителя.</span><span class="sxs-lookup"><span data-stu-id="518da-121">Device information associated with the callee endpoint of this media.</span></span>|
|<span data-ttu-id="518da-122">каллинетворк</span><span class="sxs-lookup"><span data-stu-id="518da-122">calleeNetwork</span></span>|[<span data-ttu-id="518da-123">Microsoft. Graph. Каллрекордс. Нетворкинфо</span><span class="sxs-lookup"><span data-stu-id="518da-123">microsoft.graph.callRecords.networkInfo</span></span>](callrecords-networkinfo.md)|<span data-ttu-id="518da-124">Сведения о сети, связанные с конечной точкой вызываемого носителя.</span><span class="sxs-lookup"><span data-stu-id="518da-124">Network information associated with the callee endpoint of this media.</span></span>|
|<span data-ttu-id="518da-125">представлений</span><span class="sxs-lookup"><span data-stu-id="518da-125">streams</span></span>|<span data-ttu-id="518da-126">Коллекция [Microsoft. Graph. каллрекордс. медиастреам](callrecords-mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="518da-126">[microsoft.graph.callRecords.mediaStream](callrecords-mediastream.md) collection</span></span>|<span data-ttu-id="518da-127">Сетевые потоки, связанные с этим носителем.</span><span class="sxs-lookup"><span data-stu-id="518da-127">Network streams associated with this media.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="518da-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="518da-128">JSON representation</span></span>

<span data-ttu-id="518da-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="518da-129">The following is a JSON representation of the resource.</span></span>

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

