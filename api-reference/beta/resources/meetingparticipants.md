---
title: Тип ресурса meetingParticipants
description: Участники собрания.
author: VinodRavichandran
ms.openlocfilehash: 7e44863004dab5405251e2effaf2af8c2ae31f67
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380284"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="263ad-103">Тип ресурса meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="263ad-103">meetingParticipants resource type</span></span>

> <span data-ttu-id="263ad-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="263ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="263ad-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="263ad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="263ad-106">Участники собрания.</span><span class="sxs-lookup"><span data-stu-id="263ad-106">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="263ad-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="263ad-107">Properties</span></span>

| <span data-ttu-id="263ad-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="263ad-108">Property</span></span>       | <span data-ttu-id="263ad-109">Тип</span><span class="sxs-lookup"><span data-stu-id="263ad-109">Type</span></span>    | <span data-ttu-id="263ad-110">Описание</span><span class="sxs-lookup"><span data-stu-id="263ad-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="263ad-111">attendees</span><span class="sxs-lookup"><span data-stu-id="263ad-111">attendees</span></span> | <span data-ttu-id="263ad-112">[meetingParticipantInfo](meetingparticipantinfo.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="263ad-112">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="263ad-113">organizer</span><span class="sxs-lookup"><span data-stu-id="263ad-113">organizer</span></span> | [<span data-ttu-id="263ad-114">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="263ad-114">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="263ad-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="263ad-115">JSON representation</span></span>

<span data-ttu-id="263ad-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="263ad-116">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "meetingParticipants resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
