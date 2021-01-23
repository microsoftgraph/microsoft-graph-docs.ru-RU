---
title: тип ресурса participant
description: Тип участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dc1038e80566cab0ce37eaa40b4f5c391a625824
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943726"
---
# <a name="participant-resource-type"></a><span data-ttu-id="0c91a-103">тип ресурса participant</span><span class="sxs-lookup"><span data-stu-id="0c91a-103">participant resource type</span></span>

<span data-ttu-id="0c91a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c91a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c91a-105">Представляет участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="0c91a-105">Represents a participant in a call.</span></span>

## <a name="methods"></a><span data-ttu-id="0c91a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="0c91a-106">Methods</span></span>

| <span data-ttu-id="0c91a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="0c91a-107">Method</span></span>                                                 | <span data-ttu-id="0c91a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0c91a-108">Return Type</span></span>                                                 | <span data-ttu-id="0c91a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0c91a-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="0c91a-110">Список участников</span><span class="sxs-lookup"><span data-stu-id="0c91a-110">List participant</span></span>](../api/participant-get.md)         | [<span data-ttu-id="0c91a-111">participant</span><span class="sxs-lookup"><span data-stu-id="0c91a-111">participant</span></span>](participant.md)                               | <span data-ttu-id="0c91a-112">Получить список **объектов-участников** в вызове.</span><span class="sxs-lookup"><span data-stu-id="0c91a-112">Retrieve a list of **participant** objects in the call.</span></span> |
| [<span data-ttu-id="0c91a-113">Получение участника</span><span class="sxs-lookup"><span data-stu-id="0c91a-113">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="0c91a-114">participant</span><span class="sxs-lookup"><span data-stu-id="0c91a-114">participant</span></span>](participant.md)                               | <span data-ttu-id="0c91a-115">Чтение свойств объекта **участника.**</span><span class="sxs-lookup"><span data-stu-id="0c91a-115">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="0c91a-116">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="0c91a-116">Delete participant</span></span>](../api/participant-delete.md)     | <span data-ttu-id="0c91a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="0c91a-117">None</span></span>   | <span data-ttu-id="0c91a-118">Удаление участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="0c91a-118">Delete a participant in a call.</span></span>                  |
| [<span data-ttu-id="0c91a-119">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="0c91a-119">ConfigureMixer</span></span>](../api/participant-configuremixer.md) | [<span data-ttu-id="0c91a-120">commsOperation</span><span class="sxs-lookup"><span data-stu-id="0c91a-120">commsOperation</span></span>](commsoperation.md)                         | <span data-ttu-id="0c91a-121">Настройте аудиомесяк участника.</span><span class="sxs-lookup"><span data-stu-id="0c91a-121">Configure the participant audio mixer.</span></span>         |
| [<span data-ttu-id="0c91a-122">Приглашение</span><span class="sxs-lookup"><span data-stu-id="0c91a-122">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="0c91a-123">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="0c91a-123">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                         | <span data-ttu-id="0c91a-124">Приглашение участника на вызов.</span><span class="sxs-lookup"><span data-stu-id="0c91a-124">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="0c91a-125">Отключение звука участника</span><span class="sxs-lookup"><span data-stu-id="0c91a-125">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="0c91a-126">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="0c91a-126">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="0c91a-127">Отключить звук участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="0c91a-127">Mute a participant in a call.</span></span>                  |
| [<span data-ttu-id="0c91a-128">Отключение звука всех участников</span><span class="sxs-lookup"><span data-stu-id="0c91a-128">Mute all participants</span></span>](../api/participant-muteall.md) | [<span data-ttu-id="0c91a-129">commsOperation</span><span class="sxs-lookup"><span data-stu-id="0c91a-129">commsOperation</span></span>](commsoperation.md) | <span data-ttu-id="0c91a-130">Отключить звук всех участников собрания.</span><span class="sxs-lookup"><span data-stu-id="0c91a-130">Mute all the participants in the meeting.</span></span>      |

## <a name="properties"></a><span data-ttu-id="0c91a-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c91a-131">Properties</span></span>

| <span data-ttu-id="0c91a-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c91a-132">Property</span></span>             | <span data-ttu-id="0c91a-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0c91a-133">Type</span></span>                                     | <span data-ttu-id="0c91a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0c91a-134">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="0c91a-135">id</span><span class="sxs-lookup"><span data-stu-id="0c91a-135">id</span></span>                   | <span data-ttu-id="0c91a-136">String</span><span class="sxs-lookup"><span data-stu-id="0c91a-136">String</span></span>                                   | <span data-ttu-id="0c91a-137">ИД участника.</span><span class="sxs-lookup"><span data-stu-id="0c91a-137">The participant ID.</span></span>                                          |
| <span data-ttu-id="0c91a-138">info</span><span class="sxs-lookup"><span data-stu-id="0c91a-138">info</span></span>                 | [<span data-ttu-id="0c91a-139">participantInfo</span><span class="sxs-lookup"><span data-stu-id="0c91a-139">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="0c91a-140">Сведения об участнике.</span><span class="sxs-lookup"><span data-stu-id="0c91a-140">Information about the participant.</span></span>                          |
| <span data-ttu-id="0c91a-141">isInLobby</span><span class="sxs-lookup"><span data-stu-id="0c91a-141">isInLobby</span></span>            | <span data-ttu-id="0c91a-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c91a-142">Boolean</span></span>                                  | <span data-ttu-id="0c91a-143">`true` если участник находится в "окле".</span><span class="sxs-lookup"><span data-stu-id="0c91a-143">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="0c91a-144">isMuted</span><span class="sxs-lookup"><span data-stu-id="0c91a-144">isMuted</span></span>              | <span data-ttu-id="0c91a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c91a-145">Boolean</span></span>                                  | <span data-ttu-id="0c91a-146">`true` если участник отключен (клиент или сервер отключен).</span><span class="sxs-lookup"><span data-stu-id="0c91a-146">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="0c91a-147">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="0c91a-147">mediaStreams</span></span>         | <span data-ttu-id="0c91a-148">[Коллекция mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="0c91a-148">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="0c91a-149">Список потоков мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="0c91a-149">The list of media streams.</span></span>                                   |
| <span data-ttu-id="0c91a-150">метаданные</span><span class="sxs-lookup"><span data-stu-id="0c91a-150">metadata</span></span>             | <span data-ttu-id="0c91a-151">String</span><span class="sxs-lookup"><span data-stu-id="0c91a-151">String</span></span>                                   | <span data-ttu-id="0c91a-152">Большой объем данных, предоставленный участником в составе.</span><span class="sxs-lookup"><span data-stu-id="0c91a-152">A blob of data provided by the participant in the roster.</span></span>     |
| <span data-ttu-id="0c91a-153">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="0c91a-153">recordingInfo</span></span>        | [<span data-ttu-id="0c91a-154">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="0c91a-154">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="0c91a-155">Сведения о том, есть ли у участника возможность записи.</span><span class="sxs-lookup"><span data-stu-id="0c91a-155">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0c91a-156">Связи</span><span class="sxs-lookup"><span data-stu-id="0c91a-156">Relationships</span></span>
<span data-ttu-id="0c91a-157">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0c91a-157">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c91a-158">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0c91a-158">JSON representation</span></span>

<span data-ttu-id="0c91a-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c91a-159">The following is a JSON representation of the resource.</span></span>

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
  "mediaStreams": [ { "@odata.type": "#microsoft.graph.mediaStream" } ],
  "metadata": "String",
  "recordingInfo": { "@odata.type": "#microsoft.graph.recordingInfo" }
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


