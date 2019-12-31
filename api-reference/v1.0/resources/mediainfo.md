---
title: Тип ресурса Медиаинфо
description: Сведения о мультимедиа, используемые в действиях для запросов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 20134131dba64ad48effa1c95e5d81ab81102805
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913207"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="be5ec-103">Тип ресурса Медиаинфо</span><span class="sxs-lookup"><span data-stu-id="be5ec-103">mediaInfo resource type</span></span>

<span data-ttu-id="be5ec-104">Сведения о мультимедиа, используемые в действиях для запросов.</span><span class="sxs-lookup"><span data-stu-id="be5ec-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="be5ec-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="be5ec-105">Properties</span></span>
| <span data-ttu-id="be5ec-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="be5ec-106">Property</span></span>       | <span data-ttu-id="be5ec-107">Тип</span><span class="sxs-lookup"><span data-stu-id="be5ec-107">Type</span></span>    | <span data-ttu-id="be5ec-108">Описание</span><span class="sxs-lookup"><span data-stu-id="be5ec-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="be5ec-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="be5ec-109">resourceId</span></span>     | <span data-ttu-id="be5ec-110">String</span><span class="sxs-lookup"><span data-stu-id="be5ec-110">String</span></span>  | <span data-ttu-id="be5ec-111">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="be5ec-111">Optional.</span></span> <span data-ttu-id="be5ec-112">Используется для уникальной идентификации ресурса.</span><span class="sxs-lookup"><span data-stu-id="be5ec-112">Used to uniquely identity the resource.</span></span> <span data-ttu-id="be5ec-113">Если передается, URI приглашения кэшируется для этого resourceId в качестве ключа.</span><span class="sxs-lookup"><span data-stu-id="be5ec-113">If passed in, the prompt uri will be cached against this resourceId as a key.</span></span> |
| <span data-ttu-id="be5ec-114">URI</span><span class="sxs-lookup"><span data-stu-id="be5ec-114">uri</span></span>            | <span data-ttu-id="be5ec-115">String</span><span class="sxs-lookup"><span data-stu-id="be5ec-115">String</span></span>  | <span data-ttu-id="be5ec-116">Путь к приглашению, который будет воспроизводиться.</span><span class="sxs-lookup"><span data-stu-id="be5ec-116">Path to the prompt that will be played.</span></span> <span data-ttu-id="be5ec-117">В настоящее время поддерживается только формат волнового файла (WAV), одноканальный 16-разрядный пример с частотой выборки 16 000 (16 кГц).</span><span class="sxs-lookup"><span data-stu-id="be5ec-117">Currently supports only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="be5ec-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be5ec-118">JSON representation</span></span>

<span data-ttu-id="be5ec-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be5ec-119">The following is a JSON representation of the resource.</span></span>

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
