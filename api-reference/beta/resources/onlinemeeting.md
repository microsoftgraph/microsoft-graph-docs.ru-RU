---
title: Тип ресурса Онлинемитинг
description: Содержит сведения о собрании, включая URL-адрес присоединения, список участников и описание.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 888b5d7d60a72ed95cb3e3f6cbb1b6e5407919ab
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962368"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="ec137-103">Тип ресурса Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="ec137-103">onlineMeeting resource type</span></span>

<span data-ttu-id="ec137-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec137-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec137-105">Содержит сведения о собрании, включая URL-адрес, используемый для присоединения к собранию, список участников и описание.</span><span class="sxs-lookup"><span data-stu-id="ec137-105">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="ec137-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ec137-106">Methods</span></span>

| <span data-ttu-id="ec137-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ec137-107">Method</span></span>         | <span data-ttu-id="ec137-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ec137-108">Return Type</span></span> | <span data-ttu-id="ec137-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ec137-109">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="ec137-110">Создание объекта onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ec137-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="ec137-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ec137-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="ec137-112">Создайте собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="ec137-112">Create an online meeting.</span></span> |
| [<span data-ttu-id="ec137-113">Получение Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="ec137-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="ec137-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ec137-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="ec137-115">Чтение свойств и связей объекта **онлинемитинг** .</span><span class="sxs-lookup"><span data-stu-id="ec137-115">Read the properties and relationships of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="ec137-116">Создание или получение Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="ec137-116">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="ec137-117">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ec137-117">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="ec137-118">Создайте собрание по сети с пользовательским внешним ИДЕНТИФИКАТОРом.</span><span class="sxs-lookup"><span data-stu-id="ec137-118">Create an online meeting with a custom, external ID.</span></span> <span data-ttu-id="ec137-119">Если собрание уже существует, извлеките его значение.</span><span class="sxs-lookup"><span data-stu-id="ec137-119">If the meeting already exists, retrieve its propertie.</span></span> |

## <a name="properties"></a><span data-ttu-id="ec137-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec137-120">Properties</span></span>

| <span data-ttu-id="ec137-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec137-121">Property</span></span>                  | <span data-ttu-id="ec137-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ec137-122">Type</span></span>                                                   | <span data-ttu-id="ec137-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ec137-123">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ec137-124">аутоадмиттедусерс</span><span class="sxs-lookup"><span data-stu-id="ec137-124">autoAdmittedUsers</span></span>         | <span data-ttu-id="ec137-125">String</span><span class="sxs-lookup"><span data-stu-id="ec137-125">String</span></span>                                                 | <span data-ttu-id="ec137-126">Параметр, указывающий тип участников, которые будут автоматически разрешены в собрании по сети.</span><span class="sxs-lookup"><span data-stu-id="ec137-126">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="ec137-127">Возможные значения: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span><span class="sxs-lookup"><span data-stu-id="ec137-127">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span></span> <span data-ttu-id="ec137-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec137-128">Read-only.</span></span>|
| <span data-ttu-id="ec137-129">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="ec137-129">audioConferencing</span></span>         | [<span data-ttu-id="ec137-130">аудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="ec137-130">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="ec137-131">Сведения о телефонном доступе (телефонное подключение) для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="ec137-131">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="ec137-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec137-132">Read-only.</span></span> |
| <span data-ttu-id="ec137-133">chatInfo</span><span class="sxs-lookup"><span data-stu-id="ec137-133">chatInfo</span></span>                  | [<span data-ttu-id="ec137-134">chatInfo</span><span class="sxs-lookup"><span data-stu-id="ec137-134">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="ec137-135">Сведения о чате, связанные с этим собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="ec137-135">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="ec137-136">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="ec137-136">creationDateTime</span></span>          | <span data-ttu-id="ec137-137">DateTime</span><span class="sxs-lookup"><span data-stu-id="ec137-137">DateTime</span></span>                                               | <span data-ttu-id="ec137-138">Время создания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="ec137-138">The meeting creation time in UTC.</span></span> <span data-ttu-id="ec137-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec137-139">Read-only.</span></span> |
| <span data-ttu-id="ec137-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ec137-140">startDateTime</span></span>             | <span data-ttu-id="ec137-141">DateTime</span><span class="sxs-lookup"><span data-stu-id="ec137-141">DateTime</span></span>                                               | <span data-ttu-id="ec137-142">Время начала собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="ec137-142">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="ec137-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ec137-143">endDateTime</span></span>               | <span data-ttu-id="ec137-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="ec137-144">DateTime</span></span>                                               | <span data-ttu-id="ec137-145">Время окончания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="ec137-145">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="ec137-146">id</span><span class="sxs-lookup"><span data-stu-id="ec137-146">id</span></span>                        | <span data-ttu-id="ec137-147">Строка</span><span class="sxs-lookup"><span data-stu-id="ec137-147">String</span></span>                                                 | <span data-ttu-id="ec137-148">ИДЕНТИФИКАТОР по умолчанию, связанный с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="ec137-148">The default ID associated with the online meeting.</span></span> <span data-ttu-id="ec137-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec137-149">Read-only.</span></span> |
| <span data-ttu-id="ec137-150">жоинвебурл</span><span class="sxs-lookup"><span data-stu-id="ec137-150">joinWebUrl</span></span>                   | <span data-ttu-id="ec137-151">String</span><span class="sxs-lookup"><span data-stu-id="ec137-151">String</span></span>                                                 | <span data-ttu-id="ec137-152">URL-адрес присоединения к собранию по сети.</span><span class="sxs-lookup"><span data-stu-id="ec137-152">The join URL of the online meeting.</span></span> <span data-ttu-id="ec137-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec137-153">Read-only.</span></span>|
| <span data-ttu-id="ec137-154">participants</span><span class="sxs-lookup"><span data-stu-id="ec137-154">participants</span></span>              | [<span data-ttu-id="ec137-155">митингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="ec137-155">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="ec137-156">Участники, связанные с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="ec137-156">The participants associated with the online meeting.</span></span>  <span data-ttu-id="ec137-157">Сюда входят Организатор и участники.</span><span class="sxs-lookup"><span data-stu-id="ec137-157">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="ec137-158">subject</span><span class="sxs-lookup"><span data-stu-id="ec137-158">subject</span></span>                   | <span data-ttu-id="ec137-159">String</span><span class="sxs-lookup"><span data-stu-id="ec137-159">String</span></span>                                                 | <span data-ttu-id="ec137-160">Тема собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="ec137-160">The subject of the online meeting.</span></span> |
| <span data-ttu-id="ec137-161">capabilities</span><span class="sxs-lookup"><span data-stu-id="ec137-161">capabilities</span></span>              | <span data-ttu-id="ec137-162">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ec137-162">String collection</span></span>                                      | <span data-ttu-id="ec137-163">Список возможностей собрания.</span><span class="sxs-lookup"><span data-stu-id="ec137-163">The list of meeting capabilities.</span></span> <span data-ttu-id="ec137-164">Возможные значения: `questionAndAnswer`.</span><span class="sxs-lookup"><span data-stu-id="ec137-164">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="ec137-165">видеотелеконференцеид</span><span class="sxs-lookup"><span data-stu-id="ec137-165">videoTeleconferenceId</span></span>     | <span data-ttu-id="ec137-166">String</span><span class="sxs-lookup"><span data-stu-id="ec137-166">String</span></span>                                                 | <span data-ttu-id="ec137-167">Идентификатор видеоконференций для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="ec137-167">The video teleconferencing ID.</span></span> <span data-ttu-id="ec137-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec137-168">Read-only.</span></span> |
| <span data-ttu-id="ec137-169">externalId</span><span class="sxs-lookup"><span data-stu-id="ec137-169">externalId</span></span>                | <span data-ttu-id="ec137-170">String</span><span class="sxs-lookup"><span data-stu-id="ec137-170">String</span></span>                                                 | <span data-ttu-id="ec137-171">Внешний идентификатор.</span><span class="sxs-lookup"><span data-stu-id="ec137-171">The external ID.</span></span> <span data-ttu-id="ec137-172">Настраиваемый идентификатор.</span><span class="sxs-lookup"><span data-stu-id="ec137-172">A custom ID.</span></span> <span data-ttu-id="ec137-173">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ec137-173">Optional.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="ec137-174">значения Аутоадмиттедусерс</span><span class="sxs-lookup"><span data-stu-id="ec137-174">autoAdmittedUsers values</span></span>
| <span data-ttu-id="ec137-175">Значение</span><span class="sxs-lookup"><span data-stu-id="ec137-175">Value</span></span> | <span data-ttu-id="ec137-176">Описание</span><span class="sxs-lookup"><span data-stu-id="ec137-176">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ec137-177">organizer</span><span class="sxs-lookup"><span data-stu-id="ec137-177">organizer</span></span> | <span data-ttu-id="ec137-178">Только организатор собрания додается непосредственно.</span><span class="sxs-lookup"><span data-stu-id="ec137-178">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="ec137-179">Все остальные ожидают, пока организатор не выйдет.</span><span class="sxs-lookup"><span data-stu-id="ec137-179">Everyone else waits in the lobby, until admitted by the organizer</span></span>  |
| <span data-ttu-id="ec137-180">инвитедусерсинкомпани</span><span class="sxs-lookup"><span data-stu-id="ec137-180">invitedUsersInCompany</span></span> | <span data-ttu-id="ec137-181">Организатор собрания и пользователи в той же компании, приглашенные организатором, напрямую присоединяются к собранию.</span><span class="sxs-lookup"><span data-stu-id="ec137-181">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="ec137-182">Все остальные ожидают, пока не станет допущен.</span><span class="sxs-lookup"><span data-stu-id="ec137-182">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="ec137-183">еверйонеинкомпани</span><span class="sxs-lookup"><span data-stu-id="ec137-183">everyoneInCompany</span></span> | <span data-ttu-id="ec137-184">Все пользователи в той же организации, что и организатор, напрямую присоединяются к собранию.</span><span class="sxs-lookup"><span data-stu-id="ec137-184">Everyone in the same company as the organizer join the meeting directly.</span></span>  <span data-ttu-id="ec137-185">Федеративные анонимные пользователи ожидают, пока не допустить ожидания.</span><span class="sxs-lookup"><span data-stu-id="ec137-185">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="ec137-186">еверйонеинсамеандфедератедкомпани</span><span class="sxs-lookup"><span data-stu-id="ec137-186">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="ec137-187">Все пользователи в той же организации, что и организатор и Федеративные компании, присоединяются к собранию напрямую.</span><span class="sxs-lookup"><span data-stu-id="ec137-187">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="ec137-188">Анонимные пользователи ждут ожидания в зале ожидания.</span><span class="sxs-lookup"><span data-stu-id="ec137-188">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="ec137-189">просматривающи</span><span class="sxs-lookup"><span data-stu-id="ec137-189">everyone</span></span> | <span data-ttu-id="ec137-190">Разрешен любой пользователь, что означает, что все пользователи (включая анонимных пользователей) могут присоединиться к собранию напрямую, не дожидаясь ожидания в "зале ожидания".</span><span class="sxs-lookup"><span data-stu-id="ec137-190">Any user is allowed, which means that everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="ec137-191">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ec137-191">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "externalId"
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
