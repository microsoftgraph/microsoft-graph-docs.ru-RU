---
title: Тип ресурса участника
description: Представляет тип участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 82a8cdd51cc7dd8c3be1e06c24ff61b19a9b86ac
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962340"
---
# <a name="participant-resource-type"></a><span data-ttu-id="e3d78-103">Тип ресурса участника</span><span class="sxs-lookup"><span data-stu-id="e3d78-103">participant resource type</span></span>

<span data-ttu-id="e3d78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3d78-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3d78-105">Представляет тип участника.</span><span class="sxs-lookup"><span data-stu-id="e3d78-105">Represents the participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="e3d78-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e3d78-106">Methods</span></span>

| <span data-ttu-id="e3d78-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e3d78-107">Method</span></span>                                                 | <span data-ttu-id="e3d78-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e3d78-108">Return Type</span></span>                                                 | <span data-ttu-id="e3d78-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e3d78-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="e3d78-110">Получение участника</span><span class="sxs-lookup"><span data-stu-id="e3d78-110">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="e3d78-111">participant</span><span class="sxs-lookup"><span data-stu-id="e3d78-111">participant</span></span>](participant.md)                               | <span data-ttu-id="e3d78-112">Чтение свойств объекта **участника** .</span><span class="sxs-lookup"><span data-stu-id="e3d78-112">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="e3d78-113">Приглашение</span><span class="sxs-lookup"><span data-stu-id="e3d78-113">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="e3d78-114">инвитепартиЦипантсоператион</span><span class="sxs-lookup"><span data-stu-id="e3d78-114">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                        | <span data-ttu-id="e3d78-115">Приглашение участника на звонок.</span><span class="sxs-lookup"><span data-stu-id="e3d78-115">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="e3d78-116">Отключение звука участника</span><span class="sxs-lookup"><span data-stu-id="e3d78-116">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="e3d78-117">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="e3d78-117">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="e3d78-118">Отключение выключения участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="e3d78-118">Mute a participant in a call.</span></span>                  |

## <a name="properties"></a><span data-ttu-id="e3d78-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3d78-119">Properties</span></span>

| <span data-ttu-id="e3d78-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3d78-120">Property</span></span>             | <span data-ttu-id="e3d78-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e3d78-121">Type</span></span>                                     | <span data-ttu-id="e3d78-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e3d78-122">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="e3d78-123">id</span><span class="sxs-lookup"><span data-stu-id="e3d78-123">id</span></span>                   | <span data-ttu-id="e3d78-124">String</span><span class="sxs-lookup"><span data-stu-id="e3d78-124">String</span></span>                                   | <span data-ttu-id="e3d78-125">Идентификатор участника.</span><span class="sxs-lookup"><span data-stu-id="e3d78-125">The participant ID.</span></span>                                          |
| <span data-ttu-id="e3d78-126">info</span><span class="sxs-lookup"><span data-stu-id="e3d78-126">info</span></span>                 | [<span data-ttu-id="e3d78-127">participantInfo</span><span class="sxs-lookup"><span data-stu-id="e3d78-127">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="e3d78-128">Участник участника.</span><span class="sxs-lookup"><span data-stu-id="e3d78-128">The participant of the participant.</span></span>                          |
| <span data-ttu-id="e3d78-129">исинлобби</span><span class="sxs-lookup"><span data-stu-id="e3d78-129">isInLobby</span></span>            | <span data-ttu-id="e3d78-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3d78-130">Boolean</span></span>                                  | <span data-ttu-id="e3d78-131">`true`Если участник находится в "зале ожидания".</span><span class="sxs-lookup"><span data-stu-id="e3d78-131">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="e3d78-132">Автозвук</span><span class="sxs-lookup"><span data-stu-id="e3d78-132">isMuted</span></span>              | <span data-ttu-id="e3d78-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3d78-133">Boolean</span></span>                                  | <span data-ttu-id="e3d78-134">`true`Если участник отключен (клиент или сервер выключен).</span><span class="sxs-lookup"><span data-stu-id="e3d78-134">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="e3d78-135">медиастреамс</span><span class="sxs-lookup"><span data-stu-id="e3d78-135">mediaStreams</span></span>         | <span data-ttu-id="e3d78-136">Коллекция [медиастреам](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="e3d78-136">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="e3d78-137">Список потоков мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="e3d78-137">The list of media streams.</span></span>                                   |
| <span data-ttu-id="e3d78-138">рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="e3d78-138">recordingInfo</span></span>        | [<span data-ttu-id="e3d78-139">рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="e3d78-139">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="e3d78-140">Сведения о том, имеет ли участник возможность записи.</span><span class="sxs-lookup"><span data-stu-id="e3d78-140">Information about whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e3d78-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="e3d78-141">Relationships</span></span>
<span data-ttu-id="e3d78-142">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e3d78-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3d78-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e3d78-143">JSON representation</span></span>

<span data-ttu-id="e3d78-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3d78-144">The following is a JSON representation of the resource.</span></span>

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
