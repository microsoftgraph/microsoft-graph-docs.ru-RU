---
title: Тип ресурса Медиаинфо
description: Сведения о мультимедиа, используемые в действиях для запросов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b7e2b5fb0e00a7b173e1e14962b614fcca5382f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971749"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="8ab0d-103">Тип ресурса Медиаинфо</span><span class="sxs-lookup"><span data-stu-id="8ab0d-103">mediaInfo resource type</span></span>

<span data-ttu-id="8ab0d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ab0d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ab0d-105">Сведения о мультимедиа, используемые в действиях для запросов.</span><span class="sxs-lookup"><span data-stu-id="8ab0d-105">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="8ab0d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ab0d-106">Properties</span></span>
| <span data-ttu-id="8ab0d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ab0d-107">Property</span></span>       | <span data-ttu-id="8ab0d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8ab0d-108">Type</span></span>    | <span data-ttu-id="8ab0d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8ab0d-109">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="8ab0d-110">resourceId</span><span class="sxs-lookup"><span data-stu-id="8ab0d-110">resourceId</span></span>     | <span data-ttu-id="8ab0d-111">String</span><span class="sxs-lookup"><span data-stu-id="8ab0d-111">String</span></span>  | <span data-ttu-id="8ab0d-112">Необязательный параметр, используемый для уникальной идентификации ресурса.</span><span class="sxs-lookup"><span data-stu-id="8ab0d-112">Optional, used to uniquely identity the resource.</span></span> <span data-ttu-id="8ab0d-113">При передаче URI приглашения будет кэшироваться с этим ИД ресурса как key.</span><span class="sxs-lookup"><span data-stu-id="8ab0d-113">If passed the prompt uri will be cached against this resourceId as key.</span></span> |
| <span data-ttu-id="8ab0d-114">URI</span><span class="sxs-lookup"><span data-stu-id="8ab0d-114">uri</span></span>            | <span data-ttu-id="8ab0d-115">String</span><span class="sxs-lookup"><span data-stu-id="8ab0d-115">String</span></span>  | <span data-ttu-id="8ab0d-116">Путь к приглашению для воспроизведения.</span><span class="sxs-lookup"><span data-stu-id="8ab0d-116">Path to the prompt to be played.</span></span> <span data-ttu-id="8ab0d-117">В настоящее время поддерживается только формат волнового файла (WAV), 16-разрядных образцов с частотой 16 000 (16 кГц).</span><span class="sxs-lookup"><span data-stu-id="8ab0d-117">Currently only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate is only supported.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="8ab0d-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ab0d-118">JSON representation</span></span>

<span data-ttu-id="8ab0d-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ab0d-119">The following is a JSON representation of the resource.</span></span>

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


