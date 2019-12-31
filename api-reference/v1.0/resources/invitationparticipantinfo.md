---
title: Тип ресурса ИнвитатионпартиЦипантинфо
description: '**ИнвитатионпартиЦипант** используется для представления набора удостоверений, связанных с приглашением на беседу, и предоставляет дополнительные параметры приглашения.'
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8b42e89f89332e58fa2f7edcf39c774446c6b9d9
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913403"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="7649a-103">Тип ресурса ИнвитатионпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="7649a-103">invitationParticipantInfo resource type</span></span>

<span data-ttu-id="7649a-104">Этот ресурс используется для представления объекта, приглашенного на вызов группы.</span><span class="sxs-lookup"><span data-stu-id="7649a-104">This resource is used to represent the entity that is being invited to a group call.</span></span> 

## <a name="properties"></a><span data-ttu-id="7649a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7649a-105">Properties</span></span>

| <span data-ttu-id="7649a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7649a-106">Property</span></span>                           | <span data-ttu-id="7649a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7649a-107">Type</span></span>                          | <span data-ttu-id="7649a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7649a-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="7649a-109">хищения</span><span class="sxs-lookup"><span data-stu-id="7649a-109">identity</span></span>                           | [<span data-ttu-id="7649a-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="7649a-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="7649a-111">[Удостоверение](identityset.md) , связанное с этим приглашением.</span><span class="sxs-lookup"><span data-stu-id="7649a-111">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="7649a-112">реплацескаллид</span><span class="sxs-lookup"><span data-stu-id="7649a-112">replacesCallId</span></span>                     | <span data-ttu-id="7649a-113">String</span><span class="sxs-lookup"><span data-stu-id="7649a-113">String</span></span>                        | <span data-ttu-id="7649a-114">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7649a-114">Optional.</span></span> <span data-ttu-id="7649a-115">Вызов, частью которого в данный момент является целевое удостоверение.</span><span class="sxs-lookup"><span data-stu-id="7649a-115">The call which the target identity is currently a part of.</span></span> <span data-ttu-id="7649a-116">Этот вызов будет сброшен после добавления участника.</span><span class="sxs-lookup"><span data-stu-id="7649a-116">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7649a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7649a-117">JSON representation</span></span>

<span data-ttu-id="7649a-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7649a-118">The following is a JSON representation of the resource.</span></span>

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
