---
title: Тип ресурса onlineMeeting
description: Содержит сведения о собрании.
author: jsandoval-msft
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 4e04e9f6d40be4e4ed9a432be6cc449c690790a7
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869857"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="20e45-103">Тип ресурса onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="20e45-103">onlineMeeting resource type</span></span>

<span data-ttu-id="20e45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20e45-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="20e45-105">Содержит сведения о собрании, включая URL-адрес собрания, список участников и описание.</span><span class="sxs-lookup"><span data-stu-id="20e45-105">Contains information about a meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="20e45-106">Методы</span><span class="sxs-lookup"><span data-stu-id="20e45-106">Methods</span></span>

| <span data-ttu-id="20e45-107">Метод</span><span class="sxs-lookup"><span data-stu-id="20e45-107">Method</span></span>                                                             | <span data-ttu-id="20e45-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="20e45-108">Return Type</span></span>                       | <span data-ttu-id="20e45-109">Описание</span><span class="sxs-lookup"><span data-stu-id="20e45-109">Description</span></span>                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="20e45-110">Создание объекта onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="20e45-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md)  | [<span data-ttu-id="20e45-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="20e45-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="20e45-112">Создание собрания в Интернете.</span><span class="sxs-lookup"><span data-stu-id="20e45-112">Create an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="20e45-113">Get onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="20e45-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md)                   | [<span data-ttu-id="20e45-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="20e45-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="20e45-115">Ознакомьтесь с свойствами и отношениями **объекта onlineMeeting.**</span><span class="sxs-lookup"><span data-stu-id="20e45-115">Read the properties and relationships of an **onlineMeeting** object.</span></span>                                        |
| [<span data-ttu-id="20e45-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="20e45-116">Update</span></span>](../api/onlinemeeting-update.md)                           | [<span data-ttu-id="20e45-117">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="20e45-117">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="20e45-118">Обновление свойств объекта **onlineMeeting.**</span><span class="sxs-lookup"><span data-stu-id="20e45-118">Update the properties of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="20e45-119">Удаление onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="20e45-119">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md)             | <span data-ttu-id="20e45-120">Нет</span><span class="sxs-lookup"><span data-stu-id="20e45-120">None</span></span>                              | <span data-ttu-id="20e45-121">Удаление **объекта onlineMeeting.**</span><span class="sxs-lookup"><span data-stu-id="20e45-121">Delete an **onlineMeeting** object.</span></span>                                                                                    |
| [<span data-ttu-id="20e45-122">Создание или доступ к onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="20e45-122">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="20e45-123">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="20e45-123">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="20e45-124">Создайте **объект onlineMeeting** с пользовательским внешним ID.</span><span class="sxs-lookup"><span data-stu-id="20e45-124">Create an **onlineMeeting** object with a custom, external ID.</span></span> <span data-ttu-id="20e45-125">Если собрание уже существует, извлекай его свойства.</span><span class="sxs-lookup"><span data-stu-id="20e45-125">If the meeting already exists, retrieve its properties.</span></span> |

## <a name="properties"></a><span data-ttu-id="20e45-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="20e45-126">Properties</span></span>

| <span data-ttu-id="20e45-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="20e45-127">Property</span></span>              | <span data-ttu-id="20e45-128">Тип</span><span class="sxs-lookup"><span data-stu-id="20e45-128">Type</span></span>                                          | <span data-ttu-id="20e45-129">Описание</span><span class="sxs-lookup"><span data-stu-id="20e45-129">Description</span></span>                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="20e45-130">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="20e45-130">allowedPresenters</span></span>     | [<span data-ttu-id="20e45-131">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="20e45-131">onlineMeetingPresenters</span></span>](#onlinemeetingpresenters-values)                       | <span data-ttu-id="20e45-132">Указывает, кто может быть презентовщиком на собрании.</span><span class="sxs-lookup"><span data-stu-id="20e45-132">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="20e45-133">Возможные значения перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="20e45-133">Possible values are listed in the following table.</span></span>                          |
| <span data-ttu-id="20e45-134">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="20e45-134">audioConferencing</span></span>     | [<span data-ttu-id="20e45-135">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="20e45-135">audioConferencing</span></span>](audioconferencing.md)     | <span data-ttu-id="20e45-136">Сведения о доступе к телефону для собрания в Интернете.</span><span class="sxs-lookup"><span data-stu-id="20e45-136">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="20e45-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20e45-137">Read-only.</span></span>                                                   |
| <span data-ttu-id="20e45-138">chatInfo</span><span class="sxs-lookup"><span data-stu-id="20e45-138">chatInfo</span></span>              | [<span data-ttu-id="20e45-139">chatInfo</span><span class="sxs-lookup"><span data-stu-id="20e45-139">chatInfo</span></span>](chatinfo.md)                       | <span data-ttu-id="20e45-140">Сведения о чате, связанные с этой онлайн-встречей.</span><span class="sxs-lookup"><span data-stu-id="20e45-140">The chat information associated with this online meeting.</span></span>                                                                  |
| <span data-ttu-id="20e45-141">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="20e45-141">creationDateTime</span></span>      | <span data-ttu-id="20e45-142">DateTime</span><span class="sxs-lookup"><span data-stu-id="20e45-142">DateTime</span></span>                                      | <span data-ttu-id="20e45-143">Время создания собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="20e45-143">The meeting creation time in UTC.</span></span> <span data-ttu-id="20e45-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20e45-144">Read-only.</span></span>                                                                               |
| <span data-ttu-id="20e45-145">endDateTime</span><span class="sxs-lookup"><span data-stu-id="20e45-145">endDateTime</span></span>           | <span data-ttu-id="20e45-146">DateTime</span><span class="sxs-lookup"><span data-stu-id="20e45-146">DateTime</span></span>                                      | <span data-ttu-id="20e45-147">Время окончания собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="20e45-147">The meeting end time in UTC.</span></span>                                                                                               |
| <span data-ttu-id="20e45-148">id</span><span class="sxs-lookup"><span data-stu-id="20e45-148">id</span></span>                    | <span data-ttu-id="20e45-149">String</span><span class="sxs-lookup"><span data-stu-id="20e45-149">String</span></span>                                        | <span data-ttu-id="20e45-150">ID по умолчанию, связанный с онлайн-собранием.</span><span class="sxs-lookup"><span data-stu-id="20e45-150">The default ID associated with the online meeting.</span></span> <span data-ttu-id="20e45-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20e45-151">Read-only.</span></span>                                                              |
| <span data-ttu-id="20e45-152">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="20e45-152">isEntryExitAnnounced</span></span>  | <span data-ttu-id="20e45-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="20e45-153">Boolean</span></span>                                       | <span data-ttu-id="20e45-154">Следует ли объявлять о том, когда звонители присоединяются или уходят.</span><span class="sxs-lookup"><span data-stu-id="20e45-154">Whether or not to announce when callers join or leave.</span></span>                                                                     |
| <span data-ttu-id="20e45-155">joinInformation</span><span class="sxs-lookup"><span data-stu-id="20e45-155">joinInformation</span></span>       | [<span data-ttu-id="20e45-156">itemBody</span><span class="sxs-lookup"><span data-stu-id="20e45-156">itemBody</span></span>](itembody.md)                       | <span data-ttu-id="20e45-157">Сведения о присоединиться в варианте языка и языка, указанные в `Accept-Language` заглавной странице HTTP запроса.</span><span class="sxs-lookup"><span data-stu-id="20e45-157">The join information in the language and locale variant specified in the `Accept-Language` request HTTP header.</span></span> <span data-ttu-id="20e45-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20e45-158">Read-only.</span></span> |
| <span data-ttu-id="20e45-159">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="20e45-159">joinWebUrl</span></span>            | <span data-ttu-id="20e45-160">String</span><span class="sxs-lookup"><span data-stu-id="20e45-160">String</span></span>                                        | <span data-ttu-id="20e45-161">URL-адрес присоединиться к собранию в Интернете.</span><span class="sxs-lookup"><span data-stu-id="20e45-161">The join URL of the online meeting.</span></span> <span data-ttu-id="20e45-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20e45-162">Read-only.</span></span>                                                                             |
| <span data-ttu-id="20e45-163">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="20e45-163">lobbyBypassSettings</span></span>   | [<span data-ttu-id="20e45-164">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="20e45-164">lobbyBypassSettings</span></span>](lobbyBypassSettings.md) | <span data-ttu-id="20e45-165">Указывает, какие участники могут обойти вестибюль собрания.</span><span class="sxs-lookup"><span data-stu-id="20e45-165">Specifies which participants can bypass the meeting   lobby.</span></span>                                                               |
| <span data-ttu-id="20e45-166">participants</span><span class="sxs-lookup"><span data-stu-id="20e45-166">participants</span></span>          | [<span data-ttu-id="20e45-167">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="20e45-167">meetingParticipants</span></span>](meetingparticipants.md) | <span data-ttu-id="20e45-168">Участники, связанные с онлайн-собранием.</span><span class="sxs-lookup"><span data-stu-id="20e45-168">The participants associated with the online meeting.</span></span>  <span data-ttu-id="20e45-169">Это включает организатора и участников.</span><span class="sxs-lookup"><span data-stu-id="20e45-169">This includes the organizer and the attendees.</span></span>                       |
| <span data-ttu-id="20e45-170">startDateTime</span><span class="sxs-lookup"><span data-stu-id="20e45-170">startDateTime</span></span>         | <span data-ttu-id="20e45-171">DateTime</span><span class="sxs-lookup"><span data-stu-id="20e45-171">DateTime</span></span>                                      | <span data-ttu-id="20e45-172">Время начала собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="20e45-172">The meeting start time in UTC.</span></span>                                                                                             |
| <span data-ttu-id="20e45-173">subject</span><span class="sxs-lookup"><span data-stu-id="20e45-173">subject</span></span>               | <span data-ttu-id="20e45-174">String</span><span class="sxs-lookup"><span data-stu-id="20e45-174">String</span></span>                                        | <span data-ttu-id="20e45-175">Тема собрания в Интернете.</span><span class="sxs-lookup"><span data-stu-id="20e45-175">The subject of the online meeting.</span></span>                                                                                         |
| <span data-ttu-id="20e45-176">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="20e45-176">videoTeleconferenceId</span></span> | <span data-ttu-id="20e45-177">String</span><span class="sxs-lookup"><span data-stu-id="20e45-177">String</span></span>                                        | <span data-ttu-id="20e45-178">ID видеоконференции.</span><span class="sxs-lookup"><span data-stu-id="20e45-178">The video teleconferencing ID.</span></span> <span data-ttu-id="20e45-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20e45-179">Read-only.</span></span>                                                                                  |

### <a name="onlinemeetingpresenters-values"></a><span data-ttu-id="20e45-180">значения onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="20e45-180">onlineMeetingPresenters values</span></span>

| <span data-ttu-id="20e45-181">Значение</span><span class="sxs-lookup"><span data-stu-id="20e45-181">Value</span></span>              | <span data-ttu-id="20e45-182">Описание</span><span class="sxs-lookup"><span data-stu-id="20e45-182">Description</span></span>                                                   |
| ------------------ | ------------------------------------------------------------- |
| <span data-ttu-id="20e45-183">все</span><span class="sxs-lookup"><span data-stu-id="20e45-183">everyone</span></span>           | <span data-ttu-id="20e45-184">Каждый — это презентер (это параметр по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="20e45-184">Everyone is a presenter (This is default option).</span></span>             |
| <span data-ttu-id="20e45-185">organization;</span><span class="sxs-lookup"><span data-stu-id="20e45-185">organization</span></span>       | <span data-ttu-id="20e45-186">Каждый в организации организатора — это презентер.</span><span class="sxs-lookup"><span data-stu-id="20e45-186">Everyone in organizer’s organization is a presenter.</span></span>          |
| <span data-ttu-id="20e45-187">roleIsPresenter</span><span class="sxs-lookup"><span data-stu-id="20e45-187">roleIsPresenter</span></span>    | <span data-ttu-id="20e45-188">Только участники, роль которых является презентатором, являются участниками.</span><span class="sxs-lookup"><span data-stu-id="20e45-188">Only the participants whose role is presenter are presenters.</span></span> |
| <span data-ttu-id="20e45-189">organizer</span><span class="sxs-lookup"><span data-stu-id="20e45-189">organizer</span></span>          | <span data-ttu-id="20e45-190">Только организатор — это презентер.</span><span class="sxs-lookup"><span data-stu-id="20e45-190">Only the organizer  is a presenter.</span></span>                           |
| <span data-ttu-id="20e45-191">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="20e45-191">unknownFutureValue</span></span> | <span data-ttu-id="20e45-192">Unknow future value.</span><span class="sxs-lookup"><span data-stu-id="20e45-192">Unknow future value.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="20e45-193">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20e45-193">JSON representation</span></span>

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

