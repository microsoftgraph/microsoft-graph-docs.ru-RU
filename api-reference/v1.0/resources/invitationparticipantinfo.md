---
title: Тип ресурса ИнвитатионпартиЦипантинфо
description: '**ИнвитатионпартиЦипант** используется для представления набора удостоверений, связанных с приглашением на беседу, и предоставляет дополнительные параметры приглашения.'
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1e1dc861fb1580744ed3b956338934a443f0e661
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866269"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="17dff-103">Тип ресурса ИнвитатионпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="17dff-103">invitationParticipantInfo resource type</span></span>

<span data-ttu-id="17dff-104">Этот ресурс используется для представления объекта, приглашенного на вызов группы.</span><span class="sxs-lookup"><span data-stu-id="17dff-104">This resource is used to represent the entity that is being invited to a group call.</span></span> 

## <a name="properties"></a><span data-ttu-id="17dff-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="17dff-105">Properties</span></span>

| <span data-ttu-id="17dff-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="17dff-106">Property</span></span>                           | <span data-ttu-id="17dff-107">Тип</span><span class="sxs-lookup"><span data-stu-id="17dff-107">Type</span></span>                          | <span data-ttu-id="17dff-108">Описание</span><span class="sxs-lookup"><span data-stu-id="17dff-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="17dff-109">хищения</span><span class="sxs-lookup"><span data-stu-id="17dff-109">identity</span></span>                           | [<span data-ttu-id="17dff-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="17dff-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="17dff-111">[Удостоверение](identityset.md) , связанное с этим приглашением.</span><span class="sxs-lookup"><span data-stu-id="17dff-111">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="17dff-112">реплацескаллид</span><span class="sxs-lookup"><span data-stu-id="17dff-112">replacesCallId</span></span>                     | <span data-ttu-id="17dff-113">String</span><span class="sxs-lookup"><span data-stu-id="17dff-113">String</span></span>                        | <span data-ttu-id="17dff-114">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="17dff-114">Optional.</span></span> <span data-ttu-id="17dff-115">Вызов, частью которого в данный момент является целевое удостоверение.</span><span class="sxs-lookup"><span data-stu-id="17dff-115">The call which the target identity is currently a part of.</span></span> <span data-ttu-id="17dff-116">Этот вызов будет сброшен после добавления участника.</span><span class="sxs-lookup"><span data-stu-id="17dff-116">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="17dff-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="17dff-117">JSON representation</span></span>

<span data-ttu-id="17dff-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17dff-118">The following is a JSON representation of the resource.</span></span>

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
