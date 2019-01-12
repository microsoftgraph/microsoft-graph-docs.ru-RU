---
title: Тип ресурса meetingParticipantInfo
description: Сведения о участник в собрании.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 409cf7eff4b1151a0ded11674fcde36a519f0e7f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924484"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="34908-103">Тип ресурса meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="34908-103">meetingParticipantInfo resource type</span></span>

> <span data-ttu-id="34908-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="34908-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34908-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34908-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34908-106">Сведения о участник в собрании.</span><span class="sxs-lookup"><span data-stu-id="34908-106">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="34908-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="34908-107">Properties</span></span>

| <span data-ttu-id="34908-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="34908-108">Property</span></span>       | <span data-ttu-id="34908-109">Тип</span><span class="sxs-lookup"><span data-stu-id="34908-109">Type</span></span>                          | <span data-ttu-id="34908-110">Описание</span><span class="sxs-lookup"><span data-stu-id="34908-110">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="34908-111">identity</span><span class="sxs-lookup"><span data-stu-id="34908-111">identity</span></span>       | [<span data-ttu-id="34908-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="34908-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="34908-113">Сведения об удостоверениях участника.</span><span class="sxs-lookup"><span data-stu-id="34908-113">Identity information of the participant.</span></span> |
| <span data-ttu-id="34908-114">Имя участника-пользователя</span><span class="sxs-lookup"><span data-stu-id="34908-114">upn</span></span>            | <span data-ttu-id="34908-115">String</span><span class="sxs-lookup"><span data-stu-id="34908-115">String</span></span>                        | <span data-ttu-id="34908-116">Имя участника-пользователя участника.</span><span class="sxs-lookup"><span data-stu-id="34908-116">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="34908-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34908-117">JSON representation</span></span>

<span data-ttu-id="34908-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34908-118">The following is a JSON representation of the resource.</span></span>

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
