---
title: Тип ресурса АудиоконференЦинг
description: Представляет сведения о доступе к телефонной линии для собрания по сети.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8cff9b4405dc853e8502fccd9311899bb397b758
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999008"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="c9872-103">Тип ресурса АудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="c9872-103">audioConferencing resource type</span></span>

<span data-ttu-id="c9872-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9872-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9872-105">Представляет сведения о доступе к телефонии для [онлинемитинг](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="c9872-105">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c9872-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9872-106">Properties</span></span>

| <span data-ttu-id="c9872-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9872-107">Property</span></span>            | <span data-ttu-id="c9872-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c9872-108">Type</span></span>    | <span data-ttu-id="c9872-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c9872-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="c9872-110">диалинурл</span><span class="sxs-lookup"><span data-stu-id="c9872-110">dialinUrl</span></span>           | <span data-ttu-id="c9872-111">String</span><span class="sxs-lookup"><span data-stu-id="c9872-111">String</span></span>  | <span data-ttu-id="c9872-112">URL-адрес веб-страницы, которая содержит сведения о телефонном доступе.</span><span class="sxs-lookup"><span data-stu-id="c9872-112">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="c9872-113">конференцеид</span><span class="sxs-lookup"><span data-stu-id="c9872-113">ConferenceId</span></span>        | <span data-ttu-id="c9872-114">String</span><span class="sxs-lookup"><span data-stu-id="c9872-114">String</span></span>  | <span data-ttu-id="c9872-115">Идентификатор конференции онлайн-собрания.</span><span class="sxs-lookup"><span data-stu-id="c9872-115">The conference id of the online meeting.</span></span>      |
| <span data-ttu-id="c9872-116">толлфринумбер</span><span class="sxs-lookup"><span data-stu-id="c9872-116">tollFreeNumber</span></span>      | <span data-ttu-id="c9872-117">String</span><span class="sxs-lookup"><span data-stu-id="c9872-117">String</span></span>  | <span data-ttu-id="c9872-118">Бесплатный номер, который подключается к поставщику конференции с аудио.</span><span class="sxs-lookup"><span data-stu-id="c9872-118">The toll-free number that connects to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="c9872-119">толлнумбер</span><span class="sxs-lookup"><span data-stu-id="c9872-119">tollNumber</span></span>          | <span data-ttu-id="c9872-120">String</span><span class="sxs-lookup"><span data-stu-id="c9872-120">String</span></span>  | <span data-ttu-id="c9872-121">Платный номер, который подключается к поставщику конференции с аудио-и видеоконференциями.</span><span class="sxs-lookup"><span data-stu-id="c9872-121">The toll number that connects to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="c9872-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c9872-122">JSON representation</span></span>

<span data-ttu-id="c9872-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9872-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "ConferenceId": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


