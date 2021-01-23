---
title: тип ресурса participant
description: Представляет тип участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 99f165f2f3e99ab424a318b053a060ccda8fdc1c
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943719"
---
# <a name="participant-resource-type"></a><span data-ttu-id="9c0c3-103">тип ресурса participant</span><span class="sxs-lookup"><span data-stu-id="9c0c3-103">participant resource type</span></span>

<span data-ttu-id="9c0c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c0c3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c0c3-105">Представляет участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="9c0c3-105">Represents a participant in a call.</span></span>

## <a name="methods"></a><span data-ttu-id="9c0c3-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9c0c3-106">Methods</span></span>

| <span data-ttu-id="9c0c3-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9c0c3-107">Method</span></span>                                                 | <span data-ttu-id="9c0c3-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9c0c3-108">Return Type</span></span>                                                 | <span data-ttu-id="9c0c3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9c0c3-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="9c0c3-110">Список участников</span><span class="sxs-lookup"><span data-stu-id="9c0c3-110">List participant</span></span>](../api/participant-get.md)          | [<span data-ttu-id="9c0c3-111">participant</span><span class="sxs-lookup"><span data-stu-id="9c0c3-111">participant</span></span>](participant.md)                               | <span data-ttu-id="9c0c3-112">Получить список **объектов-участников** в вызове.</span><span class="sxs-lookup"><span data-stu-id="9c0c3-112">Retrieve a list of **participant** objects in the call.</span></span> |
| [<span data-ttu-id="9c0c3-113">Получение участника</span><span class="sxs-lookup"><span data-stu-id="9c0c3-113">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="9c0c3-114">participant</span><span class="sxs-lookup"><span data-stu-id="9c0c3-114">participant</span></span>](participant.md)                               | <span data-ttu-id="9c0c3-115">Чтение свойств объекта **участника.**</span><span class="sxs-lookup"><span data-stu-id="9c0c3-115">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="9c0c3-116">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="9c0c3-116">Delete participant</span></span>](../api/participant-delete.md)         | <span data-ttu-id="9c0c3-117">Нет</span><span class="sxs-lookup"><span data-stu-id="9c0c3-117">None</span></span>   | <span data-ttu-id="9c0c3-118">Удаление участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="9c0c3-118">Delete a participant in a call.</span></span>                  |
| [<span data-ttu-id="9c0c3-119">Приглашение</span><span class="sxs-lookup"><span data-stu-id="9c0c3-119">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="9c0c3-120">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="9c0c3-120">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                        | <span data-ttu-id="9c0c3-121">Приглашение участника на вызов.</span><span class="sxs-lookup"><span data-stu-id="9c0c3-121">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="9c0c3-122">Отключение звука участника</span><span class="sxs-lookup"><span data-stu-id="9c0c3-122">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="9c0c3-123">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="9c0c3-123">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="9c0c3-124">Отключить звук участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="9c0c3-124">Mute a participant in a call.</span></span>                  |

## <a name="properties"></a><span data-ttu-id="9c0c3-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c0c3-125">Properties</span></span>

| <span data-ttu-id="9c0c3-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c0c3-126">Property</span></span>             | <span data-ttu-id="9c0c3-127">Тип</span><span class="sxs-lookup"><span data-stu-id="9c0c3-127">Type</span></span>                                     | <span data-ttu-id="9c0c3-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9c0c3-128">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="9c0c3-129">id</span><span class="sxs-lookup"><span data-stu-id="9c0c3-129">id</span></span>                   | <span data-ttu-id="9c0c3-130">String</span><span class="sxs-lookup"><span data-stu-id="9c0c3-130">String</span></span>                                   | <span data-ttu-id="9c0c3-131">ИД участника.</span><span class="sxs-lookup"><span data-stu-id="9c0c3-131">The participant ID.</span></span>                                          |
| <span data-ttu-id="9c0c3-132">info</span><span class="sxs-lookup"><span data-stu-id="9c0c3-132">info</span></span>                 | [<span data-ttu-id="9c0c3-133">participantInfo</span><span class="sxs-lookup"><span data-stu-id="9c0c3-133">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="9c0c3-134">Сведения об участнике.</span><span class="sxs-lookup"><span data-stu-id="9c0c3-134">Information about the participant.</span></span>                          |
| <span data-ttu-id="9c0c3-135">isInLobby</span><span class="sxs-lookup"><span data-stu-id="9c0c3-135">isInLobby</span></span>            | <span data-ttu-id="9c0c3-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c0c3-136">Boolean</span></span>                                  | <span data-ttu-id="9c0c3-137">`true` если участник находится в "окле".</span><span class="sxs-lookup"><span data-stu-id="9c0c3-137">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="9c0c3-138">isMuted</span><span class="sxs-lookup"><span data-stu-id="9c0c3-138">isMuted</span></span>              | <span data-ttu-id="9c0c3-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c0c3-139">Boolean</span></span>                                  | <span data-ttu-id="9c0c3-140">`true` если участник отключен (клиент или сервер отключен).</span><span class="sxs-lookup"><span data-stu-id="9c0c3-140">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="9c0c3-141">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="9c0c3-141">mediaStreams</span></span>         | <span data-ttu-id="9c0c3-142">[Коллекция mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="9c0c3-142">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="9c0c3-143">Список потоков мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="9c0c3-143">The list of media streams.</span></span>                                   |
| <span data-ttu-id="9c0c3-144">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="9c0c3-144">recordingInfo</span></span>        | [<span data-ttu-id="9c0c3-145">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="9c0c3-145">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="9c0c3-146">Сведения о том, есть ли у участника возможность записи.</span><span class="sxs-lookup"><span data-stu-id="9c0c3-146">Information about whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9c0c3-147">Связи</span><span class="sxs-lookup"><span data-stu-id="9c0c3-147">Relationships</span></span>
<span data-ttu-id="9c0c3-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9c0c3-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c0c3-149">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9c0c3-149">JSON representation</span></span>

<span data-ttu-id="9c0c3-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c0c3-150">The following is a JSON representation of the resource.</span></span>

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

