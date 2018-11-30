---
title: Тип ресурса meetingParticipantInfo
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 1d9c22924f8f05255b5e01bad4bbcd6ae5957ffe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078476"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="403fb-103">Тип ресурса meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="403fb-103">meetingParticipantInfo resource type</span></span>

> <span data-ttu-id="403fb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="403fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="403fb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="403fb-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="403fb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="403fb-106">Properties</span></span>

| <span data-ttu-id="403fb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="403fb-107">Property</span></span>       | <span data-ttu-id="403fb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="403fb-108">Type</span></span>                          | <span data-ttu-id="403fb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="403fb-109">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="403fb-110">identity</span><span class="sxs-lookup"><span data-stu-id="403fb-110">identity</span></span>       | [<span data-ttu-id="403fb-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="403fb-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="403fb-112">Сведения об удостоверениях участника.</span><span class="sxs-lookup"><span data-stu-id="403fb-112">Identity information of the participant.</span></span> |
| <span data-ttu-id="403fb-113">Имя участника-пользователя</span><span class="sxs-lookup"><span data-stu-id="403fb-113">upn</span></span>            | <span data-ttu-id="403fb-114">String</span><span class="sxs-lookup"><span data-stu-id="403fb-114">String</span></span>                        | <span data-ttu-id="403fb-115">Имя участника-пользователя участника.</span><span class="sxs-lookup"><span data-stu-id="403fb-115">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="403fb-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="403fb-116">JSON representation</span></span>

<span data-ttu-id="403fb-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="403fb-117">The following is a JSON representation of the resource.</span></span>

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
