---
title: Тип ресурса участника
description: Тип участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e6711a771d0c10112850f2d05943f4e8752ebbdf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534085"
---
# <a name="participant-resource-type"></a><span data-ttu-id="0c435-103">Тип ресурса участника</span><span class="sxs-lookup"><span data-stu-id="0c435-103">participant resource type</span></span>

<span data-ttu-id="0c435-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c435-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0c435-105">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="0c435-105">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="0c435-106">Методы</span><span class="sxs-lookup"><span data-stu-id="0c435-106">Methods</span></span>

| <span data-ttu-id="0c435-107">Метод</span><span class="sxs-lookup"><span data-stu-id="0c435-107">Method</span></span>                                                 | <span data-ttu-id="0c435-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0c435-108">Return Type</span></span>                                                 | <span data-ttu-id="0c435-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0c435-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="0c435-110">Получение участника</span><span class="sxs-lookup"><span data-stu-id="0c435-110">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="0c435-111">participant</span><span class="sxs-lookup"><span data-stu-id="0c435-111">participant</span></span>](participant.md)                               | <span data-ttu-id="0c435-112">Чтение свойств объекта **участника** .</span><span class="sxs-lookup"><span data-stu-id="0c435-112">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="0c435-113">Приглашение</span><span class="sxs-lookup"><span data-stu-id="0c435-113">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="0c435-114">инвитепартиЦипантсоператион</span><span class="sxs-lookup"><span data-stu-id="0c435-114">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                        | <span data-ttu-id="0c435-115">Приглашение участника на звонок.</span><span class="sxs-lookup"><span data-stu-id="0c435-115">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="0c435-116">Отключение звука участника</span><span class="sxs-lookup"><span data-stu-id="0c435-116">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="0c435-117">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="0c435-117">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="0c435-118">Отключение выключения участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="0c435-118">Mute a participant in a call.</span></span>                  |

## <a name="properties"></a><span data-ttu-id="0c435-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c435-119">Properties</span></span>

| <span data-ttu-id="0c435-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c435-120">Property</span></span>             | <span data-ttu-id="0c435-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0c435-121">Type</span></span>                                     | <span data-ttu-id="0c435-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0c435-122">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="0c435-123">id</span><span class="sxs-lookup"><span data-stu-id="0c435-123">id</span></span>                   | <span data-ttu-id="0c435-124">Строка</span><span class="sxs-lookup"><span data-stu-id="0c435-124">String</span></span>                                   | <span data-ttu-id="0c435-125">Идентификатор участника.</span><span class="sxs-lookup"><span data-stu-id="0c435-125">The participant ID.</span></span>                                          |
| <span data-ttu-id="0c435-126">info</span><span class="sxs-lookup"><span data-stu-id="0c435-126">info</span></span>                 | [<span data-ttu-id="0c435-127">participantInfo</span><span class="sxs-lookup"><span data-stu-id="0c435-127">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="0c435-128">Участник участника.</span><span class="sxs-lookup"><span data-stu-id="0c435-128">The participant of the participant.</span></span>                          |
| <span data-ttu-id="0c435-129">исинлобби</span><span class="sxs-lookup"><span data-stu-id="0c435-129">isInLobby</span></span>            | <span data-ttu-id="0c435-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c435-130">Boolean</span></span>                                  | <span data-ttu-id="0c435-131">`true`Если участник находится в "зале ожидания".</span><span class="sxs-lookup"><span data-stu-id="0c435-131">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="0c435-132">Автозвук</span><span class="sxs-lookup"><span data-stu-id="0c435-132">isMuted</span></span>              | <span data-ttu-id="0c435-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c435-133">Boolean</span></span>                                  | <span data-ttu-id="0c435-134">`true`Если участник отключен (клиент или сервер выключен).</span><span class="sxs-lookup"><span data-stu-id="0c435-134">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="0c435-135">медиастреамс</span><span class="sxs-lookup"><span data-stu-id="0c435-135">mediaStreams</span></span>         | <span data-ttu-id="0c435-136">Коллекция [медиастреам](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="0c435-136">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="0c435-137">Список потоков мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="0c435-137">The list of media streams.</span></span>                                   |

## <a name="relationships"></a><span data-ttu-id="0c435-138">Связи</span><span class="sxs-lookup"><span data-stu-id="0c435-138">Relationships</span></span>
<span data-ttu-id="0c435-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0c435-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c435-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0c435-140">JSON representation</span></span>

<span data-ttu-id="0c435-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c435-141">The following is a JSON representation of the resource.</span></span>

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
