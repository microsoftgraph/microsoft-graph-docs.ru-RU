---
title: Тип ресурса Медиаинфо
description: Сведения о мультимедиа, используемые в действиях для запросов.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9d9b8f4709d3379afda8e30fec2b7db64a474a0e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866267"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="55559-103">Тип ресурса Медиаинфо</span><span class="sxs-lookup"><span data-stu-id="55559-103">mediaInfo resource type</span></span>

<span data-ttu-id="55559-104">Сведения о мультимедиа, используемые в действиях для запросов.</span><span class="sxs-lookup"><span data-stu-id="55559-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="55559-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="55559-105">Properties</span></span>
| <span data-ttu-id="55559-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="55559-106">Property</span></span>       | <span data-ttu-id="55559-107">Тип</span><span class="sxs-lookup"><span data-stu-id="55559-107">Type</span></span>    | <span data-ttu-id="55559-108">Описание</span><span class="sxs-lookup"><span data-stu-id="55559-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="55559-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="55559-109">resourceId</span></span>     | <span data-ttu-id="55559-110">String</span><span class="sxs-lookup"><span data-stu-id="55559-110">String</span></span>  | <span data-ttu-id="55559-111">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="55559-111">Optional.</span></span> <span data-ttu-id="55559-112">Используется для уникальной идентификации ресурса.</span><span class="sxs-lookup"><span data-stu-id="55559-112">Used to uniquely identity the resource.</span></span> <span data-ttu-id="55559-113">Если передается, URI приглашения кэшируется для этого resourceId в качестве ключа.</span><span class="sxs-lookup"><span data-stu-id="55559-113">If passed in, the prompt uri will be cached against this resourceId as a key.</span></span> |
| <span data-ttu-id="55559-114">URI</span><span class="sxs-lookup"><span data-stu-id="55559-114">uri</span></span>            | <span data-ttu-id="55559-115">String</span><span class="sxs-lookup"><span data-stu-id="55559-115">String</span></span>  | <span data-ttu-id="55559-116">Путь к приглашению, который будет воспроизводиться.</span><span class="sxs-lookup"><span data-stu-id="55559-116">Path to the prompt that will be played.</span></span> <span data-ttu-id="55559-117">В настоящее время поддерживается только формат волнового файла (WAV), одноканальный 16-разрядный пример с частотой выборки 16 000 (16 кГц).</span><span class="sxs-lookup"><span data-stu-id="55559-117">Currently supports only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="55559-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55559-118">JSON representation</span></span>

<span data-ttu-id="55559-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55559-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
