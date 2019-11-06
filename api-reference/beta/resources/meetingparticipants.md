---
title: Тип ресурса МитингпартиЦипантс
description: Участники собрания.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 171d24629c8a219f788ad17cdf97874bbf299a62
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006629"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="64486-103">Тип ресурса МитингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="64486-103">meetingParticipants resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64486-104">Участники собрания.</span><span class="sxs-lookup"><span data-stu-id="64486-104">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="64486-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="64486-105">Properties</span></span>

| <span data-ttu-id="64486-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="64486-106">Property</span></span>       | <span data-ttu-id="64486-107">Тип</span><span class="sxs-lookup"><span data-stu-id="64486-107">Type</span></span>    | <span data-ttu-id="64486-108">Описание</span><span class="sxs-lookup"><span data-stu-id="64486-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="64486-109">attendees</span><span class="sxs-lookup"><span data-stu-id="64486-109">attendees</span></span> | <span data-ttu-id="64486-110">Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="64486-110">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="64486-111">organizer</span><span class="sxs-lookup"><span data-stu-id="64486-111">organizer</span></span> | [<span data-ttu-id="64486-112">митингпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="64486-112">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |
| <span data-ttu-id="64486-113">производители</span><span class="sxs-lookup"><span data-stu-id="64486-113">producers</span></span> | <span data-ttu-id="64486-114">Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="64486-114">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="64486-115">Только для широковещательного собрания.</span><span class="sxs-lookup"><span data-stu-id="64486-115">For broadcast meeting only.</span></span> |
| <span data-ttu-id="64486-116">участники</span><span class="sxs-lookup"><span data-stu-id="64486-116">contributors</span></span> | <span data-ttu-id="64486-117">Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="64486-117">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="64486-118">Только для широковещательного собрания.</span><span class="sxs-lookup"><span data-stu-id="64486-118">For broadcast meeting only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="64486-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64486-119">JSON representation</span></span>

<span data-ttu-id="64486-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64486-120">The following is a JSON representation of the resource.</span></span>

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
