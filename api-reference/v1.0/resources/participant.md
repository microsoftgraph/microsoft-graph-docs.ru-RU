---
title: Тип ресурса участника
description: Представляет тип участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0c5004ea45cf44818c30ffe02dc48a1f6851e64a
ms.sourcegitcommit: d12bd5435c198bcd096e1f7f6a2716f4a04631cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2020
ms.locfileid: "48137120"
---
# <a name="participant-resource-type"></a><span data-ttu-id="3c91c-103">Тип ресурса участника</span><span class="sxs-lookup"><span data-stu-id="3c91c-103">participant resource type</span></span>

<span data-ttu-id="3c91c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c91c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3c91c-105">Представляет участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="3c91c-105">Represents a participant in a call.</span></span>

## <a name="methods"></a><span data-ttu-id="3c91c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3c91c-106">Methods</span></span>

| <span data-ttu-id="3c91c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3c91c-107">Method</span></span>                                                 | <span data-ttu-id="3c91c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3c91c-108">Return Type</span></span>                                                 | <span data-ttu-id="3c91c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3c91c-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="3c91c-110">Участник списка</span><span class="sxs-lookup"><span data-stu-id="3c91c-110">List participant</span></span>](../api/participant-get.md)          | [<span data-ttu-id="3c91c-111">participant</span><span class="sxs-lookup"><span data-stu-id="3c91c-111">participant</span></span>](participant.md)                               | <span data-ttu-id="3c91c-112">Получение списка объектов **участников** в вызове.</span><span class="sxs-lookup"><span data-stu-id="3c91c-112">Retrieve a list of **participant** objects in the call.</span></span> |
| [<span data-ttu-id="3c91c-113">Получение участника</span><span class="sxs-lookup"><span data-stu-id="3c91c-113">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="3c91c-114">participant</span><span class="sxs-lookup"><span data-stu-id="3c91c-114">participant</span></span>](participant.md)                               | <span data-ttu-id="3c91c-115">Чтение свойств объекта **участника** .</span><span class="sxs-lookup"><span data-stu-id="3c91c-115">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="3c91c-116">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="3c91c-116">Delete participant</span></span>](../api/participant-delete.md)         | <span data-ttu-id="3c91c-117">Нет</span><span class="sxs-lookup"><span data-stu-id="3c91c-117">None</span></span>   | <span data-ttu-id="3c91c-118">Удаление участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="3c91c-118">Delete a participant in a call.</span></span>                  |
| [<span data-ttu-id="3c91c-119">Приглашение</span><span class="sxs-lookup"><span data-stu-id="3c91c-119">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="3c91c-120">инвитепартиЦипантсоператион</span><span class="sxs-lookup"><span data-stu-id="3c91c-120">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                        | <span data-ttu-id="3c91c-121">Приглашение участника на звонок.</span><span class="sxs-lookup"><span data-stu-id="3c91c-121">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="3c91c-122">Отключение звука участника</span><span class="sxs-lookup"><span data-stu-id="3c91c-122">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="3c91c-123">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="3c91c-123">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="3c91c-124">Отключение выключения участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="3c91c-124">Mute a participant in a call.</span></span>                  |

## <a name="properties"></a><span data-ttu-id="3c91c-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c91c-125">Properties</span></span>

| <span data-ttu-id="3c91c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c91c-126">Property</span></span>             | <span data-ttu-id="3c91c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="3c91c-127">Type</span></span>                                     | <span data-ttu-id="3c91c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="3c91c-128">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="3c91c-129">id</span><span class="sxs-lookup"><span data-stu-id="3c91c-129">id</span></span>                   | <span data-ttu-id="3c91c-130">Строка</span><span class="sxs-lookup"><span data-stu-id="3c91c-130">String</span></span>                                   | <span data-ttu-id="3c91c-131">Идентификатор участника.</span><span class="sxs-lookup"><span data-stu-id="3c91c-131">The participant ID.</span></span>                                          |
| <span data-ttu-id="3c91c-132">info</span><span class="sxs-lookup"><span data-stu-id="3c91c-132">info</span></span>                 | [<span data-ttu-id="3c91c-133">participantInfo</span><span class="sxs-lookup"><span data-stu-id="3c91c-133">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="3c91c-134">Участник участника.</span><span class="sxs-lookup"><span data-stu-id="3c91c-134">The participant of the participant.</span></span>                          |
| <span data-ttu-id="3c91c-135">исинлобби</span><span class="sxs-lookup"><span data-stu-id="3c91c-135">isInLobby</span></span>            | <span data-ttu-id="3c91c-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c91c-136">Boolean</span></span>                                  | <span data-ttu-id="3c91c-137">`true` Если участник находится в "зале ожидания".</span><span class="sxs-lookup"><span data-stu-id="3c91c-137">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="3c91c-138">Автозвук</span><span class="sxs-lookup"><span data-stu-id="3c91c-138">isMuted</span></span>              | <span data-ttu-id="3c91c-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c91c-139">Boolean</span></span>                                  | <span data-ttu-id="3c91c-140">`true` Если участник отключен (клиент или сервер выключен).</span><span class="sxs-lookup"><span data-stu-id="3c91c-140">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="3c91c-141">медиастреамс</span><span class="sxs-lookup"><span data-stu-id="3c91c-141">mediaStreams</span></span>         | <span data-ttu-id="3c91c-142">Коллекция [медиастреам](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="3c91c-142">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="3c91c-143">Список потоков мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="3c91c-143">The list of media streams.</span></span>                                   |
| <span data-ttu-id="3c91c-144">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="3c91c-144">recordingInfo</span></span>        | [<span data-ttu-id="3c91c-145">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="3c91c-145">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="3c91c-146">Сведения о том, имеет ли участник возможность записи.</span><span class="sxs-lookup"><span data-stu-id="3c91c-146">Information about whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3c91c-147">Связи</span><span class="sxs-lookup"><span data-stu-id="3c91c-147">Relationships</span></span>
<span data-ttu-id="3c91c-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3c91c-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c91c-149">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3c91c-149">JSON representation</span></span>

<span data-ttu-id="3c91c-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c91c-150">The following is a JSON representation of the resource.</span></span>

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

