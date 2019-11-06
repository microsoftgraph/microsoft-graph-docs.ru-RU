---
title: Тип ресурса участника
description: Тип участника.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e2fae206fb76ffe3c00b91d992c874e200eeae98
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006601"
---
# <a name="participant-resource-type"></a><span data-ttu-id="8e27d-103">Тип ресурса участника</span><span class="sxs-lookup"><span data-stu-id="8e27d-103">participant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e27d-104">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="8e27d-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="8e27d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="8e27d-105">Methods</span></span>

| <span data-ttu-id="8e27d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="8e27d-106">Method</span></span>                                                          | <span data-ttu-id="8e27d-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8e27d-107">Return Type</span></span>                              | <span data-ttu-id="8e27d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8e27d-108">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="8e27d-109">Получение участника</span><span class="sxs-lookup"><span data-stu-id="8e27d-109">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="8e27d-110">participant</span><span class="sxs-lookup"><span data-stu-id="8e27d-110">participant</span></span>](participant.md)            | <span data-ttu-id="8e27d-111">Чтение свойств объекта **участника** .</span><span class="sxs-lookup"><span data-stu-id="8e27d-111">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="8e27d-112">конфигуремиксер</span><span class="sxs-lookup"><span data-stu-id="8e27d-112">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="8e27d-113">commsOperation</span><span class="sxs-lookup"><span data-stu-id="8e27d-113">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="8e27d-114">Настройка микшера звука участника.</span><span class="sxs-lookup"><span data-stu-id="8e27d-114">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="8e27d-115">Приглашение</span><span class="sxs-lookup"><span data-stu-id="8e27d-115">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="8e27d-116">commsOperation</span><span class="sxs-lookup"><span data-stu-id="8e27d-116">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="8e27d-117">Приглашение участника на звонок.</span><span class="sxs-lookup"><span data-stu-id="8e27d-117">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="8e27d-118">Отключение звука участника</span><span class="sxs-lookup"><span data-stu-id="8e27d-118">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="8e27d-119">commsOperation</span><span class="sxs-lookup"><span data-stu-id="8e27d-119">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="8e27d-120">Отключение выключения участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="8e27d-120">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="8e27d-121">Отключение выключения всех участников</span><span class="sxs-lookup"><span data-stu-id="8e27d-121">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="8e27d-122">commsOperation</span><span class="sxs-lookup"><span data-stu-id="8e27d-122">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="8e27d-123">Отключение выключения всех участников собрания.</span><span class="sxs-lookup"><span data-stu-id="8e27d-123">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="8e27d-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e27d-124">Properties</span></span>

| <span data-ttu-id="8e27d-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e27d-125">Property</span></span>             | <span data-ttu-id="8e27d-126">Тип</span><span class="sxs-lookup"><span data-stu-id="8e27d-126">Type</span></span>                                     | <span data-ttu-id="8e27d-127">Описание</span><span class="sxs-lookup"><span data-stu-id="8e27d-127">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="8e27d-128">id</span><span class="sxs-lookup"><span data-stu-id="8e27d-128">id</span></span>                   | <span data-ttu-id="8e27d-129">String</span><span class="sxs-lookup"><span data-stu-id="8e27d-129">String</span></span>                                   | <span data-ttu-id="8e27d-130">Идентификатор участника.</span><span class="sxs-lookup"><span data-stu-id="8e27d-130">The participant id.</span></span>                                          |
| <span data-ttu-id="8e27d-131">info</span><span class="sxs-lookup"><span data-stu-id="8e27d-131">info</span></span>                 | [<span data-ttu-id="8e27d-132">participantInfo</span><span class="sxs-lookup"><span data-stu-id="8e27d-132">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="8e27d-133">Участник участника.</span><span class="sxs-lookup"><span data-stu-id="8e27d-133">The participant of the participant.</span></span>                          |
| <span data-ttu-id="8e27d-134">исинлобби</span><span class="sxs-lookup"><span data-stu-id="8e27d-134">isInLobby</span></span>            | <span data-ttu-id="8e27d-135">boolean</span><span class="sxs-lookup"><span data-stu-id="8e27d-135">boolean</span></span>                                  | <span data-ttu-id="8e27d-136">true, если участник находится в зале ожидания</span><span class="sxs-lookup"><span data-stu-id="8e27d-136">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="8e27d-137">Автозвук</span><span class="sxs-lookup"><span data-stu-id="8e27d-137">isMuted</span></span>              | <span data-ttu-id="8e27d-138">boolean</span><span class="sxs-lookup"><span data-stu-id="8e27d-138">boolean</span></span>                                  | <span data-ttu-id="8e27d-139">true, если участник отключен (клиент или сервер выключен)</span><span class="sxs-lookup"><span data-stu-id="8e27d-139">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="8e27d-140">медиастреамс</span><span class="sxs-lookup"><span data-stu-id="8e27d-140">mediaStreams</span></span>         | <span data-ttu-id="8e27d-141">Коллекция [медиастреам](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="8e27d-141">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="8e27d-142">Список потоков мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="8e27d-142">The list of media streams.</span></span>                                   |
| <span data-ttu-id="8e27d-143">метаданных</span><span class="sxs-lookup"><span data-stu-id="8e27d-143">metadata</span></span>             | <span data-ttu-id="8e27d-144">String</span><span class="sxs-lookup"><span data-stu-id="8e27d-144">String</span></span>                                   | <span data-ttu-id="8e27d-145">Большой двоичный объект данных, предоставляемый участником в списке</span><span class="sxs-lookup"><span data-stu-id="8e27d-145">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="8e27d-146">рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="8e27d-146">recordingInfo</span></span>        | [<span data-ttu-id="8e27d-147">рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="8e27d-147">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="8e27d-148">Сведения о том, имеет ли участник возможность записи.</span><span class="sxs-lookup"><span data-stu-id="8e27d-148">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8e27d-149">Связи</span><span class="sxs-lookup"><span data-stu-id="8e27d-149">Relationships</span></span>
<span data-ttu-id="8e27d-150">Нет</span><span class="sxs-lookup"><span data-stu-id="8e27d-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e27d-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e27d-151">JSON representation</span></span>

<span data-ttu-id="8e27d-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e27d-152">The following is a JSON representation of the resource.</span></span>

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
