---
title: Тип ресурса ИнвитатионпартиЦипантинфо
description: Представляет объект, приглашенный на вызов группы.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 7250f51b39d1e046b06eb94e1cd8e01ec5fd6bfe
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913536"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="418b3-103">Тип ресурса ИнвитатионпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="418b3-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="418b3-104">Представляет объект, приглашенный на вызов группы.</span><span class="sxs-lookup"><span data-stu-id="418b3-104">Represents an entity that is being invited to a group call.</span></span> 

## <a name="properties"></a><span data-ttu-id="418b3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="418b3-105">Properties</span></span>

| <span data-ttu-id="418b3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="418b3-106">Property</span></span>                           | <span data-ttu-id="418b3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="418b3-107">Type</span></span>                          | <span data-ttu-id="418b3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="418b3-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="418b3-109">ендпоинттипе</span><span class="sxs-lookup"><span data-stu-id="418b3-109">endpointType</span></span>                       | <span data-ttu-id="418b3-110">String</span><span class="sxs-lookup"><span data-stu-id="418b3-110">String</span></span>                        | <span data-ttu-id="418b3-111">Тип конечной точки.</span><span class="sxs-lookup"><span data-stu-id="418b3-111">The type of endpoint.</span></span> <span data-ttu-id="418b3-112">Возможные значения: `default`, `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="418b3-112">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="418b3-113">хищения</span><span class="sxs-lookup"><span data-stu-id="418b3-113">identity</span></span>                           | [<span data-ttu-id="418b3-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="418b3-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="418b3-115">[Удостоверение](identityset.md) , связанное с этим приглашением.</span><span class="sxs-lookup"><span data-stu-id="418b3-115">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="418b3-116">реплацескаллид</span><span class="sxs-lookup"><span data-stu-id="418b3-116">replacesCallId</span></span>                     | <span data-ttu-id="418b3-117">String</span><span class="sxs-lookup"><span data-stu-id="418b3-117">String</span></span>                        | <span data-ttu-id="418b3-118">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="418b3-118">Optional.</span></span> <span data-ttu-id="418b3-119">Вызов, частью которого в данный момент является целевой иденити.</span><span class="sxs-lookup"><span data-stu-id="418b3-119">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="418b3-120">Этот вызов будет сброшен после добавления участника.</span><span class="sxs-lookup"><span data-stu-id="418b3-120">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="418b3-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="418b3-121">JSON representation</span></span>

<span data-ttu-id="418b3-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="418b3-122">The following is a JSON representation of the resource.</span></span>

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
