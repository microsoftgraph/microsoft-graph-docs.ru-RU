---
title: Тип ресурса onlineMeeting
description: Содержит сведения о собрании.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 8ded2e79f8a9a2004f2ffa412b6d42e3275556b8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516096"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="523d8-103">Тип ресурса onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="523d8-103">onlineMeeting resource type</span></span>

<span data-ttu-id="523d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="523d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="523d8-105">Содержит сведения о собрании, включая URL-адрес собрания, список участников и описание.</span><span class="sxs-lookup"><span data-stu-id="523d8-105">Contains information about a meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="523d8-106">Методы</span><span class="sxs-lookup"><span data-stu-id="523d8-106">Methods</span></span>

| <span data-ttu-id="523d8-107">Метод</span><span class="sxs-lookup"><span data-stu-id="523d8-107">Method</span></span>                                                             | <span data-ttu-id="523d8-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="523d8-108">Return Type</span></span>                       | <span data-ttu-id="523d8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="523d8-109">Description</span></span>                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="523d8-110">Создание объекта onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="523d8-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md)  | [<span data-ttu-id="523d8-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="523d8-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="523d8-112">Создание собрания в Интернете.</span><span class="sxs-lookup"><span data-stu-id="523d8-112">Create an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="523d8-113">Get onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="523d8-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md)                   | [<span data-ttu-id="523d8-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="523d8-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="523d8-115">Ознакомьтесь с свойствами и отношениями **объекта onlineMeeting.**</span><span class="sxs-lookup"><span data-stu-id="523d8-115">Read the properties and relationships of an **onlineMeeting** object.</span></span>                                        |
| <span data-ttu-id="523d8-116">[обновление](../api/onlinemeeting-update.md).</span><span class="sxs-lookup"><span data-stu-id="523d8-116">[Update](../api/onlinemeeting-update.md)</span></span>                           | [<span data-ttu-id="523d8-117">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="523d8-117">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="523d8-118">Обновление свойств объекта **onlineMeeting.**</span><span class="sxs-lookup"><span data-stu-id="523d8-118">Update the properties of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="523d8-119">Удаление onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="523d8-119">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md)             | <span data-ttu-id="523d8-120">Нет</span><span class="sxs-lookup"><span data-stu-id="523d8-120">None</span></span>                              | <span data-ttu-id="523d8-121">Удаление **объекта onlineMeeting.**</span><span class="sxs-lookup"><span data-stu-id="523d8-121">Delete an **onlineMeeting** object.</span></span>                                                                                    |
| [<span data-ttu-id="523d8-122">Создание или доступ к onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="523d8-122">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="523d8-123">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="523d8-123">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="523d8-124">Создайте **объект onlineMeeting** с пользовательским внешним ID.</span><span class="sxs-lookup"><span data-stu-id="523d8-124">Create an **onlineMeeting** object with a custom, external ID.</span></span> <span data-ttu-id="523d8-125">Если собрание уже существует, извлекай его свойства.</span><span class="sxs-lookup"><span data-stu-id="523d8-125">If the meeting already exists, retrieve its properties.</span></span> |

## <a name="properties"></a><span data-ttu-id="523d8-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="523d8-126">Properties</span></span>

| <span data-ttu-id="523d8-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="523d8-127">Property</span></span>              | <span data-ttu-id="523d8-128">Тип</span><span class="sxs-lookup"><span data-stu-id="523d8-128">Type</span></span>                                          | <span data-ttu-id="523d8-129">Описание</span><span class="sxs-lookup"><span data-stu-id="523d8-129">Description</span></span>                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="523d8-130">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="523d8-130">allowedPresenters</span></span>     | <span data-ttu-id="523d8-131">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="523d8-131">onlineMeetingPresenters</span></span>                       | <span data-ttu-id="523d8-132">Указывает, кто может быть презентовщиком на собрании.</span><span class="sxs-lookup"><span data-stu-id="523d8-132">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="523d8-133">Возможные значения перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="523d8-133">Possible values are listed in the following table.</span></span>                          |
| <span data-ttu-id="523d8-134">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="523d8-134">audioConferencing</span></span>     | [<span data-ttu-id="523d8-135">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="523d8-135">audioConferencing</span></span>](audioconferencing.md)     | <span data-ttu-id="523d8-136">Сведения о доступе к телефону для собрания в Интернете.</span><span class="sxs-lookup"><span data-stu-id="523d8-136">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="523d8-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="523d8-137">Read-only.</span></span>                                                   |
| <span data-ttu-id="523d8-138">chatInfo</span><span class="sxs-lookup"><span data-stu-id="523d8-138">chatInfo</span></span>              | [<span data-ttu-id="523d8-139">chatInfo</span><span class="sxs-lookup"><span data-stu-id="523d8-139">chatInfo</span></span>](chatinfo.md)                       | <span data-ttu-id="523d8-140">Сведения о чате, связанные с этой онлайн-встречей.</span><span class="sxs-lookup"><span data-stu-id="523d8-140">The chat information associated with this online meeting.</span></span>                                                                  |
| <span data-ttu-id="523d8-141">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="523d8-141">creationDateTime</span></span>      | <span data-ttu-id="523d8-142">DateTime</span><span class="sxs-lookup"><span data-stu-id="523d8-142">DateTime</span></span>                                      | <span data-ttu-id="523d8-143">Время создания собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="523d8-143">The meeting creation time in UTC.</span></span> <span data-ttu-id="523d8-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="523d8-144">Read-only.</span></span>                                                                               |
| <span data-ttu-id="523d8-145">endDateTime</span><span class="sxs-lookup"><span data-stu-id="523d8-145">endDateTime</span></span>           | <span data-ttu-id="523d8-146">DateTime</span><span class="sxs-lookup"><span data-stu-id="523d8-146">DateTime</span></span>                                      | <span data-ttu-id="523d8-147">Время окончания собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="523d8-147">The meeting end time in UTC.</span></span>                                                                                               |
| <span data-ttu-id="523d8-148">id</span><span class="sxs-lookup"><span data-stu-id="523d8-148">id</span></span>                    | <span data-ttu-id="523d8-149">Строка</span><span class="sxs-lookup"><span data-stu-id="523d8-149">String</span></span>                                        | <span data-ttu-id="523d8-150">ID по умолчанию, связанный с онлайн-собранием.</span><span class="sxs-lookup"><span data-stu-id="523d8-150">The default ID associated with the online meeting.</span></span> <span data-ttu-id="523d8-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="523d8-151">Read-only.</span></span>                                                              |
| <span data-ttu-id="523d8-152">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="523d8-152">isEntryExitAnnounced</span></span>  | <span data-ttu-id="523d8-153">Логический</span><span class="sxs-lookup"><span data-stu-id="523d8-153">Boolean</span></span>                                       | <span data-ttu-id="523d8-154">Следует ли объявлять о том, когда звонители присоединяются или уходят.</span><span class="sxs-lookup"><span data-stu-id="523d8-154">Whether or not to announce when callers join or leave.</span></span>                                                                     |
| <span data-ttu-id="523d8-155">joinInformation</span><span class="sxs-lookup"><span data-stu-id="523d8-155">joinInformation</span></span>       | [<span data-ttu-id="523d8-156">itemBody</span><span class="sxs-lookup"><span data-stu-id="523d8-156">itemBody</span></span>](itembody.md)                       | <span data-ttu-id="523d8-157">Сведения о присоединиться в варианте языка и языка, указанные в `Accept-Language` заглавной странице HTTP запроса.</span><span class="sxs-lookup"><span data-stu-id="523d8-157">The join information in the language and locale variant specified in the `Accept-Language` request HTTP header.</span></span> <span data-ttu-id="523d8-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="523d8-158">Read-only.</span></span> |
| <span data-ttu-id="523d8-159">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="523d8-159">joinWebUrl</span></span>            | <span data-ttu-id="523d8-160">Строка</span><span class="sxs-lookup"><span data-stu-id="523d8-160">String</span></span>                                        | <span data-ttu-id="523d8-161">URL-адрес присоединиться к собранию в Интернете.</span><span class="sxs-lookup"><span data-stu-id="523d8-161">The join URL of the online meeting.</span></span> <span data-ttu-id="523d8-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="523d8-162">Read-only.</span></span>                                                                             |
| <span data-ttu-id="523d8-163">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="523d8-163">lobbyBypassSettings</span></span>   | [<span data-ttu-id="523d8-164">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="523d8-164">lobbyBypassSettings</span></span>](lobbyBypassSettings.md) | <span data-ttu-id="523d8-165">Указывает, какие участники могут обойти вестибюль собрания.</span><span class="sxs-lookup"><span data-stu-id="523d8-165">Specifies which participants can bypass the meeting   lobby.</span></span>                                                               |
| <span data-ttu-id="523d8-166">participants</span><span class="sxs-lookup"><span data-stu-id="523d8-166">participants</span></span>          | [<span data-ttu-id="523d8-167">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="523d8-167">meetingParticipants</span></span>](meetingparticipants.md) | <span data-ttu-id="523d8-168">Участники, связанные с онлайн-собранием.</span><span class="sxs-lookup"><span data-stu-id="523d8-168">The participants associated with the online meeting.</span></span>  <span data-ttu-id="523d8-169">Это включает организатора и участников.</span><span class="sxs-lookup"><span data-stu-id="523d8-169">This includes the organizer and the attendees.</span></span>                       |
| <span data-ttu-id="523d8-170">startDateTime</span><span class="sxs-lookup"><span data-stu-id="523d8-170">startDateTime</span></span>         | <span data-ttu-id="523d8-171">DateTime</span><span class="sxs-lookup"><span data-stu-id="523d8-171">DateTime</span></span>                                      | <span data-ttu-id="523d8-172">Время начала собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="523d8-172">The meeting start time in UTC.</span></span>                                                                                             |
| <span data-ttu-id="523d8-173">subject</span><span class="sxs-lookup"><span data-stu-id="523d8-173">subject</span></span>               | <span data-ttu-id="523d8-174">String</span><span class="sxs-lookup"><span data-stu-id="523d8-174">String</span></span>                                        | <span data-ttu-id="523d8-175">Тема собрания в Интернете.</span><span class="sxs-lookup"><span data-stu-id="523d8-175">The subject of the online meeting.</span></span>                                                                                         |
| <span data-ttu-id="523d8-176">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="523d8-176">videoTeleconferenceId</span></span> | <span data-ttu-id="523d8-177">Строка</span><span class="sxs-lookup"><span data-stu-id="523d8-177">String</span></span>                                        | <span data-ttu-id="523d8-178">ID видеоконференции.</span><span class="sxs-lookup"><span data-stu-id="523d8-178">The video teleconferencing ID.</span></span> <span data-ttu-id="523d8-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="523d8-179">Read-only.</span></span>                                                                                  |

### <a name="onlinemeetingpresenters-values"></a><span data-ttu-id="523d8-180">значения onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="523d8-180">onlineMeetingPresenters values</span></span>

| <span data-ttu-id="523d8-181">Значение</span><span class="sxs-lookup"><span data-stu-id="523d8-181">Value</span></span>              | <span data-ttu-id="523d8-182">Описание</span><span class="sxs-lookup"><span data-stu-id="523d8-182">Description</span></span>                                                   |
| ------------------ | ------------------------------------------------------------- |
| <span data-ttu-id="523d8-183">все</span><span class="sxs-lookup"><span data-stu-id="523d8-183">everyone</span></span>           | <span data-ttu-id="523d8-184">Каждый — это презентер (это параметр по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="523d8-184">Everyone is a presenter (This is default option).</span></span>             |
| <span data-ttu-id="523d8-185">organization;</span><span class="sxs-lookup"><span data-stu-id="523d8-185">organization</span></span>       | <span data-ttu-id="523d8-186">Каждый в организации организатора — это презентер.</span><span class="sxs-lookup"><span data-stu-id="523d8-186">Everyone in organizer’s organization is a presenter.</span></span>          |
| <span data-ttu-id="523d8-187">roleIsPresenter</span><span class="sxs-lookup"><span data-stu-id="523d8-187">roleIsPresenter</span></span>    | <span data-ttu-id="523d8-188">Только участники, роль которых является презентатором, являются участниками.</span><span class="sxs-lookup"><span data-stu-id="523d8-188">Only the participants whose role is presenter are presenters.</span></span> |
| <span data-ttu-id="523d8-189">organizer</span><span class="sxs-lookup"><span data-stu-id="523d8-189">organizer</span></span>          | <span data-ttu-id="523d8-190">Только организатор — это презентер.</span><span class="sxs-lookup"><span data-stu-id="523d8-190">Only the organizer  is a presenter.</span></span>                           |
| <span data-ttu-id="523d8-191">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="523d8-191">unknownFutureValue</span></span> | <span data-ttu-id="523d8-192">Unknow future value.</span><span class="sxs-lookup"><span data-stu-id="523d8-192">Unknow future value.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="523d8-193">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="523d8-193">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "audioConferencing": {"@odata.type": "microsoft.graph.audioConferencing"},
  "chatInfo": {"@odata.type": "microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "participants": {"@odata.type": "microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "videoTeleconferenceId": "String",
  "isEntryExitAnnounced": "Boolean",
  "lobbyBypassSettings": {"@odata.type": "microsoft.graph.lobbyBypassSettings"},
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

