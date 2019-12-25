---
title: Тип ресурса Онлинемитинг
description: Содержит сведения о собрании, включая URL-адрес присоединения, список участников и описание.
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 105c9f3ffa594dd457b40124070aef0dbb96689a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871389"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="3e1b3-103">Тип ресурса Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="3e1b3-103">onlineMeeting resource type</span></span>

<span data-ttu-id="3e1b3-104">Содержит сведения о собрании, включая URL-адрес, используемый для присоединения к собранию, список участников и описание.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-104">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="3e1b3-105">Методы</span><span class="sxs-lookup"><span data-stu-id="3e1b3-105">Methods</span></span>

| <span data-ttu-id="3e1b3-106">Метод</span><span class="sxs-lookup"><span data-stu-id="3e1b3-106">Method</span></span>         | <span data-ttu-id="3e1b3-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3e1b3-107">Return Type</span></span> | <span data-ttu-id="3e1b3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3e1b3-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="3e1b3-109">Создание Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="3e1b3-109">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="3e1b3-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="3e1b3-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="3e1b3-111">Создайте собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-111">Create an online meeting.</span></span> |
| [<span data-ttu-id="3e1b3-112">Получение Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="3e1b3-112">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="3e1b3-113">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="3e1b3-113">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="3e1b3-114">Чтение свойств и связей объекта **онлинемитинг** .</span><span class="sxs-lookup"><span data-stu-id="3e1b3-114">Read the properties and relationships of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="3e1b3-115">Удаление Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="3e1b3-115">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md) | <span data-ttu-id="3e1b3-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-116">None</span></span> | <span data-ttu-id="3e1b3-117">Удаление собрания по сети</span><span class="sxs-lookup"><span data-stu-id="3e1b3-117">Delete an online meeting</span></span> |

## <a name="properties"></a><span data-ttu-id="3e1b3-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e1b3-118">Properties</span></span>

| <span data-ttu-id="3e1b3-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e1b3-119">Property</span></span>                  | <span data-ttu-id="3e1b3-120">Тип</span><span class="sxs-lookup"><span data-stu-id="3e1b3-120">Type</span></span>                                                   | <span data-ttu-id="3e1b3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3e1b3-121">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="3e1b3-122">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="3e1b3-122">audioConferencing</span></span>         | [<span data-ttu-id="3e1b3-123">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="3e1b3-123">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="3e1b3-124">Сведения о телефонном доступе (телефонное подключение) для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-124">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="3e1b3-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-125">Read-only.</span></span> |
| <span data-ttu-id="3e1b3-126">chatInfo</span><span class="sxs-lookup"><span data-stu-id="3e1b3-126">chatInfo</span></span>                  | [<span data-ttu-id="3e1b3-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="3e1b3-127">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="3e1b3-128">Сведения о чате, связанные с этим собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-128">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="3e1b3-129">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="3e1b3-129">creationDateTime</span></span>          | <span data-ttu-id="3e1b3-130">DateTime</span><span class="sxs-lookup"><span data-stu-id="3e1b3-130">DateTime</span></span>                                               | <span data-ttu-id="3e1b3-131">Время создания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-131">The meeting creation time in UTC.</span></span> <span data-ttu-id="3e1b3-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-132">Read-only.</span></span> |
| <span data-ttu-id="3e1b3-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3e1b3-133">startDateTime</span></span>             | <span data-ttu-id="3e1b3-134">DateTime</span><span class="sxs-lookup"><span data-stu-id="3e1b3-134">DateTime</span></span>                                               | <span data-ttu-id="3e1b3-135">Время начала собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-135">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="3e1b3-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3e1b3-136">endDateTime</span></span>               | <span data-ttu-id="3e1b3-137">DateTime</span><span class="sxs-lookup"><span data-stu-id="3e1b3-137">DateTime</span></span>                                               | <span data-ttu-id="3e1b3-138">Время окончания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-138">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="3e1b3-139">id</span><span class="sxs-lookup"><span data-stu-id="3e1b3-139">id</span></span>                        | <span data-ttu-id="3e1b3-140">Строка</span><span class="sxs-lookup"><span data-stu-id="3e1b3-140">String</span></span>                                                 | <span data-ttu-id="3e1b3-141">ИДЕНТИФИКАТОР по умолчанию, связанный с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-141">The default ID associated with the online meeting.</span></span> <span data-ttu-id="3e1b3-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-142">Read-only.</span></span> |
| <span data-ttu-id="3e1b3-143">жоинвебурл</span><span class="sxs-lookup"><span data-stu-id="3e1b3-143">joinWebUrl</span></span>                | <span data-ttu-id="3e1b3-144">String</span><span class="sxs-lookup"><span data-stu-id="3e1b3-144">String</span></span>                                                 | <span data-ttu-id="3e1b3-145">URL-адрес присоединения к собранию по сети.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-145">The join URL of the online meeting.</span></span> <span data-ttu-id="3e1b3-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-146">Read-only.</span></span>|
| <span data-ttu-id="3e1b3-147">participants</span><span class="sxs-lookup"><span data-stu-id="3e1b3-147">participants</span></span>              | [<span data-ttu-id="3e1b3-148">митингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="3e1b3-148">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="3e1b3-149">Участники, связанные с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-149">The participants associated with the online meeting.</span></span>  <span data-ttu-id="3e1b3-150">Сюда входят Организатор и участники.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-150">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="3e1b3-151">subject</span><span class="sxs-lookup"><span data-stu-id="3e1b3-151">subject</span></span>                   | <span data-ttu-id="3e1b3-152">String</span><span class="sxs-lookup"><span data-stu-id="3e1b3-152">String</span></span>                                                 | <span data-ttu-id="3e1b3-153">Тема собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-153">The subject of the online meeting.</span></span> |
| <span data-ttu-id="3e1b3-154">видеотелеконференцеид</span><span class="sxs-lookup"><span data-stu-id="3e1b3-154">videoTeleconferenceId</span></span>     | <span data-ttu-id="3e1b3-155">String</span><span class="sxs-lookup"><span data-stu-id="3e1b3-155">String</span></span>                                                 | <span data-ttu-id="3e1b3-156">Идентификатор телеконференций видеио.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-156">The videio teleconferencing ID.</span></span> <span data-ttu-id="3e1b3-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e1b3-157">Read-only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="3e1b3-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e1b3-158">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "videoTeleconferenceId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
