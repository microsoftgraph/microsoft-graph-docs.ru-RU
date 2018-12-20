---
title: Тип ресурса invitationParticipantInfo
description: '**InvitationParticipant** используется для представления набора удостоверения, связанного с приглашением беседы и предоставляет приглашение Дополнительные параметры.'
author: VinodRavichandran
ms.openlocfilehash: f833fcd0c555dfcc88da4027313ed7f40da81428
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380487"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="8aa40-103">Тип ресурса invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="8aa40-103">invitationParticipantInfo resource type</span></span>

> <span data-ttu-id="8aa40-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8aa40-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8aa40-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8aa40-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8aa40-106">**InvitationParticipant** используется для представления набора удостоверения, связанного с приглашением беседы и предоставляет приглашение Дополнительные параметры.</span><span class="sxs-lookup"><span data-stu-id="8aa40-106">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="8aa40-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8aa40-107">Properties</span></span>

| <span data-ttu-id="8aa40-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8aa40-108">Property</span></span>                           | <span data-ttu-id="8aa40-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8aa40-109">Type</span></span>                          | <span data-ttu-id="8aa40-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8aa40-110">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="8aa40-111">endpointType</span><span class="sxs-lookup"><span data-stu-id="8aa40-111">endpointType</span></span>                       | <span data-ttu-id="8aa40-112">String</span><span class="sxs-lookup"><span data-stu-id="8aa40-112">String</span></span>                        | <span data-ttu-id="8aa40-113">Возможные значения: `default`, `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="8aa40-113">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="8aa40-114">identity</span><span class="sxs-lookup"><span data-stu-id="8aa40-114">identity</span></span>                           | [<span data-ttu-id="8aa40-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="8aa40-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="8aa40-116">[IdentitySet](identityset.md) , связанной с приглашением.</span><span class="sxs-lookup"><span data-stu-id="8aa40-116">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="8aa40-117">languageId</span><span class="sxs-lookup"><span data-stu-id="8aa40-117">languageId</span></span>                         | <span data-ttu-id="8aa40-118">String</span><span class="sxs-lookup"><span data-stu-id="8aa40-118">String</span></span>                        | <span data-ttu-id="8aa40-119">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="8aa40-119">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="8aa40-120">область</span><span class="sxs-lookup"><span data-stu-id="8aa40-120">region</span></span>                             | <span data-ttu-id="8aa40-121">String</span><span class="sxs-lookup"><span data-stu-id="8aa40-121">String</span></span>                        | <span data-ttu-id="8aa40-122">Область участника.</span><span class="sxs-lookup"><span data-stu-id="8aa40-122">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="8aa40-123">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="8aa40-123">replacesCallId</span></span>                     | <span data-ttu-id="8aa40-124">String</span><span class="sxs-lookup"><span data-stu-id="8aa40-124">String</span></span>                        | <span data-ttu-id="8aa40-125">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="8aa40-125">Optional.</span></span> <span data-ttu-id="8aa40-126">Вызов которого idenity целевой в настоящее время является частью.</span><span class="sxs-lookup"><span data-stu-id="8aa40-126">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="8aa40-127">Этот звонок будет удалена, после добавления участника.</span><span class="sxs-lookup"><span data-stu-id="8aa40-127">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8aa40-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8aa40-128">JSON representation</span></span>

<span data-ttu-id="8aa40-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8aa40-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "default | voicemail",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "languageId": "String",
  "region": "String",
  "replacesCallId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
