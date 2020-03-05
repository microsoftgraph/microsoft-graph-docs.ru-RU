---
title: Тип ресурса Онлинемитинг
description: Содержит сведения о собрании, включая URL-адрес присоединения, список участников и описание.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: b6e0848b88427cf0929030f07b163204842c3cd7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522258"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="81dfd-103">Тип ресурса Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="81dfd-103">onlineMeeting resource type</span></span>

<span data-ttu-id="81dfd-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="81dfd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81dfd-105">Содержит сведения о собрании, включая URL-адрес, используемый для присоединения к собранию, список участников и описание.</span><span class="sxs-lookup"><span data-stu-id="81dfd-105">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="81dfd-106">Методы</span><span class="sxs-lookup"><span data-stu-id="81dfd-106">Methods</span></span>

| <span data-ttu-id="81dfd-107">Метод</span><span class="sxs-lookup"><span data-stu-id="81dfd-107">Method</span></span>         | <span data-ttu-id="81dfd-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="81dfd-108">Return Type</span></span> | <span data-ttu-id="81dfd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="81dfd-109">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="81dfd-110">Создание объекта onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="81dfd-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="81dfd-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="81dfd-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="81dfd-112">Создайте собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="81dfd-112">Create an online meeting.</span></span> |
| [<span data-ttu-id="81dfd-113">Получение Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="81dfd-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="81dfd-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="81dfd-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="81dfd-115">Чтение свойств и связей объекта **онлинемитинг** .</span><span class="sxs-lookup"><span data-stu-id="81dfd-115">Read the properties and relationships of an **onlineMeeting** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="81dfd-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="81dfd-116">Properties</span></span>

| <span data-ttu-id="81dfd-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="81dfd-117">Property</span></span>                  | <span data-ttu-id="81dfd-118">Тип</span><span class="sxs-lookup"><span data-stu-id="81dfd-118">Type</span></span>                                                   | <span data-ttu-id="81dfd-119">Описание</span><span class="sxs-lookup"><span data-stu-id="81dfd-119">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="81dfd-120">аутоадмиттедусерс</span><span class="sxs-lookup"><span data-stu-id="81dfd-120">autoAdmittedUsers</span></span>         | <span data-ttu-id="81dfd-121">String</span><span class="sxs-lookup"><span data-stu-id="81dfd-121">String</span></span>                                                 | <span data-ttu-id="81dfd-122">Параметр, указывающий тип участников, которые будут автоматически разрешены в собрании по сети.</span><span class="sxs-lookup"><span data-stu-id="81dfd-122">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="81dfd-123">Возможные значения: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span><span class="sxs-lookup"><span data-stu-id="81dfd-123">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span></span> <span data-ttu-id="81dfd-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81dfd-124">Read-only.</span></span>|
| <span data-ttu-id="81dfd-125">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="81dfd-125">audioConferencing</span></span>         | [<span data-ttu-id="81dfd-126">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="81dfd-126">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="81dfd-127">Сведения о телефонном доступе (телефонное подключение) для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="81dfd-127">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="81dfd-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81dfd-128">Read-only.</span></span> |
| <span data-ttu-id="81dfd-129">chatInfo</span><span class="sxs-lookup"><span data-stu-id="81dfd-129">chatInfo</span></span>                  | [<span data-ttu-id="81dfd-130">chatInfo</span><span class="sxs-lookup"><span data-stu-id="81dfd-130">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="81dfd-131">Сведения о чате, связанные с этим собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="81dfd-131">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="81dfd-132">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="81dfd-132">creationDateTime</span></span>          | <span data-ttu-id="81dfd-133">DateTime</span><span class="sxs-lookup"><span data-stu-id="81dfd-133">DateTime</span></span>                                               | <span data-ttu-id="81dfd-134">Время создания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="81dfd-134">The meeting creation time in UTC.</span></span> <span data-ttu-id="81dfd-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81dfd-135">Read-only.</span></span> |
| <span data-ttu-id="81dfd-136">startDateTime</span><span class="sxs-lookup"><span data-stu-id="81dfd-136">startDateTime</span></span>             | <span data-ttu-id="81dfd-137">DateTime</span><span class="sxs-lookup"><span data-stu-id="81dfd-137">DateTime</span></span>                                               | <span data-ttu-id="81dfd-138">Время начала собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="81dfd-138">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="81dfd-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="81dfd-139">endDateTime</span></span>               | <span data-ttu-id="81dfd-140">DateTime</span><span class="sxs-lookup"><span data-stu-id="81dfd-140">DateTime</span></span>                                               | <span data-ttu-id="81dfd-141">Время окончания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="81dfd-141">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="81dfd-142">id</span><span class="sxs-lookup"><span data-stu-id="81dfd-142">id</span></span>                        | <span data-ttu-id="81dfd-143">Строка</span><span class="sxs-lookup"><span data-stu-id="81dfd-143">String</span></span>                                                 | <span data-ttu-id="81dfd-144">ИДЕНТИФИКАТОР по умолчанию, связанный с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="81dfd-144">The default ID associated with the online meeting.</span></span> <span data-ttu-id="81dfd-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81dfd-145">Read-only.</span></span> |
| <span data-ttu-id="81dfd-146">жоинвебурл</span><span class="sxs-lookup"><span data-stu-id="81dfd-146">joinWebUrl</span></span>                   | <span data-ttu-id="81dfd-147">String</span><span class="sxs-lookup"><span data-stu-id="81dfd-147">String</span></span>                                                 | <span data-ttu-id="81dfd-148">URL-адрес присоединения к собранию по сети.</span><span class="sxs-lookup"><span data-stu-id="81dfd-148">The join URL of the online meeting.</span></span> <span data-ttu-id="81dfd-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81dfd-149">Read-only.</span></span>|
| <span data-ttu-id="81dfd-150">participants</span><span class="sxs-lookup"><span data-stu-id="81dfd-150">participants</span></span>              | [<span data-ttu-id="81dfd-151">митингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="81dfd-151">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="81dfd-152">Участники, связанные с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="81dfd-152">The participants associated with the online meeting.</span></span>  <span data-ttu-id="81dfd-153">Сюда входят Организатор и участники.</span><span class="sxs-lookup"><span data-stu-id="81dfd-153">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="81dfd-154">subject</span><span class="sxs-lookup"><span data-stu-id="81dfd-154">subject</span></span>                   | <span data-ttu-id="81dfd-155">String</span><span class="sxs-lookup"><span data-stu-id="81dfd-155">String</span></span>                                                 | <span data-ttu-id="81dfd-156">Тема собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="81dfd-156">The subject of the online meeting.</span></span> |
| <span data-ttu-id="81dfd-157">capabilities</span><span class="sxs-lookup"><span data-stu-id="81dfd-157">capabilities</span></span>              | <span data-ttu-id="81dfd-158">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="81dfd-158">String collection</span></span>                                      | <span data-ttu-id="81dfd-159">Список возможностей собрания.</span><span class="sxs-lookup"><span data-stu-id="81dfd-159">The list of meeting capabilities.</span></span> <span data-ttu-id="81dfd-160">Возможные значения: `questionAndAnswer`.</span><span class="sxs-lookup"><span data-stu-id="81dfd-160">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="81dfd-161">видеотелеконференцеид</span><span class="sxs-lookup"><span data-stu-id="81dfd-161">videoTeleconferenceId</span></span>     | <span data-ttu-id="81dfd-162">String</span><span class="sxs-lookup"><span data-stu-id="81dfd-162">String</span></span>                                                 | <span data-ttu-id="81dfd-163">Идентификатор видеоконференций для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="81dfd-163">The video teleconferencing ID.</span></span> <span data-ttu-id="81dfd-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81dfd-164">Read-only.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="81dfd-165">значения Аутоадмиттедусерс</span><span class="sxs-lookup"><span data-stu-id="81dfd-165">autoAdmittedUsers values</span></span>
| <span data-ttu-id="81dfd-166">Значение</span><span class="sxs-lookup"><span data-stu-id="81dfd-166">Value</span></span> | <span data-ttu-id="81dfd-167">Описание</span><span class="sxs-lookup"><span data-stu-id="81dfd-167">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="81dfd-168">organizer</span><span class="sxs-lookup"><span data-stu-id="81dfd-168">organizer</span></span> | <span data-ttu-id="81dfd-169">Только организатор собрания додается непосредственно.</span><span class="sxs-lookup"><span data-stu-id="81dfd-169">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="81dfd-170">Все остальные ожидают, пока организатор не выйдет.</span><span class="sxs-lookup"><span data-stu-id="81dfd-170">Everyone else waits in the lobby, until admitted by the organizer</span></span>  |
| <span data-ttu-id="81dfd-171">инвитедусерсинкомпани</span><span class="sxs-lookup"><span data-stu-id="81dfd-171">invitedUsersInCompany</span></span> | <span data-ttu-id="81dfd-172">Организатор собрания и пользователи в той же компании, приглашенные организатором, напрямую присоединяются к собранию.</span><span class="sxs-lookup"><span data-stu-id="81dfd-172">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="81dfd-173">Все остальные ожидают, пока не станет допущен.</span><span class="sxs-lookup"><span data-stu-id="81dfd-173">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="81dfd-174">еверйонеинкомпани</span><span class="sxs-lookup"><span data-stu-id="81dfd-174">everyoneInCompany</span></span> | <span data-ttu-id="81dfd-175">Все пользователи в той же организации, что и организатор, напрямую присоединяются к собранию.</span><span class="sxs-lookup"><span data-stu-id="81dfd-175">Everyone in the same company as the organizer join the meeting directly.</span></span>  <span data-ttu-id="81dfd-176">Федеративные анонимные пользователи ожидают, пока не допустить ожидания.</span><span class="sxs-lookup"><span data-stu-id="81dfd-176">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="81dfd-177">еверйонеинсамеандфедератедкомпани</span><span class="sxs-lookup"><span data-stu-id="81dfd-177">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="81dfd-178">Все пользователи в той же организации, что и организатор и Федеративные компании, присоединяются к собранию напрямую.</span><span class="sxs-lookup"><span data-stu-id="81dfd-178">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="81dfd-179">Анонимные пользователи ждут ожидания в зале ожидания.</span><span class="sxs-lookup"><span data-stu-id="81dfd-179">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="81dfd-180">просматривающи</span><span class="sxs-lookup"><span data-stu-id="81dfd-180">everyone</span></span> | <span data-ttu-id="81dfd-181">Разрешен любой пользователь, что означает, что все пользователи (включая анонимных пользователей) могут присоединиться к собранию напрямую, не дожидаясь ожидания в "зале ожидания".</span><span class="sxs-lookup"><span data-stu-id="81dfd-181">Any user is allowed, which means that everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="81dfd-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81dfd-182">JSON representation</span></span>

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
