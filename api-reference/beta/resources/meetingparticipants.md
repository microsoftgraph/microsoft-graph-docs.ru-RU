---
title: Тип ресурса МитингпартиЦипантс
description: Участники собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 66bb521ae9a2222b5ea60709ac3687da930161d6
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913557"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="9b5bd-103">Тип ресурса МитингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="9b5bd-103">meetingParticipants resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b5bd-104">Участники собрания.</span><span class="sxs-lookup"><span data-stu-id="9b5bd-104">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="9b5bd-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b5bd-105">Properties</span></span>

| <span data-ttu-id="9b5bd-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b5bd-106">Property</span></span>       | <span data-ttu-id="9b5bd-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9b5bd-107">Type</span></span>    | <span data-ttu-id="9b5bd-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9b5bd-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9b5bd-109">attendees</span><span class="sxs-lookup"><span data-stu-id="9b5bd-109">attendees</span></span> | <span data-ttu-id="9b5bd-110">Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="9b5bd-110">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="9b5bd-111">organizer</span><span class="sxs-lookup"><span data-stu-id="9b5bd-111">organizer</span></span> | [<span data-ttu-id="9b5bd-112">митингпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="9b5bd-112">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |
| <span data-ttu-id="9b5bd-113">производители</span><span class="sxs-lookup"><span data-stu-id="9b5bd-113">producers</span></span> | <span data-ttu-id="9b5bd-114">Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="9b5bd-114">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="9b5bd-115">Только для широковещательного собрания.</span><span class="sxs-lookup"><span data-stu-id="9b5bd-115">For broadcast meeting only.</span></span> |
| <span data-ttu-id="9b5bd-116">участники</span><span class="sxs-lookup"><span data-stu-id="9b5bd-116">contributors</span></span> | <span data-ttu-id="9b5bd-117">Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="9b5bd-117">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="9b5bd-118">Только для широковещательного собрания.</span><span class="sxs-lookup"><span data-stu-id="9b5bd-118">For broadcast meeting only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9b5bd-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b5bd-119">JSON representation</span></span>

<span data-ttu-id="9b5bd-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b5bd-120">The following is a JSON representation of the resource.</span></span>

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
