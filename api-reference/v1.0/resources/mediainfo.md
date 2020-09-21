---
title: Тип ресурса Медиаинфо
description: Сведения о мультимедиа, используемые в действиях для запросов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8e2f5a0d59f06449d122f4ca2db582afa4da9c39
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965528"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="d831d-103">Тип ресурса Медиаинфо</span><span class="sxs-lookup"><span data-stu-id="d831d-103">mediaInfo resource type</span></span>

<span data-ttu-id="d831d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d831d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d831d-105">Сведения о мультимедиа, используемые в действиях для запросов.</span><span class="sxs-lookup"><span data-stu-id="d831d-105">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="d831d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d831d-106">Properties</span></span>
| <span data-ttu-id="d831d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d831d-107">Property</span></span>       | <span data-ttu-id="d831d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d831d-108">Type</span></span>    | <span data-ttu-id="d831d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d831d-109">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="d831d-110">resourceId</span><span class="sxs-lookup"><span data-stu-id="d831d-110">resourceId</span></span>     | <span data-ttu-id="d831d-111">String</span><span class="sxs-lookup"><span data-stu-id="d831d-111">String</span></span>  | <span data-ttu-id="d831d-112">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d831d-112">Optional.</span></span> <span data-ttu-id="d831d-113">Используется для уникальной идентификации ресурса.</span><span class="sxs-lookup"><span data-stu-id="d831d-113">Used to uniquely identity the resource.</span></span> <span data-ttu-id="d831d-114">Если передается, URI приглашения кэшируется для этого resourceId в качестве ключа.</span><span class="sxs-lookup"><span data-stu-id="d831d-114">If passed in, the prompt uri will be cached against this resourceId as a key.</span></span> |
| <span data-ttu-id="d831d-115">URI</span><span class="sxs-lookup"><span data-stu-id="d831d-115">uri</span></span>            | <span data-ttu-id="d831d-116">String</span><span class="sxs-lookup"><span data-stu-id="d831d-116">String</span></span>  | <span data-ttu-id="d831d-117">Путь к приглашению, который будет воспроизводиться.</span><span class="sxs-lookup"><span data-stu-id="d831d-117">Path to the prompt that will be played.</span></span> <span data-ttu-id="d831d-118">В настоящее время поддерживается только формат волнового файла (WAV), одноканальный 16-разрядный пример с частотой выборки 16 000 (16 кГц).</span><span class="sxs-lookup"><span data-stu-id="d831d-118">Currently supports only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="d831d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d831d-119">JSON representation</span></span>

<span data-ttu-id="d831d-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d831d-120">The following is a JSON representation of the resource.</span></span>

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

