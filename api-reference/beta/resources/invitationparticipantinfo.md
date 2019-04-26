---
title: Тип ресурса ИнвитатионпартиЦипантинфо
description: '**ИнвитатионпартиЦипант** используется для представления набора удостоверений, связанных с приглашением на беседу, и предоставляет дополнительные параметры приглашения.'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb20dde1a74472695755e65dc404a6709f79c8b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569966"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="d86c1-103">Тип ресурса ИнвитатионпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="d86c1-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d86c1-104">**ИнвитатионпартиЦипант** используется для представления набора удостоверений, связанных с приглашением на беседу, и предоставляет дополнительные параметры приглашения.</span><span class="sxs-lookup"><span data-stu-id="d86c1-104">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="d86c1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d86c1-105">Properties</span></span>

| <span data-ttu-id="d86c1-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d86c1-106">Property</span></span>                           | <span data-ttu-id="d86c1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d86c1-107">Type</span></span>                          | <span data-ttu-id="d86c1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d86c1-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="d86c1-109">Ендпоинттипе</span><span class="sxs-lookup"><span data-stu-id="d86c1-109">endpointType</span></span>                       | <span data-ttu-id="d86c1-110">String</span><span class="sxs-lookup"><span data-stu-id="d86c1-110">String</span></span>                        | <span data-ttu-id="d86c1-111">Возможные значения: `default`, `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="d86c1-111">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="d86c1-112">хищения</span><span class="sxs-lookup"><span data-stu-id="d86c1-112">identity</span></span>                           | [<span data-ttu-id="d86c1-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="d86c1-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="d86c1-114">[Удостоверение](identityset.md) , связанное с этим приглашением.</span><span class="sxs-lookup"><span data-stu-id="d86c1-114">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="d86c1-115">languageId</span><span class="sxs-lookup"><span data-stu-id="d86c1-115">languageId</span></span>                         | <span data-ttu-id="d86c1-116">String</span><span class="sxs-lookup"><span data-stu-id="d86c1-116">String</span></span>                        | <span data-ttu-id="d86c1-117">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="d86c1-117">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="d86c1-118">региональных</span><span class="sxs-lookup"><span data-stu-id="d86c1-118">region</span></span>                             | <span data-ttu-id="d86c1-119">String</span><span class="sxs-lookup"><span data-stu-id="d86c1-119">String</span></span>                        | <span data-ttu-id="d86c1-120">Регион участника.</span><span class="sxs-lookup"><span data-stu-id="d86c1-120">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="d86c1-121">Реплацескаллид</span><span class="sxs-lookup"><span data-stu-id="d86c1-121">replacesCallId</span></span>                     | <span data-ttu-id="d86c1-122">String</span><span class="sxs-lookup"><span data-stu-id="d86c1-122">String</span></span>                        | <span data-ttu-id="d86c1-123">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="d86c1-123">Optional.</span></span> <span data-ttu-id="d86c1-124">Вызов, частью которого в данный момент является целевой иденити.</span><span class="sxs-lookup"><span data-stu-id="d86c1-124">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="d86c1-125">Этот вызов будет сброшен после добавления участника.</span><span class="sxs-lookup"><span data-stu-id="d86c1-125">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d86c1-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d86c1-126">JSON representation</span></span>

<span data-ttu-id="d86c1-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d86c1-127">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
