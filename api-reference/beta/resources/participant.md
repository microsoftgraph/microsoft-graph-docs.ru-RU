---
title: Тип участника ресурса
description: Тип участника.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f49526824b2b6c4eb4a5065f05ab4c765d299faa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508148"
---
# <a name="participant-resource-type"></a><span data-ttu-id="9610f-103">Тип участника ресурса</span><span class="sxs-lookup"><span data-stu-id="9610f-103">participant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9610f-104">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="9610f-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="9610f-105">Методы</span><span class="sxs-lookup"><span data-stu-id="9610f-105">Methods</span></span>

| <span data-ttu-id="9610f-106">Метод</span><span class="sxs-lookup"><span data-stu-id="9610f-106">Method</span></span>                                                          | <span data-ttu-id="9610f-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9610f-107">Return Type</span></span>                              | <span data-ttu-id="9610f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9610f-108">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="9610f-109">Получение участников</span><span class="sxs-lookup"><span data-stu-id="9610f-109">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="9610f-110">Участник</span><span class="sxs-lookup"><span data-stu-id="9610f-110">participant</span></span>](participant.md)            | <span data-ttu-id="9610f-111">Чтение свойств объекта **участника** .</span><span class="sxs-lookup"><span data-stu-id="9610f-111">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="9610f-112">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="9610f-112">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="9610f-113">commsOperation</span><span class="sxs-lookup"><span data-stu-id="9610f-113">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="9610f-114">Настройка участников аудиомикшеру.</span><span class="sxs-lookup"><span data-stu-id="9610f-114">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="9610f-115">Приглашение</span><span class="sxs-lookup"><span data-stu-id="9610f-115">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="9610f-116">commsOperation</span><span class="sxs-lookup"><span data-stu-id="9610f-116">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="9610f-117">Приглашение участников к звонку.</span><span class="sxs-lookup"><span data-stu-id="9610f-117">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="9610f-118">Отключить участников</span><span class="sxs-lookup"><span data-stu-id="9610f-118">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="9610f-119">commsOperation</span><span class="sxs-lookup"><span data-stu-id="9610f-119">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="9610f-120">Отключение микрофона участника в ходе вызова.</span><span class="sxs-lookup"><span data-stu-id="9610f-120">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="9610f-121">Отключение всех участников</span><span class="sxs-lookup"><span data-stu-id="9610f-121">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="9610f-122">commsOperation</span><span class="sxs-lookup"><span data-stu-id="9610f-122">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="9610f-123">Отключение всех участников собрания.</span><span class="sxs-lookup"><span data-stu-id="9610f-123">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="9610f-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="9610f-124">Properties</span></span>

| <span data-ttu-id="9610f-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="9610f-125">Property</span></span>             | <span data-ttu-id="9610f-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9610f-126">Type</span></span>                                     | <span data-ttu-id="9610f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9610f-127">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="9610f-128">id</span><span class="sxs-lookup"><span data-stu-id="9610f-128">id</span></span>                   | <span data-ttu-id="9610f-129">String</span><span class="sxs-lookup"><span data-stu-id="9610f-129">String</span></span>                                   | <span data-ttu-id="9610f-130">Код участника.</span><span class="sxs-lookup"><span data-stu-id="9610f-130">The participant id.</span></span>                                          |
| <span data-ttu-id="9610f-131">сведения о</span><span class="sxs-lookup"><span data-stu-id="9610f-131">info</span></span>                 | [<span data-ttu-id="9610f-132">participantInfo</span><span class="sxs-lookup"><span data-stu-id="9610f-132">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="9610f-133">Участник участника.</span><span class="sxs-lookup"><span data-stu-id="9610f-133">The participant of the participant.</span></span>                          |
| <span data-ttu-id="9610f-134">isInLobby</span><span class="sxs-lookup"><span data-stu-id="9610f-134">isInLobby</span></span>            | <span data-ttu-id="9610f-135">boolean</span><span class="sxs-lookup"><span data-stu-id="9610f-135">boolean</span></span>                                  | <span data-ttu-id="9610f-136">значение true, если участник в зале ожидания</span><span class="sxs-lookup"><span data-stu-id="9610f-136">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="9610f-137">isMuted</span><span class="sxs-lookup"><span data-stu-id="9610f-137">isMuted</span></span>              | <span data-ttu-id="9610f-138">boolean</span><span class="sxs-lookup"><span data-stu-id="9610f-138">boolean</span></span>                                  | <span data-ttu-id="9610f-139">значение true, если выключен ли участника (клиент или сервер выключен ли)</span><span class="sxs-lookup"><span data-stu-id="9610f-139">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="9610f-140">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="9610f-140">mediaStreams</span></span>         | <span data-ttu-id="9610f-141">[mediaStream](mediastream.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9610f-141">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="9610f-142">Список мультимедийных потоков.</span><span class="sxs-lookup"><span data-stu-id="9610f-142">The list of media streams.</span></span>                                   |
| <span data-ttu-id="9610f-143">Метаданные</span><span class="sxs-lookup"><span data-stu-id="9610f-143">metadata</span></span>             | <span data-ttu-id="9610f-144">String</span><span class="sxs-lookup"><span data-stu-id="9610f-144">String</span></span>                                   | <span data-ttu-id="9610f-145">Большой двоичный объект данных, предоставленных участника в списке</span><span class="sxs-lookup"><span data-stu-id="9610f-145">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="9610f-146">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="9610f-146">recordingInfo</span></span>        | [<span data-ttu-id="9610f-147">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="9610f-147">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="9610f-148">Сведения о ли участник имеет возможность записи.</span><span class="sxs-lookup"><span data-stu-id="9610f-148">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9610f-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="9610f-149">Relationships</span></span>
<span data-ttu-id="9610f-150">Нет</span><span class="sxs-lookup"><span data-stu-id="9610f-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9610f-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9610f-151">JSON representation</span></span>

<span data-ttu-id="9610f-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9610f-152">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="9610f-153">Пример</span><span class="sxs-lookup"><span data-stu-id="9610f-153">Example</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/participant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
