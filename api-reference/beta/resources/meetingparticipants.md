---
title: Тип ресурса МитингпартиЦипантс
description: Участники собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e6d53d0359b9dc71e538c5bbe025e093a4912ffb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971659"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="0d9ef-103">Тип ресурса МитингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="0d9ef-103">meetingParticipants resource type</span></span>

<span data-ttu-id="0d9ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d9ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d9ef-105">Участники собрания.</span><span class="sxs-lookup"><span data-stu-id="0d9ef-105">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="0d9ef-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d9ef-106">Properties</span></span>

| <span data-ttu-id="0d9ef-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d9ef-107">Property</span></span>       | <span data-ttu-id="0d9ef-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0d9ef-108">Type</span></span>    | <span data-ttu-id="0d9ef-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0d9ef-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0d9ef-110">attendees</span><span class="sxs-lookup"><span data-stu-id="0d9ef-110">attendees</span></span> | <span data-ttu-id="0d9ef-111">Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="0d9ef-111">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="0d9ef-112">organizer</span><span class="sxs-lookup"><span data-stu-id="0d9ef-112">organizer</span></span> | [<span data-ttu-id="0d9ef-113">митингпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="0d9ef-113">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |
| <span data-ttu-id="0d9ef-114">производители</span><span class="sxs-lookup"><span data-stu-id="0d9ef-114">producers</span></span> | <span data-ttu-id="0d9ef-115">Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="0d9ef-115">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="0d9ef-116">Только для широковещательного собрания.</span><span class="sxs-lookup"><span data-stu-id="0d9ef-116">For broadcast meeting only.</span></span> |
| <span data-ttu-id="0d9ef-117">участники</span><span class="sxs-lookup"><span data-stu-id="0d9ef-117">contributors</span></span> | <span data-ttu-id="0d9ef-118">Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="0d9ef-118">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="0d9ef-119">Только для широковещательного собрания.</span><span class="sxs-lookup"><span data-stu-id="0d9ef-119">For broadcast meeting only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0d9ef-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d9ef-120">JSON representation</span></span>

<span data-ttu-id="0d9ef-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d9ef-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"},
  "producers": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "contributors": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
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


