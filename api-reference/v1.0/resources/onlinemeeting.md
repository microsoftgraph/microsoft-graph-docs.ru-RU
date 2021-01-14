---
title: Тип ресурса onlineMeeting
description: Содержит сведения о собрании.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 139cd4a20a6097691189d1bd1f843850ba911a21
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866111"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="9cb34-103">Тип ресурса onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="9cb34-103">onlineMeeting resource type</span></span>

<span data-ttu-id="9cb34-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cb34-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9cb34-105">Содержит сведения о собрании, включая URL-адрес, используемый для присоединиться к собранию, список участников и описание.</span><span class="sxs-lookup"><span data-stu-id="9cb34-105">Contains information about a meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="9cb34-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9cb34-106">Methods</span></span>

| <span data-ttu-id="9cb34-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9cb34-107">Method</span></span>                                                             | <span data-ttu-id="9cb34-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9cb34-108">Return Type</span></span>                       | <span data-ttu-id="9cb34-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9cb34-109">Description</span></span>                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="9cb34-110">Создание объекта onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="9cb34-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md)  | [<span data-ttu-id="9cb34-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="9cb34-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="9cb34-112">Создание собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="9cb34-112">Create an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="9cb34-113">Get onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="9cb34-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md)                   | [<span data-ttu-id="9cb34-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="9cb34-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="9cb34-115">Чтение свойств и связей объекта **onlineMeeting.**</span><span class="sxs-lookup"><span data-stu-id="9cb34-115">Read the properties and relationships of an **onlineMeeting** object.</span></span>                                        |
| [<span data-ttu-id="9cb34-116">Удаление onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="9cb34-116">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md)             | <span data-ttu-id="9cb34-117">Нет</span><span class="sxs-lookup"><span data-stu-id="9cb34-117">None</span></span>                              | <span data-ttu-id="9cb34-118">Удаление собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="9cb34-118">Delete an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="9cb34-119">Создание или get onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="9cb34-119">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="9cb34-120">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="9cb34-120">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="9cb34-121">Создание собрания по сети с пользовательским внешним ИД.</span><span class="sxs-lookup"><span data-stu-id="9cb34-121">Create an online meeting with a custom, external ID.</span></span> <span data-ttu-id="9cb34-122">Если собрание уже существует, извлекаете его свойства.</span><span class="sxs-lookup"><span data-stu-id="9cb34-122">If the meeting already exists, retrieve its properties.</span></span> |

## <a name="properties"></a><span data-ttu-id="9cb34-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="9cb34-123">Properties</span></span>

| <span data-ttu-id="9cb34-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cb34-124">Property</span></span>              | <span data-ttu-id="9cb34-125">Тип</span><span class="sxs-lookup"><span data-stu-id="9cb34-125">Type</span></span>                                          | <span data-ttu-id="9cb34-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9cb34-126">Description</span></span>                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9cb34-127">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="9cb34-127">audioConferencing</span></span>     | [<span data-ttu-id="9cb34-128">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="9cb34-128">audioConferencing</span></span>](audioconferencing.md)     | <span data-ttu-id="9cb34-129">Сведения о телефонном доступе (с телефонным доступом) для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="9cb34-129">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="9cb34-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cb34-130">Read-only.</span></span>                                                   |
| <span data-ttu-id="9cb34-131">chatInfo</span><span class="sxs-lookup"><span data-stu-id="9cb34-131">chatInfo</span></span>              | [<span data-ttu-id="9cb34-132">chatInfo</span><span class="sxs-lookup"><span data-stu-id="9cb34-132">chatInfo</span></span>](chatinfo.md)                       | <span data-ttu-id="9cb34-133">Сведения чата, связанные с этим собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="9cb34-133">The chat information associated with this online meeting.</span></span>                                                                  |
| <span data-ttu-id="9cb34-134">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="9cb34-134">creationDateTime</span></span>      | <span data-ttu-id="9cb34-135">DateTime</span><span class="sxs-lookup"><span data-stu-id="9cb34-135">DateTime</span></span>                                      | <span data-ttu-id="9cb34-136">Время создания собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="9cb34-136">The meeting creation time in UTC.</span></span> <span data-ttu-id="9cb34-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cb34-137">Read-only.</span></span>                                                                               |
| <span data-ttu-id="9cb34-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9cb34-138">startDateTime</span></span>         | <span data-ttu-id="9cb34-139">DateTime</span><span class="sxs-lookup"><span data-stu-id="9cb34-139">DateTime</span></span>                                      | <span data-ttu-id="9cb34-140">Время начала собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="9cb34-140">The meeting start time in UTC.</span></span>                                                                                             |
| <span data-ttu-id="9cb34-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9cb34-141">endDateTime</span></span>           | <span data-ttu-id="9cb34-142">DateTime</span><span class="sxs-lookup"><span data-stu-id="9cb34-142">DateTime</span></span>                                      | <span data-ttu-id="9cb34-143">Время окончания собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="9cb34-143">The meeting end time in UTC.</span></span>                                                                                               |
| <span data-ttu-id="9cb34-144">id</span><span class="sxs-lookup"><span data-stu-id="9cb34-144">id</span></span>                    | <span data-ttu-id="9cb34-145">String</span><span class="sxs-lookup"><span data-stu-id="9cb34-145">String</span></span>                                        | <span data-ttu-id="9cb34-146">ИД по умолчанию, связанный с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="9cb34-146">The default ID associated with the online meeting.</span></span> <span data-ttu-id="9cb34-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cb34-147">Read-only.</span></span>                                                              |
| <span data-ttu-id="9cb34-148">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="9cb34-148">joinWebUrl</span></span>            | <span data-ttu-id="9cb34-149">String</span><span class="sxs-lookup"><span data-stu-id="9cb34-149">String</span></span>                                        | <span data-ttu-id="9cb34-150">URL-адрес собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="9cb34-150">The join URL of the online meeting.</span></span> <span data-ttu-id="9cb34-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cb34-151">Read-only.</span></span>                                                                             |
| <span data-ttu-id="9cb34-152">participants</span><span class="sxs-lookup"><span data-stu-id="9cb34-152">participants</span></span>          | [<span data-ttu-id="9cb34-153">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="9cb34-153">meetingParticipants</span></span>](meetingparticipants.md) | <span data-ttu-id="9cb34-154">Участники, связанные с онлайн-собранием.</span><span class="sxs-lookup"><span data-stu-id="9cb34-154">The participants associated with the online meeting.</span></span>  <span data-ttu-id="9cb34-155">К ним относятся организатор и участники.</span><span class="sxs-lookup"><span data-stu-id="9cb34-155">This includes the organizer and the attendees.</span></span>                       |
| <span data-ttu-id="9cb34-156">subject</span><span class="sxs-lookup"><span data-stu-id="9cb34-156">subject</span></span>               | <span data-ttu-id="9cb34-157">String</span><span class="sxs-lookup"><span data-stu-id="9cb34-157">String</span></span>                                        | <span data-ttu-id="9cb34-158">Тема собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="9cb34-158">The subject of the online meeting.</span></span>                                                                                         |
| <span data-ttu-id="9cb34-159">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="9cb34-159">videoTeleconferenceId</span></span> | <span data-ttu-id="9cb34-160">String</span><span class="sxs-lookup"><span data-stu-id="9cb34-160">String</span></span>                                        | <span data-ttu-id="9cb34-161">ИД видеоконференции.</span><span class="sxs-lookup"><span data-stu-id="9cb34-161">The video teleconferencing ID.</span></span> <span data-ttu-id="9cb34-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cb34-162">Read-only.</span></span>                                                                                  |
| <span data-ttu-id="9cb34-163">joinInformation</span><span class="sxs-lookup"><span data-stu-id="9cb34-163">joinInformation</span></span>       | [<span data-ttu-id="9cb34-164">itemBody</span><span class="sxs-lookup"><span data-stu-id="9cb34-164">itemBody</span></span>](itembody.md)                       | <span data-ttu-id="9cb34-165">Сведения о подступах к языку и языковом варианте, указанные в `Accept-Language` http-заголке запроса.</span><span class="sxs-lookup"><span data-stu-id="9cb34-165">The join information in the language and locale variant specified in the `Accept-Language` request HTTP header.</span></span> <span data-ttu-id="9cb34-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cb34-166">Read-only.</span></span> |
| <span data-ttu-id="9cb34-167">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="9cb34-167">isEntryExitAnnounced</span></span>  | <span data-ttu-id="9cb34-168">Логический</span><span class="sxs-lookup"><span data-stu-id="9cb34-168">Boolean</span></span>                                       | <span data-ttu-id="9cb34-169">Следует ли объявлять, когда звонят, присоединяться или уходить.</span><span class="sxs-lookup"><span data-stu-id="9cb34-169">Whether or not to announce when callers join or leave.</span></span>                                                                     |
| <span data-ttu-id="9cb34-170">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="9cb34-170">lobbyBypassSettings</span></span>   | [<span data-ttu-id="9cb34-171">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="9cb34-171">lobbyBypassSettings</span></span>](lobbyBypassSettings.md) | <span data-ttu-id="9cb34-172">Указывает, какие участники могут обходить "lobby" собрания.</span><span class="sxs-lookup"><span data-stu-id="9cb34-172">Specifies which participants can bypass the meeting   lobby.</span></span>                                                               |
| <span data-ttu-id="9cb34-173">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="9cb34-173">allowedPresenters</span></span>     | <span data-ttu-id="9cb34-174">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="9cb34-174">onlineMeetingPresenters</span></span>                       | <span data-ttu-id="9cb34-175">Указывает, кто может быть presenter в собрании.</span><span class="sxs-lookup"><span data-stu-id="9cb34-175">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="9cb34-176">Возможные значения перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="9cb34-176">Possible values are listed in the following table.</span></span>                          |

### <a name="onlinemeetingpresenters-values"></a><span data-ttu-id="9cb34-177">Значения onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="9cb34-177">onlineMeetingPresenters values</span></span>

| <span data-ttu-id="9cb34-178">Значение</span><span class="sxs-lookup"><span data-stu-id="9cb34-178">Value</span></span>              | <span data-ttu-id="9cb34-179">Описание</span><span class="sxs-lookup"><span data-stu-id="9cb34-179">Description</span></span>                                                   |
| ------------------ | ------------------------------------------------------------- |
| <span data-ttu-id="9cb34-180">все</span><span class="sxs-lookup"><span data-stu-id="9cb34-180">everyone</span></span>           | <span data-ttu-id="9cb34-181">Все — это presenter (это параметр по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="9cb34-181">Everyone is a presenter (This is default option).</span></span>             |
| <span data-ttu-id="9cb34-182">organization;</span><span class="sxs-lookup"><span data-stu-id="9cb34-182">organization</span></span>       | <span data-ttu-id="9cb34-183">Все в организации организатора — это организатор.</span><span class="sxs-lookup"><span data-stu-id="9cb34-183">Everyone in organizer’s organization is a presenter.</span></span>          |
| <span data-ttu-id="9cb34-184">roleIsPresenter</span><span class="sxs-lookup"><span data-stu-id="9cb34-184">roleIsPresenter</span></span>    | <span data-ttu-id="9cb34-185">Только участники, роль которых является presenter, являются участниками.</span><span class="sxs-lookup"><span data-stu-id="9cb34-185">Only the participants whose role is presenter are presenters.</span></span> |
| <span data-ttu-id="9cb34-186">organizer</span><span class="sxs-lookup"><span data-stu-id="9cb34-186">organizer</span></span>          | <span data-ttu-id="9cb34-187">Только организатор является организатором.</span><span class="sxs-lookup"><span data-stu-id="9cb34-187">Only the organizer  is a presenter.</span></span>                           |
| <span data-ttu-id="9cb34-188">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="9cb34-188">unknownFutureValue</span></span> | <span data-ttu-id="9cb34-189">Unknow future value.</span><span class="sxs-lookup"><span data-stu-id="9cb34-189">Unknow future value.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="9cb34-190">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9cb34-190">JSON representation</span></span>

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
  "videoTeleconferenceId": "String",
  "isEntryExitAnnounced": "Boolean",
  "lobbyBypassSettings": {"@odata.type": "#microsoft.graph.lobbyBypassSettings"},
  "allowedPresenters": "String"
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

