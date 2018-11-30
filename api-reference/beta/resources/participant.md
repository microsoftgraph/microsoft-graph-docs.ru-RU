---
title: Тип участника ресурса
description: Тип участника.
ms.openlocfilehash: dcb456df0c7269bab91dcf593e674307db5358b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079310"
---
# <a name="participant-resource-type"></a><span data-ttu-id="e585e-103">Тип участника ресурса</span><span class="sxs-lookup"><span data-stu-id="e585e-103">participant resource type</span></span>

> <span data-ttu-id="e585e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e585e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e585e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e585e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e585e-106">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="e585e-106">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="e585e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e585e-107">Methods</span></span>

| <span data-ttu-id="e585e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e585e-108">Method</span></span>                                                          | <span data-ttu-id="e585e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e585e-109">Return Type</span></span>                              | <span data-ttu-id="e585e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e585e-110">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="e585e-111">Получение участников</span><span class="sxs-lookup"><span data-stu-id="e585e-111">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="e585e-112">Участник</span><span class="sxs-lookup"><span data-stu-id="e585e-112">participant</span></span>](participant.md)            | <span data-ttu-id="e585e-113">Чтение свойств объекта **участника** .</span><span class="sxs-lookup"><span data-stu-id="e585e-113">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="e585e-114">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="e585e-114">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="e585e-115">commsOperation</span><span class="sxs-lookup"><span data-stu-id="e585e-115">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="e585e-116">Настройка участников аудиомикшеру.</span><span class="sxs-lookup"><span data-stu-id="e585e-116">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="e585e-117">Приглашение</span><span class="sxs-lookup"><span data-stu-id="e585e-117">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="e585e-118">commsOperation</span><span class="sxs-lookup"><span data-stu-id="e585e-118">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="e585e-119">Приглашение участников к звонку.</span><span class="sxs-lookup"><span data-stu-id="e585e-119">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="e585e-120">Отключить участников</span><span class="sxs-lookup"><span data-stu-id="e585e-120">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="e585e-121">commsOperation</span><span class="sxs-lookup"><span data-stu-id="e585e-121">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="e585e-122">Отключение микрофона участника в ходе вызова.</span><span class="sxs-lookup"><span data-stu-id="e585e-122">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="e585e-123">Отключение всех участников</span><span class="sxs-lookup"><span data-stu-id="e585e-123">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="e585e-124">commsOperation</span><span class="sxs-lookup"><span data-stu-id="e585e-124">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="e585e-125">Отключение всех участников собрания.</span><span class="sxs-lookup"><span data-stu-id="e585e-125">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="e585e-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="e585e-126">Properties</span></span>

| <span data-ttu-id="e585e-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="e585e-127">Property</span></span>             | <span data-ttu-id="e585e-128">Тип</span><span class="sxs-lookup"><span data-stu-id="e585e-128">Type</span></span>                                     | <span data-ttu-id="e585e-129">Описание</span><span class="sxs-lookup"><span data-stu-id="e585e-129">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="e585e-130">id</span><span class="sxs-lookup"><span data-stu-id="e585e-130">id</span></span>                   | <span data-ttu-id="e585e-131">String</span><span class="sxs-lookup"><span data-stu-id="e585e-131">String</span></span>                                   | <span data-ttu-id="e585e-132">Код участника.</span><span class="sxs-lookup"><span data-stu-id="e585e-132">The participant id.</span></span>                                          |
| <span data-ttu-id="e585e-133">сведения о</span><span class="sxs-lookup"><span data-stu-id="e585e-133">info</span></span>                 | [<span data-ttu-id="e585e-134">participantInfo</span><span class="sxs-lookup"><span data-stu-id="e585e-134">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="e585e-135">Участник участника.</span><span class="sxs-lookup"><span data-stu-id="e585e-135">The participant of the participant.</span></span>                          |
| <span data-ttu-id="e585e-136">isInLobby</span><span class="sxs-lookup"><span data-stu-id="e585e-136">isInLobby</span></span>            | <span data-ttu-id="e585e-137">boolean</span><span class="sxs-lookup"><span data-stu-id="e585e-137">boolean</span></span>                                  | <span data-ttu-id="e585e-138">значение true, если участник в зале ожидания</span><span class="sxs-lookup"><span data-stu-id="e585e-138">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="e585e-139">isMuted</span><span class="sxs-lookup"><span data-stu-id="e585e-139">isMuted</span></span>              | <span data-ttu-id="e585e-140">boolean</span><span class="sxs-lookup"><span data-stu-id="e585e-140">boolean</span></span>                                  | <span data-ttu-id="e585e-141">значение true, если выключен ли участника (клиент или сервер выключен ли)</span><span class="sxs-lookup"><span data-stu-id="e585e-141">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="e585e-142">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="e585e-142">mediaStreams</span></span>         | <span data-ttu-id="e585e-143">[mediaStream](mediastream.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e585e-143">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="e585e-144">Список мультимедийных потоков.</span><span class="sxs-lookup"><span data-stu-id="e585e-144">The list of media streams.</span></span>                                   |
| <span data-ttu-id="e585e-145">метаданные</span><span class="sxs-lookup"><span data-stu-id="e585e-145">metadata</span></span>             | <span data-ttu-id="e585e-146">String</span><span class="sxs-lookup"><span data-stu-id="e585e-146">String</span></span>                                   | <span data-ttu-id="e585e-147">Большой двоичный объект данных, предоставленных участника в списке</span><span class="sxs-lookup"><span data-stu-id="e585e-147">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="e585e-148">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="e585e-148">recordingInfo</span></span>        | [<span data-ttu-id="e585e-149">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="e585e-149">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="e585e-150">Сведения о ли участник имеет возможность записи.</span><span class="sxs-lookup"><span data-stu-id="e585e-150">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e585e-151">Связи</span><span class="sxs-lookup"><span data-stu-id="e585e-151">Relationships</span></span>
<span data-ttu-id="e585e-152">Нет</span><span class="sxs-lookup"><span data-stu-id="e585e-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e585e-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e585e-153">JSON representation</span></span>

<span data-ttu-id="e585e-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e585e-154">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="e585e-155">Пример</span><span class="sxs-lookup"><span data-stu-id="e585e-155">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
