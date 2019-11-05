---
title: Тип ресурса Онлинемитинг
description: Сбор сведений о собрании, в том числе URL-адреса присоединения, списка участников и описания.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-cloud communications
doc_type: resourcePageType
ms.openlocfilehash: 5cc62c4caa564aa071ffc6b206d5494814b0cb53
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37969803"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="916fb-103">Тип ресурса Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="916fb-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="916fb-104">Содержит сведения о собрании, включая URL-адрес присоединения, список участников и описание.</span><span class="sxs-lookup"><span data-stu-id="916fb-104">Contains information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="916fb-105">Методы</span><span class="sxs-lookup"><span data-stu-id="916fb-105">Methods</span></span>

| <span data-ttu-id="916fb-106">Метод</span><span class="sxs-lookup"><span data-stu-id="916fb-106">Method</span></span>         | <span data-ttu-id="916fb-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="916fb-107">Return Type</span></span> | <span data-ttu-id="916fb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="916fb-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="916fb-109">Создание Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="916fb-109">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="916fb-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="916fb-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="916fb-111">Создайте собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="916fb-111">Create an online meeting.</span></span> |
| [<span data-ttu-id="916fb-112">Получение Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="916fb-112">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="916fb-113">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="916fb-113">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="916fb-114">Чтение свойств и связей объекта **онлинемитинг** .</span><span class="sxs-lookup"><span data-stu-id="916fb-114">Read the properties and relationships of an **onlineMeeting** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="916fb-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="916fb-115">Properties</span></span>

| <span data-ttu-id="916fb-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="916fb-116">Property</span></span>                  | <span data-ttu-id="916fb-117">Тип</span><span class="sxs-lookup"><span data-stu-id="916fb-117">Type</span></span>                                                   | <span data-ttu-id="916fb-118">Описание</span><span class="sxs-lookup"><span data-stu-id="916fb-118">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="916fb-119">аутоадмиттедусерс</span><span class="sxs-lookup"><span data-stu-id="916fb-119">autoAdmittedUsers</span></span>         | <span data-ttu-id="916fb-120">String</span><span class="sxs-lookup"><span data-stu-id="916fb-120">String</span></span>                                                 | <span data-ttu-id="916fb-121">Параметр, указывающий тип участников, которые будут автоматически разрешены в собрании по сети.</span><span class="sxs-lookup"><span data-stu-id="916fb-121">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="916fb-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="916fb-122">Read-only.</span></span> <span data-ttu-id="916fb-123">`everyone`Возможные значения: `everyoneInSameAndFederatedCompany`,, `everyoneInCompany`,, `invitedUsersInCompany``organizer`</span><span class="sxs-lookup"><span data-stu-id="916fb-123">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`</span></span>|
| <span data-ttu-id="916fb-124">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="916fb-124">audioConferencing</span></span>         | [<span data-ttu-id="916fb-125">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="916fb-125">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="916fb-126">Сведения о телефонном доступе (телефонное подключение) для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="916fb-126">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="916fb-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="916fb-127">Read-only.</span></span> |
| <span data-ttu-id="916fb-128">канцеледдатетиме</span><span class="sxs-lookup"><span data-stu-id="916fb-128">canceledDateTime</span></span>          | <span data-ttu-id="916fb-129">DateTime</span><span class="sxs-lookup"><span data-stu-id="916fb-129">DateTime</span></span>                                               | <span data-ttu-id="916fb-130">Время в формате UTC, когда собрание было отменено.</span><span class="sxs-lookup"><span data-stu-id="916fb-130">The time in UTC when the meeting was canceled.</span></span> <span data-ttu-id="916fb-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="916fb-131">Read-only.</span></span> |
| <span data-ttu-id="916fb-132">chatInfo</span><span class="sxs-lookup"><span data-stu-id="916fb-132">chatInfo</span></span>                  | [<span data-ttu-id="916fb-133">chatInfo</span><span class="sxs-lookup"><span data-stu-id="916fb-133">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="916fb-134">Сведения о чате, связанные с этим собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="916fb-134">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="916fb-135">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="916fb-135">creationDateTime</span></span>          | <span data-ttu-id="916fb-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="916fb-136">DateTime</span></span>                                               | <span data-ttu-id="916fb-137">Время создания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="916fb-137">The meeting creation time in UTC.</span></span> <span data-ttu-id="916fb-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="916fb-138">Read-only.</span></span> |
| <span data-ttu-id="916fb-139">startDateTime</span><span class="sxs-lookup"><span data-stu-id="916fb-139">startDateTime</span></span>             | <span data-ttu-id="916fb-140">DateTime</span><span class="sxs-lookup"><span data-stu-id="916fb-140">DateTime</span></span>                                               | <span data-ttu-id="916fb-141">Время начала собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="916fb-141">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="916fb-142">endDateTime</span><span class="sxs-lookup"><span data-stu-id="916fb-142">endDateTime</span></span>               | <span data-ttu-id="916fb-143">DateTime</span><span class="sxs-lookup"><span data-stu-id="916fb-143">DateTime</span></span>                                               | <span data-ttu-id="916fb-144">Время окончания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="916fb-144">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="916fb-145">id</span><span class="sxs-lookup"><span data-stu-id="916fb-145">id</span></span>                        | <span data-ttu-id="916fb-146">Строка</span><span class="sxs-lookup"><span data-stu-id="916fb-146">String</span></span>                                                 | <span data-ttu-id="916fb-147">ИДЕНТИФИКАТОР по умолчанию, связанный с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="916fb-147">The default ID associated with the online meeting.</span></span> <span data-ttu-id="916fb-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="916fb-148">Read-only.</span></span> |
| <span data-ttu-id="916fb-149">Отменено</span><span class="sxs-lookup"><span data-stu-id="916fb-149">isCanceled</span></span>                | <span data-ttu-id="916fb-150">Логический</span><span class="sxs-lookup"><span data-stu-id="916fb-150">Boolean</span></span>                                                | <span data-ttu-id="916fb-151">Указывает, было ли собрание отменено.</span><span class="sxs-lookup"><span data-stu-id="916fb-151">Indicates whether the meeting has been canceled.</span></span> <span data-ttu-id="916fb-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="916fb-152">Read-only.</span></span> |
| <span data-ttu-id="916fb-153">жоинурл</span><span class="sxs-lookup"><span data-stu-id="916fb-153">joinUrl</span></span>                   | <span data-ttu-id="916fb-154">String</span><span class="sxs-lookup"><span data-stu-id="916fb-154">String</span></span>                                                 | <span data-ttu-id="916fb-155">URL-адрес присоединения к собранию по сети.</span><span class="sxs-lookup"><span data-stu-id="916fb-155">The join URL of the online meeting.</span></span> <span data-ttu-id="916fb-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="916fb-156">Read-only.</span></span>|
| <span data-ttu-id="916fb-157">Передача</span><span class="sxs-lookup"><span data-stu-id="916fb-157">isBroadcast</span></span>               | <span data-ttu-id="916fb-158">Логический</span><span class="sxs-lookup"><span data-stu-id="916fb-158">Boolean</span></span>                                                | <span data-ttu-id="916fb-159">Флаг, определяющий, является ли собрание широковещательным.</span><span class="sxs-lookup"><span data-stu-id="916fb-159">The flag to determine whether it's a broadcast meeting.</span></span> |
| <span data-ttu-id="916fb-160">participants</span><span class="sxs-lookup"><span data-stu-id="916fb-160">participants</span></span>              | [<span data-ttu-id="916fb-161">митингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="916fb-161">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="916fb-162">Участники, связанные с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="916fb-162">The participants associated with the online meeting.</span></span>  <span data-ttu-id="916fb-163">Сюда входят Организатор и участники.</span><span class="sxs-lookup"><span data-stu-id="916fb-163">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="916fb-164">subject</span><span class="sxs-lookup"><span data-stu-id="916fb-164">subject</span></span>                   | <span data-ttu-id="916fb-165">String</span><span class="sxs-lookup"><span data-stu-id="916fb-165">String</span></span>                                                 | <span data-ttu-id="916fb-166">Тема собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="916fb-166">The subject of the online meeting.</span></span> |
| <span data-ttu-id="916fb-167">capabilities</span><span class="sxs-lookup"><span data-stu-id="916fb-167">capabilities</span></span>              | <span data-ttu-id="916fb-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="916fb-168">String collection</span></span>                                      | <span data-ttu-id="916fb-169">Список возможностей собрания.</span><span class="sxs-lookup"><span data-stu-id="916fb-169">The list of meeting capabilities.</span></span> <span data-ttu-id="916fb-170">Возможные значения: `questionAndAnswer`.</span><span class="sxs-lookup"><span data-stu-id="916fb-170">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="916fb-171">видеотелеконференцеид</span><span class="sxs-lookup"><span data-stu-id="916fb-171">videoTeleconferenceId</span></span>     | <span data-ttu-id="916fb-172">String</span><span class="sxs-lookup"><span data-stu-id="916fb-172">String</span></span>                                                 | <span data-ttu-id="916fb-173">Идентификатор телеконференций видеио.</span><span class="sxs-lookup"><span data-stu-id="916fb-173">The videio teleconferencing ID.</span></span> <span data-ttu-id="916fb-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="916fb-174">Read-only.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="916fb-175">значения Аутоадмиттедусерс</span><span class="sxs-lookup"><span data-stu-id="916fb-175">autoAdmittedUsers values</span></span>
| <span data-ttu-id="916fb-176">Значение</span><span class="sxs-lookup"><span data-stu-id="916fb-176">Value</span></span> | <span data-ttu-id="916fb-177">Описание</span><span class="sxs-lookup"><span data-stu-id="916fb-177">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="916fb-178">organizer</span><span class="sxs-lookup"><span data-stu-id="916fb-178">organizer</span></span> | <span data-ttu-id="916fb-179">Только организатор собрания додается непосредственно.</span><span class="sxs-lookup"><span data-stu-id="916fb-179">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="916fb-180">Все остальные ожидают, пока организатор не выйдет в "зале ожидания".</span><span class="sxs-lookup"><span data-stu-id="916fb-180">Everyone else waits in the lobby, until admitted by the organizer.</span></span>  |
| <span data-ttu-id="916fb-181">инвитедусерсинкомпани</span><span class="sxs-lookup"><span data-stu-id="916fb-181">invitedUsersInCompany</span></span> | <span data-ttu-id="916fb-182">Организатор собрания и пользователи в той же компании, приглашенные организатором, напрямую присоединяются к собранию.</span><span class="sxs-lookup"><span data-stu-id="916fb-182">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="916fb-183">Все остальные ожидают, пока не станет допущен.</span><span class="sxs-lookup"><span data-stu-id="916fb-183">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="916fb-184">еверйонеинкомпани</span><span class="sxs-lookup"><span data-stu-id="916fb-184">everyoneInCompany</span></span> | <span data-ttu-id="916fb-185">Все пользователи в той же организации, что и организатор, напрямую присоединяются к собранию.</span><span class="sxs-lookup"><span data-stu-id="916fb-185">Everyone in the same company as the organizer join the meeting directly.</span></span> <span data-ttu-id="916fb-186">Федеративные анонимные пользователи ожидают, пока не допустить ожидания.</span><span class="sxs-lookup"><span data-stu-id="916fb-186">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="916fb-187">еверйонеинсамеандфедератедкомпани</span><span class="sxs-lookup"><span data-stu-id="916fb-187">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="916fb-188">Все пользователи в той же организации, что и организатор и Федеративные компании, присоединяются к собранию напрямую.</span><span class="sxs-lookup"><span data-stu-id="916fb-188">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="916fb-189">Анонимные пользователи ждут ожидания в зале ожидания.</span><span class="sxs-lookup"><span data-stu-id="916fb-189">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="916fb-190">просматривающи</span><span class="sxs-lookup"><span data-stu-id="916fb-190">everyone</span></span> | <span data-ttu-id="916fb-191">Разрешен любой пользователь.</span><span class="sxs-lookup"><span data-stu-id="916fb-191">Any user is allowed.</span></span> <span data-ttu-id="916fb-192">Все пользователи (включая анонимных пользователей) могут присоединяться к собранию напрямую, не дожидаясь ожидания в "зале ожидания".</span><span class="sxs-lookup"><span data-stu-id="916fb-192">Everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="916fb-193">Связи</span><span class="sxs-lookup"><span data-stu-id="916fb-193">Relationships</span></span>
<span data-ttu-id="916fb-194">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="916fb-194">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="916fb-195">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="916fb-195">JSON representation</span></span>

<span data-ttu-id="916fb-196">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="916fb-196">The following is a JSON representation of the resource.</span></span>

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
