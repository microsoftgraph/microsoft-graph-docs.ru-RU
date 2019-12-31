---
title: Тип ресурса Медиаинфо
description: Сведения о мультимедиа, используемые в действиях для запросов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d17117880cf736870d2728a9666af689a4296d04
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913298"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="cf1f3-103">Тип ресурса Медиаинфо</span><span class="sxs-lookup"><span data-stu-id="cf1f3-103">mediaInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf1f3-104">Сведения о мультимедиа, используемые в действиях для запросов.</span><span class="sxs-lookup"><span data-stu-id="cf1f3-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="cf1f3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf1f3-105">Properties</span></span>
| <span data-ttu-id="cf1f3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf1f3-106">Property</span></span>       | <span data-ttu-id="cf1f3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="cf1f3-107">Type</span></span>    | <span data-ttu-id="cf1f3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="cf1f3-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="cf1f3-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="cf1f3-109">resourceId</span></span>     | <span data-ttu-id="cf1f3-110">String</span><span class="sxs-lookup"><span data-stu-id="cf1f3-110">String</span></span>  | <span data-ttu-id="cf1f3-111">Необязательный параметр, используемый для уникальной идентификации ресурса.</span><span class="sxs-lookup"><span data-stu-id="cf1f3-111">Optional, used to uniquely identity the resource.</span></span> <span data-ttu-id="cf1f3-112">При передаче URI приглашения будет кэшироваться с этим ИД ресурса как key.</span><span class="sxs-lookup"><span data-stu-id="cf1f3-112">If passed the prompt uri will be cached against this resourceId as key.</span></span> |
| <span data-ttu-id="cf1f3-113">URI</span><span class="sxs-lookup"><span data-stu-id="cf1f3-113">uri</span></span>            | <span data-ttu-id="cf1f3-114">String</span><span class="sxs-lookup"><span data-stu-id="cf1f3-114">String</span></span>  | <span data-ttu-id="cf1f3-115">Путь к приглашению для воспроизведения.</span><span class="sxs-lookup"><span data-stu-id="cf1f3-115">Path to the prompt to be played.</span></span> <span data-ttu-id="cf1f3-116">В настоящее время поддерживается только формат волнового файла (WAV), 16-разрядных образцов с частотой 16 000 (16 кГц).</span><span class="sxs-lookup"><span data-stu-id="cf1f3-116">Currently only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate is only supported.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="cf1f3-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cf1f3-117">JSON representation</span></span>

<span data-ttu-id="cf1f3-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf1f3-118">The following is a JSON representation of the resource.</span></span>

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
