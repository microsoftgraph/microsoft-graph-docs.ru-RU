---
title: Тип ресурса участника
description: Тип участника.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4a138267529127562fa9df42d8b20a985939b50e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345021"
---
# <a name="participant-resource-type"></a><span data-ttu-id="463eb-103">Тип ресурса участника</span><span class="sxs-lookup"><span data-stu-id="463eb-103">participant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="463eb-104">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="463eb-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="463eb-105">Методы</span><span class="sxs-lookup"><span data-stu-id="463eb-105">Methods</span></span>

| <span data-ttu-id="463eb-106">Метод</span><span class="sxs-lookup"><span data-stu-id="463eb-106">Method</span></span>                                                          | <span data-ttu-id="463eb-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="463eb-107">Return Type</span></span>                              | <span data-ttu-id="463eb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="463eb-108">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="463eb-109">Получение участника</span><span class="sxs-lookup"><span data-stu-id="463eb-109">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="463eb-110">абонент</span><span class="sxs-lookup"><span data-stu-id="463eb-110">participant</span></span>](participant.md)            | <span data-ttu-id="463eb-111">Чтение свойств объекта **участника** .</span><span class="sxs-lookup"><span data-stu-id="463eb-111">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="463eb-112">Конфигуремиксер</span><span class="sxs-lookup"><span data-stu-id="463eb-112">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="463eb-113">commsOperation</span><span class="sxs-lookup"><span data-stu-id="463eb-113">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="463eb-114">Настройка микшера звука участника.</span><span class="sxs-lookup"><span data-stu-id="463eb-114">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="463eb-115">Приглашение</span><span class="sxs-lookup"><span data-stu-id="463eb-115">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="463eb-116">commsOperation</span><span class="sxs-lookup"><span data-stu-id="463eb-116">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="463eb-117">Приглашение участника на звонок.</span><span class="sxs-lookup"><span data-stu-id="463eb-117">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="463eb-118">Отключение звука для участника</span><span class="sxs-lookup"><span data-stu-id="463eb-118">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="463eb-119">commsOperation</span><span class="sxs-lookup"><span data-stu-id="463eb-119">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="463eb-120">Отключение выключения участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="463eb-120">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="463eb-121">Отключение выключения всех участников</span><span class="sxs-lookup"><span data-stu-id="463eb-121">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="463eb-122">commsOperation</span><span class="sxs-lookup"><span data-stu-id="463eb-122">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="463eb-123">Отключение выключения всех участников собрания.</span><span class="sxs-lookup"><span data-stu-id="463eb-123">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="463eb-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="463eb-124">Properties</span></span>

| <span data-ttu-id="463eb-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="463eb-125">Property</span></span>             | <span data-ttu-id="463eb-126">Тип</span><span class="sxs-lookup"><span data-stu-id="463eb-126">Type</span></span>                                     | <span data-ttu-id="463eb-127">Описание</span><span class="sxs-lookup"><span data-stu-id="463eb-127">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="463eb-128">id</span><span class="sxs-lookup"><span data-stu-id="463eb-128">id</span></span>                   | <span data-ttu-id="463eb-129">String</span><span class="sxs-lookup"><span data-stu-id="463eb-129">String</span></span>                                   | <span data-ttu-id="463eb-130">Идентификатор участника.</span><span class="sxs-lookup"><span data-stu-id="463eb-130">The participant id.</span></span>                                          |
| <span data-ttu-id="463eb-131">info</span><span class="sxs-lookup"><span data-stu-id="463eb-131">info</span></span>                 | [<span data-ttu-id="463eb-132">participantInfo</span><span class="sxs-lookup"><span data-stu-id="463eb-132">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="463eb-133">Участник участника.</span><span class="sxs-lookup"><span data-stu-id="463eb-133">The participant of the participant.</span></span>                          |
| <span data-ttu-id="463eb-134">Исинлобби</span><span class="sxs-lookup"><span data-stu-id="463eb-134">isInLobby</span></span>            | <span data-ttu-id="463eb-135">boolean</span><span class="sxs-lookup"><span data-stu-id="463eb-135">boolean</span></span>                                  | <span data-ttu-id="463eb-136">true, если участник находится в зале ожидания</span><span class="sxs-lookup"><span data-stu-id="463eb-136">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="463eb-137">автоЗвук</span><span class="sxs-lookup"><span data-stu-id="463eb-137">isMuted</span></span>              | <span data-ttu-id="463eb-138">boolean</span><span class="sxs-lookup"><span data-stu-id="463eb-138">boolean</span></span>                                  | <span data-ttu-id="463eb-139">true, если участник отключен (клиент или сервер выключен)</span><span class="sxs-lookup"><span data-stu-id="463eb-139">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="463eb-140">Медиастреамс</span><span class="sxs-lookup"><span data-stu-id="463eb-140">mediaStreams</span></span>         | <span data-ttu-id="463eb-141">Коллекция [медиастреам](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="463eb-141">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="463eb-142">Список потоков мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="463eb-142">The list of media streams.</span></span>                                   |
| <span data-ttu-id="463eb-143">метаданных</span><span class="sxs-lookup"><span data-stu-id="463eb-143">metadata</span></span>             | <span data-ttu-id="463eb-144">String</span><span class="sxs-lookup"><span data-stu-id="463eb-144">String</span></span>                                   | <span data-ttu-id="463eb-145">Большой двоичный объект данных, предоставляемый участником в списке</span><span class="sxs-lookup"><span data-stu-id="463eb-145">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="463eb-146">Рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="463eb-146">recordingInfo</span></span>        | [<span data-ttu-id="463eb-147">Рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="463eb-147">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="463eb-148">Сведения о том, имеет ли участник возможность записи.</span><span class="sxs-lookup"><span data-stu-id="463eb-148">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="463eb-149">Связи</span><span class="sxs-lookup"><span data-stu-id="463eb-149">Relationships</span></span>
<span data-ttu-id="463eb-150">Нет</span><span class="sxs-lookup"><span data-stu-id="463eb-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="463eb-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="463eb-151">JSON representation</span></span>

<span data-ttu-id="463eb-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="463eb-152">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="463eb-153">Пример</span><span class="sxs-lookup"><span data-stu-id="463eb-153">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "info": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-US",
    "region": "westus"
  },
  "isInLobby": false,
  "isMuted": false,
  "mediaStreams": [
    {
      "sourceId": "1",
      "direction": "sendReceive",
      "label": "main-audio",
      "mediaType": "audio",
      "serverMuted": false
    }
  ],
  "metadata": "metadata-value",
  "recordingInfo": {
    "status": "recordingCapable"
  }
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
