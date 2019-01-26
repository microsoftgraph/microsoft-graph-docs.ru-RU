---
title: Тип ресурса invitationParticipantInfo
description: '**InvitationParticipant** используется для представления набора удостоверения, связанного с приглашением беседы и предоставляет приглашение Дополнительные параметры.'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 666de597d40570a567ea88a375ab15d1e5f09038
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573601"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="6d2d7-103">Тип ресурса invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="6d2d7-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d2d7-104">**InvitationParticipant** используется для представления набора удостоверения, связанного с приглашением беседы и предоставляет приглашение Дополнительные параметры.</span><span class="sxs-lookup"><span data-stu-id="6d2d7-104">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="6d2d7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d2d7-105">Properties</span></span>

| <span data-ttu-id="6d2d7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d2d7-106">Property</span></span>                           | <span data-ttu-id="6d2d7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6d2d7-107">Type</span></span>                          | <span data-ttu-id="6d2d7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6d2d7-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="6d2d7-109">endpointType</span><span class="sxs-lookup"><span data-stu-id="6d2d7-109">endpointType</span></span>                       | <span data-ttu-id="6d2d7-110">operationStatus</span><span class="sxs-lookup"><span data-stu-id="6d2d7-110">operationStatus</span></span>               | <span data-ttu-id="6d2d7-111">Возможные значения: `default`, `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="6d2d7-111">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="6d2d7-112">identity</span><span class="sxs-lookup"><span data-stu-id="6d2d7-112">identity</span></span>                           | [<span data-ttu-id="6d2d7-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="6d2d7-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="6d2d7-114">[IdentitySet](identityset.md) , связанной с приглашением.</span><span class="sxs-lookup"><span data-stu-id="6d2d7-114">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="6d2d7-115">languageId</span><span class="sxs-lookup"><span data-stu-id="6d2d7-115">languageId</span></span>                         | <span data-ttu-id="6d2d7-116">Строка</span><span class="sxs-lookup"><span data-stu-id="6d2d7-116">String</span></span>                        | <span data-ttu-id="6d2d7-117">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="6d2d7-117">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="6d2d7-118">область</span><span class="sxs-lookup"><span data-stu-id="6d2d7-118">region</span></span>                             | <span data-ttu-id="6d2d7-119">Строка</span><span class="sxs-lookup"><span data-stu-id="6d2d7-119">String</span></span>                        | <span data-ttu-id="6d2d7-120">Область участника.</span><span class="sxs-lookup"><span data-stu-id="6d2d7-120">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="6d2d7-121">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="6d2d7-121">replacesCallId</span></span>                     | <span data-ttu-id="6d2d7-122">Строка</span><span class="sxs-lookup"><span data-stu-id="6d2d7-122">String</span></span>                        | <span data-ttu-id="6d2d7-123">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6d2d7-123">Optional.</span></span> <span data-ttu-id="6d2d7-124">Вызов которого idenity целевой в настоящее время является частью.</span><span class="sxs-lookup"><span data-stu-id="6d2d7-124">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="6d2d7-125">Этот звонок будет удалена, после добавления участника.</span><span class="sxs-lookup"><span data-stu-id="6d2d7-125">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6d2d7-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d2d7-126">JSON representation</span></span>

<span data-ttu-id="6d2d7-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d2d7-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "operationStatus",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "languageId": "String",
  "region": "String",
  "replacesCallId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/invitationparticipantinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
