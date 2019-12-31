---
title: Тип ресурса АудиоконференЦинг
description: Представляет сведения о доступе к телефонной линии для собрания по сети.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f1c58fb5cbf65b73aed2978fd0b3be45d7d30aec
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913480"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="6df1b-103">Тип ресурса АудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="6df1b-103">audioConferencing resource type</span></span>

<span data-ttu-id="6df1b-104">Представляет сведения о доступе к телефонии для [онлинемитинг](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="6df1b-104">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6df1b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6df1b-105">Properties</span></span>

| <span data-ttu-id="6df1b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6df1b-106">Property</span></span>            | <span data-ttu-id="6df1b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6df1b-107">Type</span></span>    | <span data-ttu-id="6df1b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6df1b-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="6df1b-109">диалинурл</span><span class="sxs-lookup"><span data-stu-id="6df1b-109">dialinUrl</span></span>           | <span data-ttu-id="6df1b-110">String</span><span class="sxs-lookup"><span data-stu-id="6df1b-110">String</span></span>  | <span data-ttu-id="6df1b-111">URL-адрес веб-страницы, которая содержит сведения о телефонном доступе.</span><span class="sxs-lookup"><span data-stu-id="6df1b-111">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="6df1b-112">конференцеид</span><span class="sxs-lookup"><span data-stu-id="6df1b-112">ConferenceId</span></span>        | <span data-ttu-id="6df1b-113">String</span><span class="sxs-lookup"><span data-stu-id="6df1b-113">String</span></span>  | <span data-ttu-id="6df1b-114">Идентификатор конференции онлайн-собрания.</span><span class="sxs-lookup"><span data-stu-id="6df1b-114">The conference id of the online meeting.</span></span>      |
| <span data-ttu-id="6df1b-115">толлфринумбер</span><span class="sxs-lookup"><span data-stu-id="6df1b-115">tollFreeNumber</span></span>      | <span data-ttu-id="6df1b-116">String</span><span class="sxs-lookup"><span data-stu-id="6df1b-116">String</span></span>  | <span data-ttu-id="6df1b-117">Бесплатный номер, который подключается к поставщику конференции с аудио.</span><span class="sxs-lookup"><span data-stu-id="6df1b-117">The toll-free number that connects to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="6df1b-118">толлнумбер</span><span class="sxs-lookup"><span data-stu-id="6df1b-118">tollNumber</span></span>          | <span data-ttu-id="6df1b-119">String</span><span class="sxs-lookup"><span data-stu-id="6df1b-119">String</span></span>  | <span data-ttu-id="6df1b-120">Платный номер, который подключается к поставщику конференции с аудио-и видеоконференциями.</span><span class="sxs-lookup"><span data-stu-id="6df1b-120">The toll number that connects to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="6df1b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6df1b-121">JSON representation</span></span>

<span data-ttu-id="6df1b-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6df1b-122">The following is a JSON representation of the resource.</span></span>

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
