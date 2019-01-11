---
title: Тип ресурса meetingParticipantInfo
description: Сведения о участник в собрании.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: d7b5ae17bd3bfb566bce0da9814b86aab98173da
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834260"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="071d4-103">Тип ресурса meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="071d4-103">meetingParticipantInfo resource type</span></span>

> <span data-ttu-id="071d4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="071d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="071d4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="071d4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="071d4-106">Сведения о участник в собрании.</span><span class="sxs-lookup"><span data-stu-id="071d4-106">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="071d4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="071d4-107">Properties</span></span>

| <span data-ttu-id="071d4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="071d4-108">Property</span></span>       | <span data-ttu-id="071d4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="071d4-109">Type</span></span>                          | <span data-ttu-id="071d4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="071d4-110">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="071d4-111">identity</span><span class="sxs-lookup"><span data-stu-id="071d4-111">identity</span></span>       | [<span data-ttu-id="071d4-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="071d4-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="071d4-113">Сведения об удостоверениях участника.</span><span class="sxs-lookup"><span data-stu-id="071d4-113">Identity information of the participant.</span></span> |
| <span data-ttu-id="071d4-114">Имя участника-пользователя</span><span class="sxs-lookup"><span data-stu-id="071d4-114">upn</span></span>            | <span data-ttu-id="071d4-115">Строка</span><span class="sxs-lookup"><span data-stu-id="071d4-115">String</span></span>                        | <span data-ttu-id="071d4-116">Имя участника-пользователя участника.</span><span class="sxs-lookup"><span data-stu-id="071d4-116">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="071d4-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="071d4-117">JSON representation</span></span>

<span data-ttu-id="071d4-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="071d4-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
