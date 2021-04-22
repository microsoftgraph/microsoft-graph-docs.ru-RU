---
title: тип ресурса meetingParticipants
description: Участники собрания.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 93ca3d73518f9739cc3115c80efd2aec551629b5
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944165"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="e6adc-103">тип ресурса meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="e6adc-103">meetingParticipants resource type</span></span>

<span data-ttu-id="e6adc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6adc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6adc-105">Участники собрания.</span><span class="sxs-lookup"><span data-stu-id="e6adc-105">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="e6adc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6adc-106">Properties</span></span>

| <span data-ttu-id="e6adc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6adc-107">Property</span></span>                  | <span data-ttu-id="e6adc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e6adc-108">Type</span></span>                                                           | <span data-ttu-id="e6adc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e6adc-109">Description</span></span>                           |
| :------------------------ | :------------------------------------------------------------- | :------------------------------------ |
| <span data-ttu-id="e6adc-110">attendees</span><span class="sxs-lookup"><span data-stu-id="e6adc-110">attendees</span></span>                 | <span data-ttu-id="e6adc-111">[коллекция meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="e6adc-111">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="e6adc-112">Сведения участников собрания.</span><span class="sxs-lookup"><span data-stu-id="e6adc-112">Information of the meeting attendees.</span></span> |
| <span data-ttu-id="e6adc-113">organizer</span><span class="sxs-lookup"><span data-stu-id="e6adc-113">organizer</span></span>                 | [<span data-ttu-id="e6adc-114">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="e6adc-114">meetingParticipantInfo</span></span>](meetingparticipantinfo.md)            | <span data-ttu-id="e6adc-115">Сведения организатора собрания.</span><span class="sxs-lookup"><span data-stu-id="e6adc-115">Information of the meeting organizer.</span></span> |
| <span data-ttu-id="e6adc-116">производители (неподготовленные)</span><span class="sxs-lookup"><span data-stu-id="e6adc-116">producers (deprecated)</span></span>    | <span data-ttu-id="e6adc-117">[коллекция meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="e6adc-117">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="e6adc-118">Только для собрания трансляции.</span><span class="sxs-lookup"><span data-stu-id="e6adc-118">For broadcast meeting only.</span></span>           |
| <span data-ttu-id="e6adc-119">вкладчики (неподготовленные)</span><span class="sxs-lookup"><span data-stu-id="e6adc-119">contributors (deprecated)</span></span> | <span data-ttu-id="e6adc-120">[коллекция meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="e6adc-120">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="e6adc-121">Только для собрания трансляции.</span><span class="sxs-lookup"><span data-stu-id="e6adc-121">For broadcast meeting only.</span></span>           |

> [!CAUTION]
> <span data-ttu-id="e6adc-122">Свойства **производителей** и **авторов** неоценимы.</span><span class="sxs-lookup"><span data-stu-id="e6adc-122">The **producers** and **contributors** properties are deprecated.</span></span> <span data-ttu-id="e6adc-123">Все участники собрания возвращаются в **коллекцию участников.**</span><span class="sxs-lookup"><span data-stu-id="e6adc-123">All meeting participants are returned in the **attendees** collection.</span></span> <span data-ttu-id="e6adc-124">Используйте **свойство role** [meetingParticipantInfo](meetingparticipantinfo.md) для определения роли собрания участника.</span><span class="sxs-lookup"><span data-stu-id="e6adc-124">Use the **role** property of [meetingParticipantInfo](meetingparticipantinfo.md) to identify the meeting role of the attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6adc-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6adc-125">JSON representation</span></span>

<span data-ttu-id="e6adc-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6adc-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"},
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


