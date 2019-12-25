---
title: Тип ресурса Онлинемитинг
description: Содержит сведения о собрании, включая URL-адрес присоединения, список участников и описание.
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: e7cae71f220a2a519908e3af890029a2da555577
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866688"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="6ad8b-103">Тип ресурса Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="6ad8b-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ad8b-104">Содержит сведения о собрании, включая URL-адрес, используемый для присоединения к собранию, список участников и описание.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-104">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="6ad8b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="6ad8b-105">Methods</span></span>

| <span data-ttu-id="6ad8b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="6ad8b-106">Method</span></span>         | <span data-ttu-id="6ad8b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6ad8b-107">Return Type</span></span> | <span data-ttu-id="6ad8b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6ad8b-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="6ad8b-109">Создание Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="6ad8b-109">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="6ad8b-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="6ad8b-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="6ad8b-111">Создайте собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-111">Create an online meeting.</span></span> |
| [<span data-ttu-id="6ad8b-112">Получение Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="6ad8b-112">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="6ad8b-113">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="6ad8b-113">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="6ad8b-114">Чтение свойств и связей объекта **онлинемитинг** .</span><span class="sxs-lookup"><span data-stu-id="6ad8b-114">Read the properties and relationships of an **onlineMeeting** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6ad8b-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ad8b-115">Properties</span></span>

| <span data-ttu-id="6ad8b-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ad8b-116">Property</span></span>                  | <span data-ttu-id="6ad8b-117">Тип</span><span class="sxs-lookup"><span data-stu-id="6ad8b-117">Type</span></span>                                                   | <span data-ttu-id="6ad8b-118">Описание</span><span class="sxs-lookup"><span data-stu-id="6ad8b-118">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6ad8b-119">аутоадмиттедусерс</span><span class="sxs-lookup"><span data-stu-id="6ad8b-119">autoAdmittedUsers</span></span>         | <span data-ttu-id="6ad8b-120">String</span><span class="sxs-lookup"><span data-stu-id="6ad8b-120">String</span></span>                                                 | <span data-ttu-id="6ad8b-121">Параметр, указывающий тип участников, которые будут автоматически разрешены в собрании по сети.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-121">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="6ad8b-122">Возможные значения: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-122">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span></span> <span data-ttu-id="6ad8b-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-123">Read-only.</span></span>|
| <span data-ttu-id="6ad8b-124">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="6ad8b-124">audioConferencing</span></span>         | [<span data-ttu-id="6ad8b-125">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="6ad8b-125">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="6ad8b-126">Сведения о телефонном доступе (телефонное подключение) для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-126">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="6ad8b-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-127">Read-only.</span></span> |
| <span data-ttu-id="6ad8b-128">chatInfo</span><span class="sxs-lookup"><span data-stu-id="6ad8b-128">chatInfo</span></span>                  | [<span data-ttu-id="6ad8b-129">chatInfo</span><span class="sxs-lookup"><span data-stu-id="6ad8b-129">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="6ad8b-130">Сведения о чате, связанные с этим собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-130">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="6ad8b-131">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="6ad8b-131">creationDateTime</span></span>          | <span data-ttu-id="6ad8b-132">DateTime</span><span class="sxs-lookup"><span data-stu-id="6ad8b-132">DateTime</span></span>                                               | <span data-ttu-id="6ad8b-133">Время создания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-133">The meeting creation time in UTC.</span></span> <span data-ttu-id="6ad8b-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-134">Read-only.</span></span> |
| <span data-ttu-id="6ad8b-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6ad8b-135">startDateTime</span></span>             | <span data-ttu-id="6ad8b-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="6ad8b-136">DateTime</span></span>                                               | <span data-ttu-id="6ad8b-137">Время начала собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-137">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="6ad8b-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6ad8b-138">endDateTime</span></span>               | <span data-ttu-id="6ad8b-139">DateTime</span><span class="sxs-lookup"><span data-stu-id="6ad8b-139">DateTime</span></span>                                               | <span data-ttu-id="6ad8b-140">Время окончания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-140">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="6ad8b-141">id</span><span class="sxs-lookup"><span data-stu-id="6ad8b-141">id</span></span>                        | <span data-ttu-id="6ad8b-142">Строка</span><span class="sxs-lookup"><span data-stu-id="6ad8b-142">String</span></span>                                                 | <span data-ttu-id="6ad8b-143">ИДЕНТИФИКАТОР по умолчанию, связанный с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-143">The default ID associated with the online meeting.</span></span> <span data-ttu-id="6ad8b-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-144">Read-only.</span></span> |
| <span data-ttu-id="6ad8b-145">жоинвебурл</span><span class="sxs-lookup"><span data-stu-id="6ad8b-145">joinWebUrl</span></span>                   | <span data-ttu-id="6ad8b-146">String</span><span class="sxs-lookup"><span data-stu-id="6ad8b-146">String</span></span>                                                 | <span data-ttu-id="6ad8b-147">URL-адрес присоединения к собранию по сети.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-147">The join URL of the online meeting.</span></span> <span data-ttu-id="6ad8b-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-148">Read-only.</span></span>|
| <span data-ttu-id="6ad8b-149">participants</span><span class="sxs-lookup"><span data-stu-id="6ad8b-149">participants</span></span>              | [<span data-ttu-id="6ad8b-150">митингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="6ad8b-150">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="6ad8b-151">Участники, связанные с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-151">The participants associated with the online meeting.</span></span>  <span data-ttu-id="6ad8b-152">Сюда входят Организатор и участники.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-152">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="6ad8b-153">subject</span><span class="sxs-lookup"><span data-stu-id="6ad8b-153">subject</span></span>                   | <span data-ttu-id="6ad8b-154">String</span><span class="sxs-lookup"><span data-stu-id="6ad8b-154">String</span></span>                                                 | <span data-ttu-id="6ad8b-155">Тема собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-155">The subject of the online meeting.</span></span> |
| <span data-ttu-id="6ad8b-156">capabilities</span><span class="sxs-lookup"><span data-stu-id="6ad8b-156">capabilities</span></span>              | <span data-ttu-id="6ad8b-157">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6ad8b-157">String collection</span></span>                                      | <span data-ttu-id="6ad8b-158">Список возможностей собрания.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-158">The list of meeting capabilities.</span></span> <span data-ttu-id="6ad8b-159">Возможные значения: `questionAndAnswer`.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-159">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="6ad8b-160">видеотелеконференцеид</span><span class="sxs-lookup"><span data-stu-id="6ad8b-160">videoTeleconferenceId</span></span>     | <span data-ttu-id="6ad8b-161">String</span><span class="sxs-lookup"><span data-stu-id="6ad8b-161">String</span></span>                                                 | <span data-ttu-id="6ad8b-162">Идентификатор видеоконференций для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-162">The video teleconferencing ID.</span></span> <span data-ttu-id="6ad8b-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-163">Read-only.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="6ad8b-164">значения Аутоадмиттедусерс</span><span class="sxs-lookup"><span data-stu-id="6ad8b-164">autoAdmittedUsers values</span></span>
| <span data-ttu-id="6ad8b-165">Значение</span><span class="sxs-lookup"><span data-stu-id="6ad8b-165">Value</span></span> | <span data-ttu-id="6ad8b-166">Описание</span><span class="sxs-lookup"><span data-stu-id="6ad8b-166">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6ad8b-167">organizer</span><span class="sxs-lookup"><span data-stu-id="6ad8b-167">organizer</span></span> | <span data-ttu-id="6ad8b-168">Только организатор собрания додается непосредственно.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-168">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="6ad8b-169">Все остальные ожидают, пока организатор не выйдет.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-169">Everyone else waits in the lobby, until admitted by the organizer</span></span>  |
| <span data-ttu-id="6ad8b-170">инвитедусерсинкомпани</span><span class="sxs-lookup"><span data-stu-id="6ad8b-170">invitedUsersInCompany</span></span> | <span data-ttu-id="6ad8b-171">Организатор собрания и пользователи в той же компании, приглашенные организатором, напрямую присоединяются к собранию.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-171">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="6ad8b-172">Все остальные ожидают, пока не станет допущен.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-172">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="6ad8b-173">еверйонеинкомпани</span><span class="sxs-lookup"><span data-stu-id="6ad8b-173">everyoneInCompany</span></span> | <span data-ttu-id="6ad8b-174">Все пользователи в той же организации, что и организатор, напрямую присоединяются к собранию.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-174">Everyone in the same company as the organizer join the meeting directly.</span></span>  <span data-ttu-id="6ad8b-175">Федеративные анонимные пользователи ожидают, пока не допустить ожидания.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-175">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="6ad8b-176">еверйонеинсамеандфедератедкомпани</span><span class="sxs-lookup"><span data-stu-id="6ad8b-176">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="6ad8b-177">Все пользователи в той же организации, что и организатор и Федеративные компании, присоединяются к собранию напрямую.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-177">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="6ad8b-178">Анонимные пользователи ждут ожидания в зале ожидания.</span><span class="sxs-lookup"><span data-stu-id="6ad8b-178">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="6ad8b-179">просматривающи</span><span class="sxs-lookup"><span data-stu-id="6ad8b-179">everyone</span></span> | <span data-ttu-id="6ad8b-180">Разрешен любой пользователь, что означает, что все пользователи (включая анонимных пользователей) могут присоединиться к собранию напрямую, не дожидаясь ожидания в "зале ожидания".</span><span class="sxs-lookup"><span data-stu-id="6ad8b-180">Any user is allowed, which means that everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="6ad8b-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ad8b-181">JSON representation</span></span>

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
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
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
