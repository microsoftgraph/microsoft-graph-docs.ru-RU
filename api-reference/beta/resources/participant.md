---
title: Тип ресурса участника
description: Тип участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6ae920e35c3ba7c2b31c5947f15b3e9d6585a21c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522041"
---
# <a name="participant-resource-type"></a><span data-ttu-id="0bffc-103">Тип ресурса участника</span><span class="sxs-lookup"><span data-stu-id="0bffc-103">participant resource type</span></span>

<span data-ttu-id="0bffc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0bffc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bffc-105">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="0bffc-105">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="0bffc-106">Методы</span><span class="sxs-lookup"><span data-stu-id="0bffc-106">Methods</span></span>

| <span data-ttu-id="0bffc-107">Метод</span><span class="sxs-lookup"><span data-stu-id="0bffc-107">Method</span></span>                                                 | <span data-ttu-id="0bffc-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0bffc-108">Return Type</span></span>                                                 | <span data-ttu-id="0bffc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0bffc-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="0bffc-110">Получение участника</span><span class="sxs-lookup"><span data-stu-id="0bffc-110">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="0bffc-111">participant</span><span class="sxs-lookup"><span data-stu-id="0bffc-111">participant</span></span>](participant.md)                               | <span data-ttu-id="0bffc-112">Чтение свойств объекта **участника** .</span><span class="sxs-lookup"><span data-stu-id="0bffc-112">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="0bffc-113">конфигуремиксер</span><span class="sxs-lookup"><span data-stu-id="0bffc-113">ConfigureMixer</span></span>](../api/participant-configuremixer.md) | [<span data-ttu-id="0bffc-114">commsOperation</span><span class="sxs-lookup"><span data-stu-id="0bffc-114">commsOperation</span></span>](commsoperation.md)                         | <span data-ttu-id="0bffc-115">Настройка микшера звука участника.</span><span class="sxs-lookup"><span data-stu-id="0bffc-115">Configure the participant audio mixer.</span></span>         |
| [<span data-ttu-id="0bffc-116">Приглашение</span><span class="sxs-lookup"><span data-stu-id="0bffc-116">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="0bffc-117">инвитепартиЦипантсоператион</span><span class="sxs-lookup"><span data-stu-id="0bffc-117">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                         | <span data-ttu-id="0bffc-118">Приглашение участника на звонок.</span><span class="sxs-lookup"><span data-stu-id="0bffc-118">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="0bffc-119">Отключение звука участника</span><span class="sxs-lookup"><span data-stu-id="0bffc-119">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="0bffc-120">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="0bffc-120">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="0bffc-121">Отключение выключения участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="0bffc-121">Mute a participant in a call.</span></span>                  |
| [<span data-ttu-id="0bffc-122">Отключение звука всех участников</span><span class="sxs-lookup"><span data-stu-id="0bffc-122">Mute all participants</span></span>](../api/participant-muteall.md) | [<span data-ttu-id="0bffc-123">commsOperation</span><span class="sxs-lookup"><span data-stu-id="0bffc-123">commsOperation</span></span>](commsoperation.md) | <span data-ttu-id="0bffc-124">Отключение выключения всех участников собрания.</span><span class="sxs-lookup"><span data-stu-id="0bffc-124">Mute all the participants in the meeting.</span></span>      |

## <a name="properties"></a><span data-ttu-id="0bffc-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="0bffc-125">Properties</span></span>

| <span data-ttu-id="0bffc-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="0bffc-126">Property</span></span>             | <span data-ttu-id="0bffc-127">Тип</span><span class="sxs-lookup"><span data-stu-id="0bffc-127">Type</span></span>                                     | <span data-ttu-id="0bffc-128">Описание</span><span class="sxs-lookup"><span data-stu-id="0bffc-128">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="0bffc-129">id</span><span class="sxs-lookup"><span data-stu-id="0bffc-129">id</span></span>                   | <span data-ttu-id="0bffc-130">String</span><span class="sxs-lookup"><span data-stu-id="0bffc-130">String</span></span>                                   | <span data-ttu-id="0bffc-131">Идентификатор участника.</span><span class="sxs-lookup"><span data-stu-id="0bffc-131">The participant ID.</span></span>                                          |
| <span data-ttu-id="0bffc-132">info</span><span class="sxs-lookup"><span data-stu-id="0bffc-132">info</span></span>                 | [<span data-ttu-id="0bffc-133">participantInfo</span><span class="sxs-lookup"><span data-stu-id="0bffc-133">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="0bffc-134">Участник участника.</span><span class="sxs-lookup"><span data-stu-id="0bffc-134">The participant of the participant.</span></span>                          |
| <span data-ttu-id="0bffc-135">исинлобби</span><span class="sxs-lookup"><span data-stu-id="0bffc-135">isInLobby</span></span>            | <span data-ttu-id="0bffc-136">Логический</span><span class="sxs-lookup"><span data-stu-id="0bffc-136">Boolean</span></span>                                  | <span data-ttu-id="0bffc-137">`true`Если участник находится в "зале ожидания".</span><span class="sxs-lookup"><span data-stu-id="0bffc-137">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="0bffc-138">Автозвук</span><span class="sxs-lookup"><span data-stu-id="0bffc-138">isMuted</span></span>              | <span data-ttu-id="0bffc-139">Логический</span><span class="sxs-lookup"><span data-stu-id="0bffc-139">Boolean</span></span>                                  | <span data-ttu-id="0bffc-140">`true`Если участник отключен (клиент или сервер выключен).</span><span class="sxs-lookup"><span data-stu-id="0bffc-140">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="0bffc-141">медиастреамс</span><span class="sxs-lookup"><span data-stu-id="0bffc-141">mediaStreams</span></span>         | <span data-ttu-id="0bffc-142">Коллекция [медиастреам](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="0bffc-142">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="0bffc-143">Список потоков мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="0bffc-143">The list of media streams.</span></span>                                   |
| <span data-ttu-id="0bffc-144">метаданных</span><span class="sxs-lookup"><span data-stu-id="0bffc-144">metadata</span></span>             | <span data-ttu-id="0bffc-145">String</span><span class="sxs-lookup"><span data-stu-id="0bffc-145">String</span></span>                                   | <span data-ttu-id="0bffc-146">Большой двоичный объект данных, предоставляемый участником в списке.</span><span class="sxs-lookup"><span data-stu-id="0bffc-146">A blob of data provided by the participant in the roster.</span></span>     |
| <span data-ttu-id="0bffc-147">рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="0bffc-147">recordingInfo</span></span>        | [<span data-ttu-id="0bffc-148">рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="0bffc-148">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="0bffc-149">Сведения о том, имеет ли участник возможность записи.</span><span class="sxs-lookup"><span data-stu-id="0bffc-149">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0bffc-150">Связи</span><span class="sxs-lookup"><span data-stu-id="0bffc-150">Relationships</span></span>
<span data-ttu-id="0bffc-151">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0bffc-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0bffc-152">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0bffc-152">JSON representation</span></span>

<span data-ttu-id="0bffc-153">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0bffc-153">The following is a JSON representation of the resource.</span></span>

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
