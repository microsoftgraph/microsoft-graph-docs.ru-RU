---
title: Тип ресурса Онлинемитинг
description: Содержит сведения о собрании, включая URL-адрес присоединения, список участников и описание.
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 64b2c1880edafe1241367ac91889440a513964d9
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006615"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="0d022-103">Тип ресурса Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="0d022-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d022-104">Содержит сведения о собрании, включая URL-адрес, используемый для присоединения к собранию, список участников и описание.</span><span class="sxs-lookup"><span data-stu-id="0d022-104">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="0d022-105">Методы</span><span class="sxs-lookup"><span data-stu-id="0d022-105">Methods</span></span>

| <span data-ttu-id="0d022-106">Метод</span><span class="sxs-lookup"><span data-stu-id="0d022-106">Method</span></span>         | <span data-ttu-id="0d022-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0d022-107">Return Type</span></span> | <span data-ttu-id="0d022-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0d022-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="0d022-109">Создание Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="0d022-109">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="0d022-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="0d022-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="0d022-111">Создайте собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="0d022-111">Create an online meeting.</span></span> |
| [<span data-ttu-id="0d022-112">Получение Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="0d022-112">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="0d022-113">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="0d022-113">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="0d022-114">Чтение свойств и связей объекта **онлинемитинг** .</span><span class="sxs-lookup"><span data-stu-id="0d022-114">Read the properties and relationships of an **onlineMeeting** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0d022-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d022-115">Properties</span></span>

| <span data-ttu-id="0d022-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d022-116">Property</span></span>                  | <span data-ttu-id="0d022-117">Тип</span><span class="sxs-lookup"><span data-stu-id="0d022-117">Type</span></span>                                                   | <span data-ttu-id="0d022-118">Описание</span><span class="sxs-lookup"><span data-stu-id="0d022-118">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="0d022-119">аутоадмиттедусерс</span><span class="sxs-lookup"><span data-stu-id="0d022-119">autoAdmittedUsers</span></span>         | <span data-ttu-id="0d022-120">String</span><span class="sxs-lookup"><span data-stu-id="0d022-120">String</span></span>                                                 | <span data-ttu-id="0d022-121">Параметр, указывающий тип участников, которые будут автоматически разрешены в собрании по сети.</span><span class="sxs-lookup"><span data-stu-id="0d022-121">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="0d022-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d022-122">Read-only.</span></span> <span data-ttu-id="0d022-123">`everyone`Возможные значения: `everyoneInSameAndFederatedCompany`,, `everyoneInCompany`,, `invitedUsersInCompany``organizer`</span><span class="sxs-lookup"><span data-stu-id="0d022-123">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`</span></span>|
| <span data-ttu-id="0d022-124">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="0d022-124">audioConferencing</span></span>         | [<span data-ttu-id="0d022-125">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="0d022-125">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="0d022-126">Сведения о телефонном доступе (телефонное подключение) для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="0d022-126">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="0d022-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d022-127">Read-only.</span></span> |
| <span data-ttu-id="0d022-128">канцеледдатетиме</span><span class="sxs-lookup"><span data-stu-id="0d022-128">canceledDateTime</span></span>          | <span data-ttu-id="0d022-129">DateTime</span><span class="sxs-lookup"><span data-stu-id="0d022-129">DateTime</span></span>                                               | <span data-ttu-id="0d022-130">Время в формате UTC, когда собрание было отменено.</span><span class="sxs-lookup"><span data-stu-id="0d022-130">The time in UTC when the meeting was canceled.</span></span> <span data-ttu-id="0d022-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d022-131">Read-only.</span></span> |
| <span data-ttu-id="0d022-132">chatInfo</span><span class="sxs-lookup"><span data-stu-id="0d022-132">chatInfo</span></span>                  | [<span data-ttu-id="0d022-133">chatInfo</span><span class="sxs-lookup"><span data-stu-id="0d022-133">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="0d022-134">Сведения о чате, связанные с этим собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="0d022-134">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="0d022-135">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="0d022-135">creationDateTime</span></span>          | <span data-ttu-id="0d022-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="0d022-136">DateTime</span></span>                                               | <span data-ttu-id="0d022-137">Время создания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0d022-137">The meeting creation time in UTC.</span></span> <span data-ttu-id="0d022-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d022-138">Read-only.</span></span> |
| <span data-ttu-id="0d022-139">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0d022-139">startDateTime</span></span>             | <span data-ttu-id="0d022-140">DateTime</span><span class="sxs-lookup"><span data-stu-id="0d022-140">DateTime</span></span>                                               | <span data-ttu-id="0d022-141">Время начала собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0d022-141">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="0d022-142">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0d022-142">endDateTime</span></span>               | <span data-ttu-id="0d022-143">DateTime</span><span class="sxs-lookup"><span data-stu-id="0d022-143">DateTime</span></span>                                               | <span data-ttu-id="0d022-144">Время окончания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0d022-144">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="0d022-145">id</span><span class="sxs-lookup"><span data-stu-id="0d022-145">id</span></span>                        | <span data-ttu-id="0d022-146">Строка</span><span class="sxs-lookup"><span data-stu-id="0d022-146">String</span></span>                                                 | <span data-ttu-id="0d022-147">ИДЕНТИФИКАТОР по умолчанию, связанный с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="0d022-147">The default ID associated with the online meeting.</span></span> <span data-ttu-id="0d022-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d022-148">Read-only.</span></span> |
| <span data-ttu-id="0d022-149">Отменено</span><span class="sxs-lookup"><span data-stu-id="0d022-149">isCanceled</span></span>                | <span data-ttu-id="0d022-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d022-150">Boolean</span></span>                                                | <span data-ttu-id="0d022-151">Указывает, было ли собрание отменено.</span><span class="sxs-lookup"><span data-stu-id="0d022-151">Indicates whether the meeting has been canceled.</span></span> <span data-ttu-id="0d022-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d022-152">Read-only.</span></span> |
| <span data-ttu-id="0d022-153">жоинурл</span><span class="sxs-lookup"><span data-stu-id="0d022-153">joinUrl</span></span>                   | <span data-ttu-id="0d022-154">String</span><span class="sxs-lookup"><span data-stu-id="0d022-154">String</span></span>                                                 | <span data-ttu-id="0d022-155">URL-адрес присоединения к собранию по сети.</span><span class="sxs-lookup"><span data-stu-id="0d022-155">The join URL of the online meeting.</span></span> <span data-ttu-id="0d022-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d022-156">Read-only.</span></span>|
| <span data-ttu-id="0d022-157">Передача</span><span class="sxs-lookup"><span data-stu-id="0d022-157">isBroadcast</span></span>               | <span data-ttu-id="0d022-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d022-158">Boolean</span></span>                                                | <span data-ttu-id="0d022-159">Указывает, является ли собрание широковещательным.</span><span class="sxs-lookup"><span data-stu-id="0d022-159">Indicates whether the meeting is a broadcast meeting.</span></span> |
| <span data-ttu-id="0d022-160">participants</span><span class="sxs-lookup"><span data-stu-id="0d022-160">participants</span></span>              | [<span data-ttu-id="0d022-161">митингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="0d022-161">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="0d022-162">Участники, связанные с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="0d022-162">The participants associated with the online meeting.</span></span>  <span data-ttu-id="0d022-163">Сюда входят Организатор и участники.</span><span class="sxs-lookup"><span data-stu-id="0d022-163">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="0d022-164">subject</span><span class="sxs-lookup"><span data-stu-id="0d022-164">subject</span></span>                   | <span data-ttu-id="0d022-165">String</span><span class="sxs-lookup"><span data-stu-id="0d022-165">String</span></span>                                                 | <span data-ttu-id="0d022-166">Тема собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="0d022-166">The subject of the online meeting.</span></span> |
| <span data-ttu-id="0d022-167">capabilities</span><span class="sxs-lookup"><span data-stu-id="0d022-167">capabilities</span></span>              | <span data-ttu-id="0d022-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0d022-168">String collection</span></span>                                      | <span data-ttu-id="0d022-169">Список возможностей собрания.</span><span class="sxs-lookup"><span data-stu-id="0d022-169">The list of meeting capabilities.</span></span> <span data-ttu-id="0d022-170">Возможные значения: `questionAndAnswer`.</span><span class="sxs-lookup"><span data-stu-id="0d022-170">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="0d022-171">видеотелеконференцеид</span><span class="sxs-lookup"><span data-stu-id="0d022-171">videoTeleconferenceId</span></span>     | <span data-ttu-id="0d022-172">String</span><span class="sxs-lookup"><span data-stu-id="0d022-172">String</span></span>                                                 | <span data-ttu-id="0d022-173">Идентификатор телеконференций видеио.</span><span class="sxs-lookup"><span data-stu-id="0d022-173">The videio teleconferencing ID.</span></span> <span data-ttu-id="0d022-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d022-174">Read-only.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="0d022-175">значения Аутоадмиттедусерс</span><span class="sxs-lookup"><span data-stu-id="0d022-175">autoAdmittedUsers values</span></span>
| <span data-ttu-id="0d022-176">Значение</span><span class="sxs-lookup"><span data-stu-id="0d022-176">Value</span></span> | <span data-ttu-id="0d022-177">Описание</span><span class="sxs-lookup"><span data-stu-id="0d022-177">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="0d022-178">organizer</span><span class="sxs-lookup"><span data-stu-id="0d022-178">organizer</span></span> | <span data-ttu-id="0d022-179">Только организатор собрания додается непосредственно.</span><span class="sxs-lookup"><span data-stu-id="0d022-179">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="0d022-180">Все остальные ожидают, пока организатор не выйдет.</span><span class="sxs-lookup"><span data-stu-id="0d022-180">Everyone else waits in the lobby, until admitted by the organizer</span></span>  |
| <span data-ttu-id="0d022-181">инвитедусерсинкомпани</span><span class="sxs-lookup"><span data-stu-id="0d022-181">invitedUsersInCompany</span></span> | <span data-ttu-id="0d022-182">Организатор собрания и пользователи в той же компании, приглашенные организатором, напрямую присоединяются к собранию.</span><span class="sxs-lookup"><span data-stu-id="0d022-182">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="0d022-183">Все остальные ожидают, пока не станет допущен.</span><span class="sxs-lookup"><span data-stu-id="0d022-183">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="0d022-184">еверйонеинкомпани</span><span class="sxs-lookup"><span data-stu-id="0d022-184">everyoneInCompany</span></span> | <span data-ttu-id="0d022-185">Все пользователи в той же организации, что и организатор, напрямую присоединяются к собранию.</span><span class="sxs-lookup"><span data-stu-id="0d022-185">Everyone in the same company as the organizer join the meeting directly.</span></span>  <span data-ttu-id="0d022-186">Федеративные анонимные пользователи ожидают, пока не допустить ожидания.</span><span class="sxs-lookup"><span data-stu-id="0d022-186">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="0d022-187">еверйонеинсамеандфедератедкомпани</span><span class="sxs-lookup"><span data-stu-id="0d022-187">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="0d022-188">Все пользователи в той же организации, что и организатор и Федеративные компании, присоединяются к собранию напрямую.</span><span class="sxs-lookup"><span data-stu-id="0d022-188">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="0d022-189">Анонимные пользователи ждут ожидания в зале ожидания.</span><span class="sxs-lookup"><span data-stu-id="0d022-189">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="0d022-190">просматривающи</span><span class="sxs-lookup"><span data-stu-id="0d022-190">everyone</span></span> | <span data-ttu-id="0d022-191">Разрешен любой пользователь, что означает, что все пользователи (включая анонимных пользователей) могут присоединиться к собранию напрямую, не дожидаясь ожидания в "зале ожидания".</span><span class="sxs-lookup"><span data-stu-id="0d022-191">Any user is allowed, which means that everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="0d022-192">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d022-192">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "autoAdmittedUsers": "everyone | everyoneInSameAndFederatedCompany | everyoneInCompany | invitedUsersInCompany | organizer",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCanceled": false,
  "joinUrl": "String",
  "isBroadcast": false,
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "capabilities": [ "questionAndAnswer" ],
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
