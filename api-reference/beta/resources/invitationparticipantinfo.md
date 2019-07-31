---
title: Тип ресурса ИнвитатионпартиЦипантинфо
description: '**ИнвитатионпартиЦипант** используется для представления набора удостоверений, связанных с приглашением на беседу, и предоставляет дополнительные параметры приглашения.'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 570c2740cce2f4bc3b5584ba04ed50c9467591af
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967156"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="a7703-103">Тип ресурса ИнвитатионпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="a7703-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7703-104">**ИнвитатионпартиЦипант** используется для представления набора удостоверений, связанных с приглашением на беседу, и предоставляет дополнительные параметры приглашения.</span><span class="sxs-lookup"><span data-stu-id="a7703-104">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="a7703-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7703-105">Properties</span></span>

| <span data-ttu-id="a7703-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7703-106">Property</span></span>                           | <span data-ttu-id="a7703-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a7703-107">Type</span></span>                          | <span data-ttu-id="a7703-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a7703-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="a7703-109">Ендпоинттипе</span><span class="sxs-lookup"><span data-stu-id="a7703-109">endpointType</span></span>                       | <span data-ttu-id="a7703-110">String</span><span class="sxs-lookup"><span data-stu-id="a7703-110">String</span></span>                        | <span data-ttu-id="a7703-111">Возможные значения: `default`, `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="a7703-111">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="a7703-112">хищения</span><span class="sxs-lookup"><span data-stu-id="a7703-112">identity</span></span>                           | [<span data-ttu-id="a7703-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="a7703-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="a7703-114">[Удостоверение](identityset.md) , связанное с этим приглашением.</span><span class="sxs-lookup"><span data-stu-id="a7703-114">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="a7703-115">languageId</span><span class="sxs-lookup"><span data-stu-id="a7703-115">languageId</span></span>                         | <span data-ttu-id="a7703-116">String</span><span class="sxs-lookup"><span data-stu-id="a7703-116">String</span></span>                        | <span data-ttu-id="a7703-117">Строка языка и региональных параметров языка.</span><span class="sxs-lookup"><span data-stu-id="a7703-117">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="a7703-118">региональных</span><span class="sxs-lookup"><span data-stu-id="a7703-118">region</span></span>                             | <span data-ttu-id="a7703-119">String</span><span class="sxs-lookup"><span data-stu-id="a7703-119">String</span></span>                        | <span data-ttu-id="a7703-120">Регион участника.</span><span class="sxs-lookup"><span data-stu-id="a7703-120">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="a7703-121">Реплацескаллид</span><span class="sxs-lookup"><span data-stu-id="a7703-121">replacesCallId</span></span>                     | <span data-ttu-id="a7703-122">String</span><span class="sxs-lookup"><span data-stu-id="a7703-122">String</span></span>                        | <span data-ttu-id="a7703-123">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a7703-123">Optional.</span></span> <span data-ttu-id="a7703-124">Вызов, частью которого в данный момент является целевой иденити.</span><span class="sxs-lookup"><span data-stu-id="a7703-124">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="a7703-125">Этот вызов будет сброшен после добавления участника.</span><span class="sxs-lookup"><span data-stu-id="a7703-125">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a7703-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7703-126">JSON representation</span></span>

<span data-ttu-id="a7703-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7703-127">The following is a JSON representation of the resource.</span></span>

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
