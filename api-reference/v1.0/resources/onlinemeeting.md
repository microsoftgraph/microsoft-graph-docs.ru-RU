---
title: Тип ресурса Онлинемитинг
description: Содержит сведения о собрании, включая URL-адрес присоединения, список участников и описание.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 531413ee2a9c322af99a98ecf2270faa50ccb0e0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534158"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="3b3a1-103">Тип ресурса Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="3b3a1-103">onlineMeeting resource type</span></span>

<span data-ttu-id="3b3a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b3a1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3b3a1-105">Содержит сведения о собрании, включая URL-адрес, используемый для присоединения к собранию, список участников и описание.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-105">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="3b3a1-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3b3a1-106">Methods</span></span>

| <span data-ttu-id="3b3a1-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3b3a1-107">Method</span></span>         | <span data-ttu-id="3b3a1-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3b3a1-108">Return Type</span></span> | <span data-ttu-id="3b3a1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3b3a1-109">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="3b3a1-110">Создание объекта onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="3b3a1-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="3b3a1-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="3b3a1-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="3b3a1-112">Создайте собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-112">Create an online meeting.</span></span> |
| [<span data-ttu-id="3b3a1-113">Получение Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="3b3a1-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="3b3a1-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="3b3a1-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="3b3a1-115">Чтение свойств и связей объекта **онлинемитинг** .</span><span class="sxs-lookup"><span data-stu-id="3b3a1-115">Read the properties and relationships of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="3b3a1-116">Удаление Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="3b3a1-116">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md) | <span data-ttu-id="3b3a1-117">Нет</span><span class="sxs-lookup"><span data-stu-id="3b3a1-117">None</span></span> | <span data-ttu-id="3b3a1-118">Удаление собрания по сети</span><span class="sxs-lookup"><span data-stu-id="3b3a1-118">Delete an online meeting</span></span> |

## <a name="properties"></a><span data-ttu-id="3b3a1-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b3a1-119">Properties</span></span>

| <span data-ttu-id="3b3a1-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b3a1-120">Property</span></span>                  | <span data-ttu-id="3b3a1-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3b3a1-121">Type</span></span>                                                   | <span data-ttu-id="3b3a1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3b3a1-122">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="3b3a1-123">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="3b3a1-123">audioConferencing</span></span>         | [<span data-ttu-id="3b3a1-124">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="3b3a1-124">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="3b3a1-125">Сведения о телефонном доступе (телефонное подключение) для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-125">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="3b3a1-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-126">Read-only.</span></span> |
| <span data-ttu-id="3b3a1-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="3b3a1-127">chatInfo</span></span>                  | [<span data-ttu-id="3b3a1-128">chatInfo</span><span class="sxs-lookup"><span data-stu-id="3b3a1-128">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="3b3a1-129">Сведения о чате, связанные с этим собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-129">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="3b3a1-130">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="3b3a1-130">creationDateTime</span></span>          | <span data-ttu-id="3b3a1-131">DateTime</span><span class="sxs-lookup"><span data-stu-id="3b3a1-131">DateTime</span></span>                                               | <span data-ttu-id="3b3a1-132">Время создания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-132">The meeting creation time in UTC.</span></span> <span data-ttu-id="3b3a1-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-133">Read-only.</span></span> |
| <span data-ttu-id="3b3a1-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3b3a1-134">startDateTime</span></span>             | <span data-ttu-id="3b3a1-135">DateTime</span><span class="sxs-lookup"><span data-stu-id="3b3a1-135">DateTime</span></span>                                               | <span data-ttu-id="3b3a1-136">Время начала собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-136">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="3b3a1-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3b3a1-137">endDateTime</span></span>               | <span data-ttu-id="3b3a1-138">DateTime</span><span class="sxs-lookup"><span data-stu-id="3b3a1-138">DateTime</span></span>                                               | <span data-ttu-id="3b3a1-139">Время окончания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-139">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="3b3a1-140">id</span><span class="sxs-lookup"><span data-stu-id="3b3a1-140">id</span></span>                        | <span data-ttu-id="3b3a1-141">Строка</span><span class="sxs-lookup"><span data-stu-id="3b3a1-141">String</span></span>                                                 | <span data-ttu-id="3b3a1-142">ИДЕНТИФИКАТОР по умолчанию, связанный с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-142">The default ID associated with the online meeting.</span></span> <span data-ttu-id="3b3a1-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-143">Read-only.</span></span> |
| <span data-ttu-id="3b3a1-144">жоинвебурл</span><span class="sxs-lookup"><span data-stu-id="3b3a1-144">joinWebUrl</span></span>                | <span data-ttu-id="3b3a1-145">String</span><span class="sxs-lookup"><span data-stu-id="3b3a1-145">String</span></span>                                                 | <span data-ttu-id="3b3a1-146">URL-адрес присоединения к собранию по сети.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-146">The join URL of the online meeting.</span></span> <span data-ttu-id="3b3a1-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-147">Read-only.</span></span>|
| <span data-ttu-id="3b3a1-148">participants</span><span class="sxs-lookup"><span data-stu-id="3b3a1-148">participants</span></span>              | [<span data-ttu-id="3b3a1-149">митингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="3b3a1-149">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="3b3a1-150">Участники, связанные с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-150">The participants associated with the online meeting.</span></span>  <span data-ttu-id="3b3a1-151">Сюда входят Организатор и участники.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-151">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="3b3a1-152">subject</span><span class="sxs-lookup"><span data-stu-id="3b3a1-152">subject</span></span>                   | <span data-ttu-id="3b3a1-153">String</span><span class="sxs-lookup"><span data-stu-id="3b3a1-153">String</span></span>                                                 | <span data-ttu-id="3b3a1-154">Тема собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-154">The subject of the online meeting.</span></span> |
| <span data-ttu-id="3b3a1-155">видеотелеконференцеид</span><span class="sxs-lookup"><span data-stu-id="3b3a1-155">videoTeleconferenceId</span></span>     | <span data-ttu-id="3b3a1-156">String</span><span class="sxs-lookup"><span data-stu-id="3b3a1-156">String</span></span>                                                 | <span data-ttu-id="3b3a1-157">Идентификатор видеоконференций для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-157">The video teleconferencing ID.</span></span> <span data-ttu-id="3b3a1-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b3a1-158">Read-only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="3b3a1-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b3a1-159">JSON representation</span></span>

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
