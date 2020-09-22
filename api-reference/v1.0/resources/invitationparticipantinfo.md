---
title: Тип ресурса ИнвитатионпартиЦипантинфо
description: '**ИнвитатионпартиЦипант** используется для представления набора удостоверений, связанных с приглашением на беседу, и предоставляет дополнительные параметры приглашения.'
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2425f7ebd6ac516a9100605c9ebfe47f1b87a114
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984252"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="66c34-103">Тип ресурса ИнвитатионпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="66c34-103">invitationParticipantInfo resource type</span></span>

<span data-ttu-id="66c34-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66c34-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="66c34-105">Этот ресурс используется для представления объекта, приглашенного на вызов группы.</span><span class="sxs-lookup"><span data-stu-id="66c34-105">This resource is used to represent the entity that is being invited to a group call.</span></span> 

## <a name="properties"></a><span data-ttu-id="66c34-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="66c34-106">Properties</span></span>

| <span data-ttu-id="66c34-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="66c34-107">Property</span></span>                           | <span data-ttu-id="66c34-108">Тип</span><span class="sxs-lookup"><span data-stu-id="66c34-108">Type</span></span>                          | <span data-ttu-id="66c34-109">Описание</span><span class="sxs-lookup"><span data-stu-id="66c34-109">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="66c34-110">хищения</span><span class="sxs-lookup"><span data-stu-id="66c34-110">identity</span></span>                           | [<span data-ttu-id="66c34-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="66c34-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="66c34-112">[Удостоверение](identityset.md) , связанное с этим приглашением.</span><span class="sxs-lookup"><span data-stu-id="66c34-112">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="66c34-113">реплацескаллид</span><span class="sxs-lookup"><span data-stu-id="66c34-113">replacesCallId</span></span>                     | <span data-ttu-id="66c34-114">String</span><span class="sxs-lookup"><span data-stu-id="66c34-114">String</span></span>                        | <span data-ttu-id="66c34-115">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="66c34-115">Optional.</span></span> <span data-ttu-id="66c34-116">Вызов, частью которого в данный момент является целевое удостоверение.</span><span class="sxs-lookup"><span data-stu-id="66c34-116">The call which the target identity is currently a part of.</span></span> <span data-ttu-id="66c34-117">Этот вызов будет сброшен после добавления участника.</span><span class="sxs-lookup"><span data-stu-id="66c34-117">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="66c34-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66c34-118">JSON representation</span></span>

<span data-ttu-id="66c34-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66c34-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "replacesCallId"
  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
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

