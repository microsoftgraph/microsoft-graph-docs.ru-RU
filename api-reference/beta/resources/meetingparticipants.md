---
title: Тип ресурса МитингпартиЦипантс
description: Участники собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 38071e4ab18127ca8f49b4ef4befdfafbf4c7e04
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522724"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="9494c-103">Тип ресурса МитингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="9494c-103">meetingParticipants resource type</span></span>

<span data-ttu-id="9494c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9494c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9494c-105">Участники собрания.</span><span class="sxs-lookup"><span data-stu-id="9494c-105">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="9494c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9494c-106">Properties</span></span>

| <span data-ttu-id="9494c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9494c-107">Property</span></span>       | <span data-ttu-id="9494c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9494c-108">Type</span></span>    | <span data-ttu-id="9494c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9494c-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9494c-110">attendees</span><span class="sxs-lookup"><span data-stu-id="9494c-110">attendees</span></span> | <span data-ttu-id="9494c-111">Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="9494c-111">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="9494c-112">organizer</span><span class="sxs-lookup"><span data-stu-id="9494c-112">organizer</span></span> | [<span data-ttu-id="9494c-113">митингпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="9494c-113">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |
| <span data-ttu-id="9494c-114">производители</span><span class="sxs-lookup"><span data-stu-id="9494c-114">producers</span></span> | <span data-ttu-id="9494c-115">Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="9494c-115">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="9494c-116">Только для широковещательного собрания.</span><span class="sxs-lookup"><span data-stu-id="9494c-116">For broadcast meeting only.</span></span> |
| <span data-ttu-id="9494c-117">участники</span><span class="sxs-lookup"><span data-stu-id="9494c-117">contributors</span></span> | <span data-ttu-id="9494c-118">Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="9494c-118">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="9494c-119">Только для широковещательного собрания.</span><span class="sxs-lookup"><span data-stu-id="9494c-119">For broadcast meeting only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9494c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9494c-120">JSON representation</span></span>

<span data-ttu-id="9494c-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9494c-121">The following is a JSON representation of the resource.</span></span>

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
