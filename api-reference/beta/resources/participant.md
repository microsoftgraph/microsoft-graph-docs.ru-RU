---
title: Тип ресурса участника
description: Тип участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 7598171b4d706a639a11d425ffa409e25126dcf8
ms.sourcegitcommit: d12bd5435c198bcd096e1f7f6a2716f4a04631cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2020
ms.locfileid: "48137150"
---
# <a name="participant-resource-type"></a><span data-ttu-id="74ec9-103">Тип ресурса участника</span><span class="sxs-lookup"><span data-stu-id="74ec9-103">participant resource type</span></span>

<span data-ttu-id="74ec9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74ec9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74ec9-105">Представляет участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="74ec9-105">Represents a participant in a call.</span></span>

## <a name="methods"></a><span data-ttu-id="74ec9-106">Методы</span><span class="sxs-lookup"><span data-stu-id="74ec9-106">Methods</span></span>

| <span data-ttu-id="74ec9-107">Метод</span><span class="sxs-lookup"><span data-stu-id="74ec9-107">Method</span></span>                                                 | <span data-ttu-id="74ec9-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="74ec9-108">Return Type</span></span>                                                 | <span data-ttu-id="74ec9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="74ec9-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="74ec9-110">Участник списка</span><span class="sxs-lookup"><span data-stu-id="74ec9-110">List participant</span></span>](../api/participant-get.md)         | [<span data-ttu-id="74ec9-111">participant</span><span class="sxs-lookup"><span data-stu-id="74ec9-111">participant</span></span>](participant.md)                               | <span data-ttu-id="74ec9-112">Получение списка объектов **участников** в вызове.</span><span class="sxs-lookup"><span data-stu-id="74ec9-112">Retrieve a list of **participant** objects in the call.</span></span> |
| [<span data-ttu-id="74ec9-113">Получение участника</span><span class="sxs-lookup"><span data-stu-id="74ec9-113">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="74ec9-114">participant</span><span class="sxs-lookup"><span data-stu-id="74ec9-114">participant</span></span>](participant.md)                               | <span data-ttu-id="74ec9-115">Чтение свойств объекта **участника** .</span><span class="sxs-lookup"><span data-stu-id="74ec9-115">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="74ec9-116">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="74ec9-116">Delete participant</span></span>](../api/participant-delete.md)     | <span data-ttu-id="74ec9-117">Нет</span><span class="sxs-lookup"><span data-stu-id="74ec9-117">None</span></span>   | <span data-ttu-id="74ec9-118">Удаление участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="74ec9-118">Delete a participant in a call.</span></span>                  |
| [<span data-ttu-id="74ec9-119">конфигуремиксер</span><span class="sxs-lookup"><span data-stu-id="74ec9-119">ConfigureMixer</span></span>](../api/participant-configuremixer.md) | [<span data-ttu-id="74ec9-120">commsOperation</span><span class="sxs-lookup"><span data-stu-id="74ec9-120">commsOperation</span></span>](commsoperation.md)                         | <span data-ttu-id="74ec9-121">Настройка микшера звука участника.</span><span class="sxs-lookup"><span data-stu-id="74ec9-121">Configure the participant audio mixer.</span></span>         |
| [<span data-ttu-id="74ec9-122">Приглашение</span><span class="sxs-lookup"><span data-stu-id="74ec9-122">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="74ec9-123">инвитепартиЦипантсоператион</span><span class="sxs-lookup"><span data-stu-id="74ec9-123">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                         | <span data-ttu-id="74ec9-124">Приглашение участника на звонок.</span><span class="sxs-lookup"><span data-stu-id="74ec9-124">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="74ec9-125">Отключение звука участника</span><span class="sxs-lookup"><span data-stu-id="74ec9-125">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="74ec9-126">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="74ec9-126">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="74ec9-127">Отключение выключения участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="74ec9-127">Mute a participant in a call.</span></span>                  |
| [<span data-ttu-id="74ec9-128">Отключение звука всех участников</span><span class="sxs-lookup"><span data-stu-id="74ec9-128">Mute all participants</span></span>](../api/participant-muteall.md) | [<span data-ttu-id="74ec9-129">commsOperation</span><span class="sxs-lookup"><span data-stu-id="74ec9-129">commsOperation</span></span>](commsoperation.md) | <span data-ttu-id="74ec9-130">Отключение выключения всех участников собрания.</span><span class="sxs-lookup"><span data-stu-id="74ec9-130">Mute all the participants in the meeting.</span></span>      |

## <a name="properties"></a><span data-ttu-id="74ec9-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="74ec9-131">Properties</span></span>

| <span data-ttu-id="74ec9-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="74ec9-132">Property</span></span>             | <span data-ttu-id="74ec9-133">Тип</span><span class="sxs-lookup"><span data-stu-id="74ec9-133">Type</span></span>                                     | <span data-ttu-id="74ec9-134">Описание</span><span class="sxs-lookup"><span data-stu-id="74ec9-134">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="74ec9-135">id</span><span class="sxs-lookup"><span data-stu-id="74ec9-135">id</span></span>                   | <span data-ttu-id="74ec9-136">Строка</span><span class="sxs-lookup"><span data-stu-id="74ec9-136">String</span></span>                                   | <span data-ttu-id="74ec9-137">Идентификатор участника.</span><span class="sxs-lookup"><span data-stu-id="74ec9-137">The participant ID.</span></span>                                          |
| <span data-ttu-id="74ec9-138">info</span><span class="sxs-lookup"><span data-stu-id="74ec9-138">info</span></span>                 | [<span data-ttu-id="74ec9-139">participantInfo</span><span class="sxs-lookup"><span data-stu-id="74ec9-139">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="74ec9-140">Участник участника.</span><span class="sxs-lookup"><span data-stu-id="74ec9-140">The participant of the participant.</span></span>                          |
| <span data-ttu-id="74ec9-141">исинлобби</span><span class="sxs-lookup"><span data-stu-id="74ec9-141">isInLobby</span></span>            | <span data-ttu-id="74ec9-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="74ec9-142">Boolean</span></span>                                  | <span data-ttu-id="74ec9-143">`true` Если участник находится в "зале ожидания".</span><span class="sxs-lookup"><span data-stu-id="74ec9-143">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="74ec9-144">Автозвук</span><span class="sxs-lookup"><span data-stu-id="74ec9-144">isMuted</span></span>              | <span data-ttu-id="74ec9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="74ec9-145">Boolean</span></span>                                  | <span data-ttu-id="74ec9-146">`true` Если участник отключен (клиент или сервер выключен).</span><span class="sxs-lookup"><span data-stu-id="74ec9-146">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="74ec9-147">медиастреамс</span><span class="sxs-lookup"><span data-stu-id="74ec9-147">mediaStreams</span></span>         | <span data-ttu-id="74ec9-148">Коллекция [медиастреам](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="74ec9-148">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="74ec9-149">Список потоков мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="74ec9-149">The list of media streams.</span></span>                                   |
| <span data-ttu-id="74ec9-150">метаданных</span><span class="sxs-lookup"><span data-stu-id="74ec9-150">metadata</span></span>             | <span data-ttu-id="74ec9-151">Строка</span><span class="sxs-lookup"><span data-stu-id="74ec9-151">String</span></span>                                   | <span data-ttu-id="74ec9-152">Большой двоичный объект данных, предоставляемый участником в списке.</span><span class="sxs-lookup"><span data-stu-id="74ec9-152">A blob of data provided by the participant in the roster.</span></span>     |
| <span data-ttu-id="74ec9-153">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="74ec9-153">recordingInfo</span></span>        | [<span data-ttu-id="74ec9-154">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="74ec9-154">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="74ec9-155">Сведения о том, имеет ли участник возможность записи.</span><span class="sxs-lookup"><span data-stu-id="74ec9-155">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="74ec9-156">Связи</span><span class="sxs-lookup"><span data-stu-id="74ec9-156">Relationships</span></span>
<span data-ttu-id="74ec9-157">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="74ec9-157">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="74ec9-158">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="74ec9-158">JSON representation</span></span>

<span data-ttu-id="74ec9-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74ec9-159">The following is a JSON representation of the resource.</span></span>

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


