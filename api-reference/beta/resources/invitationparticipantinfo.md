---
title: Тип ресурса ИнвитатионпартиЦипантинфо
description: '**ИнвитатионпартиЦипант** используется для представления набора удостоверений, связанных с приглашением на беседу, и предоставляет дополнительные параметры приглашения.'
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 762e5dc75c03cda78581b90b54c3fea27a7f12f2
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636671"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="566b8-103">Тип ресурса ИнвитатионпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="566b8-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="566b8-104">Этот ресурс используется для представления набора удостоверений, связанных с приглашением на беседу, и предоставляет дополнительные параметры приглашения.</span><span class="sxs-lookup"><span data-stu-id="566b8-104">This resource is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="566b8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="566b8-105">Properties</span></span>

| <span data-ttu-id="566b8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="566b8-106">Property</span></span>                           | <span data-ttu-id="566b8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="566b8-107">Type</span></span>                          | <span data-ttu-id="566b8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="566b8-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="566b8-109">ендпоинттипе</span><span class="sxs-lookup"><span data-stu-id="566b8-109">endpointType</span></span>                       | <span data-ttu-id="566b8-110">String</span><span class="sxs-lookup"><span data-stu-id="566b8-110">String</span></span>                        | <span data-ttu-id="566b8-111">Тип конечной точки.</span><span class="sxs-lookup"><span data-stu-id="566b8-111">The type of endpoint.</span></span> <span data-ttu-id="566b8-112">Возможные значения: `default`, `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="566b8-112">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="566b8-113">хищения</span><span class="sxs-lookup"><span data-stu-id="566b8-113">identity</span></span>                           | [<span data-ttu-id="566b8-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="566b8-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="566b8-115">[Удостоверение](identityset.md) , связанное с этим приглашением.</span><span class="sxs-lookup"><span data-stu-id="566b8-115">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="566b8-116">реплацескаллид</span><span class="sxs-lookup"><span data-stu-id="566b8-116">replacesCallId</span></span>                     | <span data-ttu-id="566b8-117">String</span><span class="sxs-lookup"><span data-stu-id="566b8-117">String</span></span>                        | <span data-ttu-id="566b8-118">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="566b8-118">Optional.</span></span> <span data-ttu-id="566b8-119">Вызов, частью которого в данный момент является целевой иденити.</span><span class="sxs-lookup"><span data-stu-id="566b8-119">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="566b8-120">Этот вызов будет сброшен после добавления участника.</span><span class="sxs-lookup"><span data-stu-id="566b8-120">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="566b8-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="566b8-121">JSON representation</span></span>

<span data-ttu-id="566b8-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="566b8-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "endpointType",
    "replacesCallId"
  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "default | voicemail",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
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
