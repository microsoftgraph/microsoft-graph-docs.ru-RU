---
title: Тип ресурса МитингпартиЦипантс
description: Участники собрания.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b88a59b3d9def58217ca3badd833b275760b49c1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966838"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="9a18e-103">Тип ресурса МитингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="9a18e-103">meetingParticipants resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a18e-104">Участники собрания.</span><span class="sxs-lookup"><span data-stu-id="9a18e-104">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="9a18e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a18e-105">Properties</span></span>

| <span data-ttu-id="9a18e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a18e-106">Property</span></span>       | <span data-ttu-id="9a18e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9a18e-107">Type</span></span>    | <span data-ttu-id="9a18e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9a18e-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9a18e-109">attendees</span><span class="sxs-lookup"><span data-stu-id="9a18e-109">attendees</span></span> | <span data-ttu-id="9a18e-110">Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="9a18e-110">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="9a18e-111">organizer</span><span class="sxs-lookup"><span data-stu-id="9a18e-111">organizer</span></span> | [<span data-ttu-id="9a18e-112">МитингпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="9a18e-112">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="9a18e-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a18e-113">JSON representation</span></span>

<span data-ttu-id="9a18e-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a18e-114">The following is a JSON representation of the resource.</span></span>

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
