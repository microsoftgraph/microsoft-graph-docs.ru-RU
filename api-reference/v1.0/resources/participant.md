---
title: Тип ресурса участника
description: Тип участника.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f20bd68cbd4669c002edb37c2ab5fb0a7340dba4
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866260"
---
# <a name="participant-resource-type"></a><span data-ttu-id="df0db-103">Тип ресурса участника</span><span class="sxs-lookup"><span data-stu-id="df0db-103">participant resource type</span></span>

<span data-ttu-id="df0db-104">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="df0db-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="df0db-105">Методы</span><span class="sxs-lookup"><span data-stu-id="df0db-105">Methods</span></span>

| <span data-ttu-id="df0db-106">Метод</span><span class="sxs-lookup"><span data-stu-id="df0db-106">Method</span></span>                                                 | <span data-ttu-id="df0db-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="df0db-107">Return Type</span></span>                                                 | <span data-ttu-id="df0db-108">Описание</span><span class="sxs-lookup"><span data-stu-id="df0db-108">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="df0db-109">Получение участника</span><span class="sxs-lookup"><span data-stu-id="df0db-109">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="df0db-110">participant</span><span class="sxs-lookup"><span data-stu-id="df0db-110">participant</span></span>](participant.md)                               | <span data-ttu-id="df0db-111">Чтение свойств объекта **участника** .</span><span class="sxs-lookup"><span data-stu-id="df0db-111">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="df0db-112">Приглашение</span><span class="sxs-lookup"><span data-stu-id="df0db-112">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="df0db-113">инвитепартиЦипантсоператион</span><span class="sxs-lookup"><span data-stu-id="df0db-113">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                        | <span data-ttu-id="df0db-114">Приглашение участника на звонок.</span><span class="sxs-lookup"><span data-stu-id="df0db-114">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="df0db-115">Отключение звука участника</span><span class="sxs-lookup"><span data-stu-id="df0db-115">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="df0db-116">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="df0db-116">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="df0db-117">Отключение выключения участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="df0db-117">Mute a participant in a call.</span></span>                  |

## <a name="properties"></a><span data-ttu-id="df0db-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="df0db-118">Properties</span></span>

| <span data-ttu-id="df0db-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="df0db-119">Property</span></span>             | <span data-ttu-id="df0db-120">Тип</span><span class="sxs-lookup"><span data-stu-id="df0db-120">Type</span></span>                                     | <span data-ttu-id="df0db-121">Описание</span><span class="sxs-lookup"><span data-stu-id="df0db-121">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="df0db-122">id</span><span class="sxs-lookup"><span data-stu-id="df0db-122">id</span></span>                   | <span data-ttu-id="df0db-123">String</span><span class="sxs-lookup"><span data-stu-id="df0db-123">String</span></span>                                   | <span data-ttu-id="df0db-124">Идентификатор участника.</span><span class="sxs-lookup"><span data-stu-id="df0db-124">The participant ID.</span></span>                                          |
| <span data-ttu-id="df0db-125">info</span><span class="sxs-lookup"><span data-stu-id="df0db-125">info</span></span>                 | [<span data-ttu-id="df0db-126">participantInfo</span><span class="sxs-lookup"><span data-stu-id="df0db-126">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="df0db-127">Участник участника.</span><span class="sxs-lookup"><span data-stu-id="df0db-127">The participant of the participant.</span></span>                          |
| <span data-ttu-id="df0db-128">исинлобби</span><span class="sxs-lookup"><span data-stu-id="df0db-128">isInLobby</span></span>            | <span data-ttu-id="df0db-129">Логический</span><span class="sxs-lookup"><span data-stu-id="df0db-129">Boolean</span></span>                                  | <span data-ttu-id="df0db-130">`true`Если участник находится в "зале ожидания".</span><span class="sxs-lookup"><span data-stu-id="df0db-130">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="df0db-131">Автозвук</span><span class="sxs-lookup"><span data-stu-id="df0db-131">isMuted</span></span>              | <span data-ttu-id="df0db-132">Логический</span><span class="sxs-lookup"><span data-stu-id="df0db-132">Boolean</span></span>                                  | <span data-ttu-id="df0db-133">`true`Если участник отключен (клиент или сервер выключен).</span><span class="sxs-lookup"><span data-stu-id="df0db-133">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="df0db-134">медиастреамс</span><span class="sxs-lookup"><span data-stu-id="df0db-134">mediaStreams</span></span>         | <span data-ttu-id="df0db-135">Коллекция [медиастреам](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="df0db-135">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="df0db-136">Список потоков мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="df0db-136">The list of media streams.</span></span>                                   |

## <a name="relationships"></a><span data-ttu-id="df0db-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="df0db-137">Relationships</span></span>
<span data-ttu-id="df0db-138">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="df0db-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="df0db-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="df0db-139">JSON representation</span></span>

<span data-ttu-id="df0db-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df0db-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "String (identifier)",
  "info": {"@odata.type": "#microsoft.graph.participantInfo"},
  "isInLobby": true,
  "isMuted": true,
  "mediaStreams": [ { "@odata.type": "#microsoft.graph.mediaStream" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
