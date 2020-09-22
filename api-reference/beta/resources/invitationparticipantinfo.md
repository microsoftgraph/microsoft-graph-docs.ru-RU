---
title: Тип ресурса ИнвитатионпартиЦипантинфо
description: Представляет объект, приглашенный на вызов группы.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9193ec70a3884ba9bf25e4f1c8c33eb7c77d838f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989040"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="9959a-103">Тип ресурса ИнвитатионпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="9959a-103">invitationParticipantInfo resource type</span></span>

<span data-ttu-id="9959a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9959a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9959a-105">Представляет объект, приглашенный на вызов группы.</span><span class="sxs-lookup"><span data-stu-id="9959a-105">Represents an entity that is being invited to a group call.</span></span> 

## <a name="properties"></a><span data-ttu-id="9959a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9959a-106">Properties</span></span>

| <span data-ttu-id="9959a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9959a-107">Property</span></span>                           | <span data-ttu-id="9959a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9959a-108">Type</span></span>                          | <span data-ttu-id="9959a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9959a-109">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="9959a-110">ендпоинттипе</span><span class="sxs-lookup"><span data-stu-id="9959a-110">endpointType</span></span>                       | <span data-ttu-id="9959a-111">String</span><span class="sxs-lookup"><span data-stu-id="9959a-111">String</span></span>                        | <span data-ttu-id="9959a-112">Тип конечной точки.</span><span class="sxs-lookup"><span data-stu-id="9959a-112">The type of endpoint.</span></span> <span data-ttu-id="9959a-113">Возможные значения: `default`, `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="9959a-113">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="9959a-114">хищения</span><span class="sxs-lookup"><span data-stu-id="9959a-114">identity</span></span>                           | [<span data-ttu-id="9959a-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="9959a-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="9959a-116">[Удостоверение](identityset.md) , связанное с этим приглашением.</span><span class="sxs-lookup"><span data-stu-id="9959a-116">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="9959a-117">реплацескаллид</span><span class="sxs-lookup"><span data-stu-id="9959a-117">replacesCallId</span></span>                     | <span data-ttu-id="9959a-118">String</span><span class="sxs-lookup"><span data-stu-id="9959a-118">String</span></span>                        | <span data-ttu-id="9959a-119">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9959a-119">Optional.</span></span> <span data-ttu-id="9959a-120">Вызов, частью которого в данный момент является целевой иденити.</span><span class="sxs-lookup"><span data-stu-id="9959a-120">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="9959a-121">Этот вызов будет сброшен после добавления участника.</span><span class="sxs-lookup"><span data-stu-id="9959a-121">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9959a-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9959a-122">JSON representation</span></span>

<span data-ttu-id="9959a-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9959a-123">The following is a JSON representation of the resource.</span></span>

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


