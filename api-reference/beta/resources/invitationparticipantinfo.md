---
title: Тип ресурса ИнвитатионпартиЦипантинфо
description: Представляет объект, приглашенный на вызов группы.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a21ffce09a7f086bced5416eace2a95170b3eaf2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523186"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="459a6-103">Тип ресурса ИнвитатионпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="459a6-103">invitationParticipantInfo resource type</span></span>

<span data-ttu-id="459a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="459a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="459a6-105">Представляет объект, приглашенный на вызов группы.</span><span class="sxs-lookup"><span data-stu-id="459a6-105">Represents an entity that is being invited to a group call.</span></span> 

## <a name="properties"></a><span data-ttu-id="459a6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="459a6-106">Properties</span></span>

| <span data-ttu-id="459a6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="459a6-107">Property</span></span>                           | <span data-ttu-id="459a6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="459a6-108">Type</span></span>                          | <span data-ttu-id="459a6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="459a6-109">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="459a6-110">ендпоинттипе</span><span class="sxs-lookup"><span data-stu-id="459a6-110">endpointType</span></span>                       | <span data-ttu-id="459a6-111">String</span><span class="sxs-lookup"><span data-stu-id="459a6-111">String</span></span>                        | <span data-ttu-id="459a6-112">Тип конечной точки.</span><span class="sxs-lookup"><span data-stu-id="459a6-112">The type of endpoint.</span></span> <span data-ttu-id="459a6-113">Возможные значения: `default`, `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="459a6-113">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="459a6-114">хищения</span><span class="sxs-lookup"><span data-stu-id="459a6-114">identity</span></span>                           | [<span data-ttu-id="459a6-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="459a6-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="459a6-116">[Удостоверение](identityset.md) , связанное с этим приглашением.</span><span class="sxs-lookup"><span data-stu-id="459a6-116">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="459a6-117">реплацескаллид</span><span class="sxs-lookup"><span data-stu-id="459a6-117">replacesCallId</span></span>                     | <span data-ttu-id="459a6-118">String</span><span class="sxs-lookup"><span data-stu-id="459a6-118">String</span></span>                        | <span data-ttu-id="459a6-119">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="459a6-119">Optional.</span></span> <span data-ttu-id="459a6-120">Вызов, частью которого в данный момент является целевой иденити.</span><span class="sxs-lookup"><span data-stu-id="459a6-120">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="459a6-121">Этот вызов будет сброшен после добавления участника.</span><span class="sxs-lookup"><span data-stu-id="459a6-121">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="459a6-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="459a6-122">JSON representation</span></span>

<span data-ttu-id="459a6-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="459a6-123">The following is a JSON representation of the resource.</span></span>

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
