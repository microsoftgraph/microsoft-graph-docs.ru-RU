---
title: тип ресурса audioConferencing
description: Представляет сведения о доступе к телефону для собрания в Интернете.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9462971d1c2694b3443c9b3a4e799a24362eee80
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515641"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="43c9b-103">тип ресурса audioConferencing</span><span class="sxs-lookup"><span data-stu-id="43c9b-103">audioConferencing resource type</span></span>

<span data-ttu-id="43c9b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43c9b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="43c9b-105">Представляет сведения о доступе к телефону для [onlineMeeting.](onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="43c9b-105">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="43c9b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="43c9b-106">Properties</span></span>

| <span data-ttu-id="43c9b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="43c9b-107">Property</span></span>            | <span data-ttu-id="43c9b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="43c9b-108">Type</span></span>    | <span data-ttu-id="43c9b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="43c9b-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="43c9b-110">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="43c9b-110">dialinUrl</span></span>           | <span data-ttu-id="43c9b-111">Строка</span><span class="sxs-lookup"><span data-stu-id="43c9b-111">String</span></span>  | <span data-ttu-id="43c9b-112">URL-адрес веб-страницы, доступной извне, который содержит сведения о диалоговом номере.</span><span class="sxs-lookup"><span data-stu-id="43c9b-112">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="43c9b-113">conferenceId</span><span class="sxs-lookup"><span data-stu-id="43c9b-113">conferenceId</span></span>        | <span data-ttu-id="43c9b-114">Строка</span><span class="sxs-lookup"><span data-stu-id="43c9b-114">String</span></span>  | <span data-ttu-id="43c9b-115">ID конференции собрания в Интернете.</span><span class="sxs-lookup"><span data-stu-id="43c9b-115">The conference id of the online meeting.</span></span>      |
| <span data-ttu-id="43c9b-116">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="43c9b-116">tollFreeNumber</span></span>      | <span data-ttu-id="43c9b-117">Строка</span><span class="sxs-lookup"><span data-stu-id="43c9b-117">String</span></span>  | <span data-ttu-id="43c9b-118">Бесплатный номер, подключенный к поставщику аудиоконференции.</span><span class="sxs-lookup"><span data-stu-id="43c9b-118">The toll-free number that connects to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="43c9b-119">tollNumber</span><span class="sxs-lookup"><span data-stu-id="43c9b-119">tollNumber</span></span>          | <span data-ttu-id="43c9b-120">Строка</span><span class="sxs-lookup"><span data-stu-id="43c9b-120">String</span></span>  | <span data-ttu-id="43c9b-121">Платный номер, который подключается к поставщику аудиоконференции.</span><span class="sxs-lookup"><span data-stu-id="43c9b-121">The toll number that connects to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="43c9b-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="43c9b-122">JSON representation</span></span>

<span data-ttu-id="43c9b-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43c9b-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "conferenceId": "String",
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

