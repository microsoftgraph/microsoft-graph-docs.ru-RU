---
title: Тип ресурса АудиоконференЦинг
description: Представляет сведения о доступе к телефонной линии для собрания по сети.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d2eab9732660f53c7e003b49f6c6ca780c8a4610
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866277"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="89267-103">Тип ресурса АудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="89267-103">audioConferencing resource type</span></span>

<span data-ttu-id="89267-104">Представляет сведения о доступе к телефонии для [онлинемитинг](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="89267-104">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="89267-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="89267-105">Properties</span></span>

| <span data-ttu-id="89267-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="89267-106">Property</span></span>            | <span data-ttu-id="89267-107">Тип</span><span class="sxs-lookup"><span data-stu-id="89267-107">Type</span></span>    | <span data-ttu-id="89267-108">Описание</span><span class="sxs-lookup"><span data-stu-id="89267-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="89267-109">диалинурл</span><span class="sxs-lookup"><span data-stu-id="89267-109">dialinUrl</span></span>           | <span data-ttu-id="89267-110">String</span><span class="sxs-lookup"><span data-stu-id="89267-110">String</span></span>  | <span data-ttu-id="89267-111">URL-адрес веб-страницы, которая содержит сведения о телефонном доступе.</span><span class="sxs-lookup"><span data-stu-id="89267-111">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="89267-112">конференцеид</span><span class="sxs-lookup"><span data-stu-id="89267-112">ConferenceId</span></span>        | <span data-ttu-id="89267-113">String</span><span class="sxs-lookup"><span data-stu-id="89267-113">String</span></span>  | <span data-ttu-id="89267-114">Идентификатор конференции онлайн-собрания.</span><span class="sxs-lookup"><span data-stu-id="89267-114">The conference id of the online meeting.</span></span>      |
| <span data-ttu-id="89267-115">толлфринумбер</span><span class="sxs-lookup"><span data-stu-id="89267-115">tollFreeNumber</span></span>      | <span data-ttu-id="89267-116">String</span><span class="sxs-lookup"><span data-stu-id="89267-116">String</span></span>  | <span data-ttu-id="89267-117">Бесплатный номер, который подключается к поставщику конференции с аудио.</span><span class="sxs-lookup"><span data-stu-id="89267-117">The toll-free number that connects to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="89267-118">толлнумбер</span><span class="sxs-lookup"><span data-stu-id="89267-118">tollNumber</span></span>          | <span data-ttu-id="89267-119">String</span><span class="sxs-lookup"><span data-stu-id="89267-119">String</span></span>  | <span data-ttu-id="89267-120">Платный номер, который подключается к поставщику конференции с аудио-и видеоконференциями.</span><span class="sxs-lookup"><span data-stu-id="89267-120">The toll number that connects to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="89267-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89267-121">JSON representation</span></span>

<span data-ttu-id="89267-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89267-122">The following is a JSON representation of the resource.</span></span>

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
