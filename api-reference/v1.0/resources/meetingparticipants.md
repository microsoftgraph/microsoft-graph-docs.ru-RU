---
title: Тип ресурса МитингпартиЦипантс
description: Участники собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ba13a5993a4969162a1b8753e6391afa01802dff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984259"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="cbfc6-103">Тип ресурса МитингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="cbfc6-103">meetingParticipants resource type</span></span>

<span data-ttu-id="cbfc6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbfc6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cbfc6-105">Участники собрания.</span><span class="sxs-lookup"><span data-stu-id="cbfc6-105">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="cbfc6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cbfc6-106">Properties</span></span>

| <span data-ttu-id="cbfc6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cbfc6-107">Property</span></span>       | <span data-ttu-id="cbfc6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cbfc6-108">Type</span></span>    | <span data-ttu-id="cbfc6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cbfc6-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cbfc6-110">attendees</span><span class="sxs-lookup"><span data-stu-id="cbfc6-110">attendees</span></span> | <span data-ttu-id="cbfc6-111">Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="cbfc6-111">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="cbfc6-112">organizer</span><span class="sxs-lookup"><span data-stu-id="cbfc6-112">organizer</span></span> | [<span data-ttu-id="cbfc6-113">митингпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="cbfc6-113">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="cbfc6-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cbfc6-114">JSON representation</span></span>

<span data-ttu-id="cbfc6-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cbfc6-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipants resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

