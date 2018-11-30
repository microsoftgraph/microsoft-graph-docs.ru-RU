---
title: Тип ресурса группы
description: 'Группы в группах Microsoft — это коллекция каналов. '
ms.openlocfilehash: 5ebb4dbc2c5913d69b69bdb244d8a7cfc83cec8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078915"
---
# <a name="team-resource-type"></a><span data-ttu-id="15b5c-103">Тип ресурса группы</span><span class="sxs-lookup"><span data-stu-id="15b5c-103">team resource type</span></span>

> <span data-ttu-id="15b5c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="15b5c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15b5c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15b5c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15b5c-106">Группы в группах Microsoft — это коллекция [каналов](channel.md).</span><span class="sxs-lookup"><span data-stu-id="15b5c-106">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="15b5c-107">Канал представляет раздел и логическая изоляции обсуждения в группе.</span><span class="sxs-lookup"><span data-stu-id="15b5c-107">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="15b5c-108">Для любой группы связан с [группы](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="15b5c-108">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="15b5c-109">Группа имеет тот же идентификатор, как команда — например, /groups/ {идентификатор} / team совпадает с /teams/ {идентификатор}.</span><span class="sxs-lookup"><span data-stu-id="15b5c-109">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="15b5c-110">Дополнительные сведения о работе с группами и участниками групп показано [Использование интерфейса API REST графическое представление Microsoft для работы с группами Майкрософт](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="15b5c-110">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="15b5c-111">Методы</span><span class="sxs-lookup"><span data-stu-id="15b5c-111">Methods</span></span>

| <span data-ttu-id="15b5c-112">Метод</span><span class="sxs-lookup"><span data-stu-id="15b5c-112">Method</span></span>       | <span data-ttu-id="15b5c-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="15b5c-113">Return Type</span></span>  |<span data-ttu-id="15b5c-114">Описание</span><span class="sxs-lookup"><span data-stu-id="15b5c-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="15b5c-115">Создание группы</span><span class="sxs-lookup"><span data-stu-id="15b5c-115">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="15b5c-116">Группа</span><span class="sxs-lookup"><span data-stu-id="15b5c-116">team</span></span>](team.md) | <span data-ttu-id="15b5c-117">Создание новой группы или добавление группы к существующей группе.</span><span class="sxs-lookup"><span data-stu-id="15b5c-117">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="15b5c-118">Получение группы</span><span class="sxs-lookup"><span data-stu-id="15b5c-118">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="15b5c-119">Группа</span><span class="sxs-lookup"><span data-stu-id="15b5c-119">team</span></span>](team.md) | <span data-ttu-id="15b5c-120">Извлечение свойств и связи из указанной группы.</span><span class="sxs-lookup"><span data-stu-id="15b5c-120">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="15b5c-121">Группа обновления</span><span class="sxs-lookup"><span data-stu-id="15b5c-121">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="15b5c-122">Группа</span><span class="sxs-lookup"><span data-stu-id="15b5c-122">team</span></span>](team.md) |<span data-ttu-id="15b5c-123">Обновление свойств указанной группы.</span><span class="sxs-lookup"><span data-stu-id="15b5c-123">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="15b5c-124">Удаление группы</span><span class="sxs-lookup"><span data-stu-id="15b5c-124">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="15b5c-125">Нет</span><span class="sxs-lookup"><span data-stu-id="15b5c-125">None</span></span> |<span data-ttu-id="15b5c-126">Удаление группы и его связанную группу.</span><span class="sxs-lookup"><span data-stu-id="15b5c-126">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="15b5c-127">Клонирование группы</span><span class="sxs-lookup"><span data-stu-id="15b5c-127">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="15b5c-128">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="15b5c-128">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="15b5c-129">Скопируйте группа и его связанную группу.</span><span class="sxs-lookup"><span data-stu-id="15b5c-129">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="15b5c-130">Группа архива</span><span class="sxs-lookup"><span data-stu-id="15b5c-130">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="15b5c-131">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="15b5c-131">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="15b5c-132">Поместите группа в состояние только для чтения.</span><span class="sxs-lookup"><span data-stu-id="15b5c-132">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="15b5c-133">Unarchive группы</span><span class="sxs-lookup"><span data-stu-id="15b5c-133">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="15b5c-134">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="15b5c-134">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="15b5c-135">Восстановите группа в состояние чтение запись.</span><span class="sxs-lookup"><span data-stu-id="15b5c-135">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="15b5c-136">Список рабочих групп</span><span class="sxs-lookup"><span data-stu-id="15b5c-136">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="15b5c-137">семейства сайтов [групп](team.md)</span><span class="sxs-lookup"><span data-stu-id="15b5c-137">[team](team.md) collection</span></span> | <span data-ttu-id="15b5c-138">Список групп, которые вы являетесь членом.</span><span class="sxs-lookup"><span data-stu-id="15b5c-138">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="15b5c-139">Список всех групп</span><span class="sxs-lookup"><span data-stu-id="15b5c-139">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="15b5c-140">Коллекция объектов [group](group.md)</span><span class="sxs-lookup"><span data-stu-id="15b5c-140">[group](group.md) collection</span></span> | <span data-ttu-id="15b5c-141">Список всех групп, которые имеют группами.</span><span class="sxs-lookup"><span data-stu-id="15b5c-141">List all groups that have teams.</span></span> |
|[<span data-ttu-id="15b5c-142">Публикация приложений для вашей организации</span><span class="sxs-lookup"><span data-stu-id="15b5c-142">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="15b5c-143">teamsApp</span><span class="sxs-lookup"><span data-stu-id="15b5c-143">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="15b5c-144">Создание групп приложений видимым только для вашей организации.</span><span class="sxs-lookup"><span data-stu-id="15b5c-144">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="15b5c-145">Добавление приложения в группу</span><span class="sxs-lookup"><span data-stu-id="15b5c-145">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="15b5c-146">teamsappinstallation</span><span class="sxs-lookup"><span data-stu-id="15b5c-146">teamsappinstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="15b5c-147">Добавляет (установить) приложения в группу.</span><span class="sxs-lookup"><span data-stu-id="15b5c-147">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="15b5c-148">Добавление вкладки канала</span><span class="sxs-lookup"><span data-stu-id="15b5c-148">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="15b5c-149">teamsTab</span><span class="sxs-lookup"><span data-stu-id="15b5c-149">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="15b5c-150">Добавляет (установить) вкладки канал группы.</span><span class="sxs-lookup"><span data-stu-id="15b5c-150">Adds (installs) a tab to a team's channel.</span></span>|
|[<span data-ttu-id="15b5c-151">Список сообщения</span><span class="sxs-lookup"><span data-stu-id="15b5c-151">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="15b5c-152">chatMessage</span><span class="sxs-lookup"><span data-stu-id="15b5c-152">chatMessage</span></span>](../resources/chatmessage.md) | [<span data-ttu-id="15b5c-153">Получение сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="15b5c-153">Get messages in a channel</span></span>](../api/channel-list-messages.md) |

## <a name="properties"></a><span data-ttu-id="15b5c-154">Свойства</span><span class="sxs-lookup"><span data-stu-id="15b5c-154">Properties</span></span>

| <span data-ttu-id="15b5c-155">Свойство</span><span class="sxs-lookup"><span data-stu-id="15b5c-155">Property</span></span> | <span data-ttu-id="15b5c-156">Тип</span><span class="sxs-lookup"><span data-stu-id="15b5c-156">Type</span></span>   | <span data-ttu-id="15b5c-157">Description</span><span class="sxs-lookup"><span data-stu-id="15b5c-157">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="15b5c-158">funSettings</span><span class="sxs-lookup"><span data-stu-id="15b5c-158">funSettings</span></span>|[<span data-ttu-id="15b5c-159">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="15b5c-159">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="15b5c-160">Параметры для настройки использования Giphy, memes и наклейки рабочих групп.</span><span class="sxs-lookup"><span data-stu-id="15b5c-160">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="15b5c-161">guestSettings</span><span class="sxs-lookup"><span data-stu-id="15b5c-161">guestSettings</span></span>|[<span data-ttu-id="15b5c-162">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="15b5c-162">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="15b5c-163">Параметры для настройки ли гости могут создать, обновить или удалить каналы рабочих групп.</span><span class="sxs-lookup"><span data-stu-id="15b5c-163">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="15b5c-164">isArchived</span><span class="sxs-lookup"><span data-stu-id="15b5c-164">isArchived</span></span>|<span data-ttu-id="15b5c-165">Логический</span><span class="sxs-lookup"><span data-stu-id="15b5c-165">Boolean</span></span>|<span data-ttu-id="15b5c-166">Является ли эта группа в режиме только для чтения.</span><span class="sxs-lookup"><span data-stu-id="15b5c-166">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="15b5c-167">memberSettings</span><span class="sxs-lookup"><span data-stu-id="15b5c-167">memberSettings</span></span>|[<span data-ttu-id="15b5c-168">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="15b5c-168">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="15b5c-169">Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, рабочих групп.</span><span class="sxs-lookup"><span data-stu-id="15b5c-169">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="15b5c-170">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="15b5c-170">messagingSettings</span></span>|[<span data-ttu-id="15b5c-171">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="15b5c-171">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="15b5c-172">Параметры для настройки системы обмена сообщениями и упоминания рабочих групп.</span><span class="sxs-lookup"><span data-stu-id="15b5c-172">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="15b5c-173">webUrl</span><span class="sxs-lookup"><span data-stu-id="15b5c-173">webUrl</span></span>|<span data-ttu-id="15b5c-174">String (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="15b5c-174">string (readonly)</span></span> | <span data-ttu-id="15b5c-175">Гиперссылка, будут поступать на группы в клиенте группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="15b5c-175">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="15b5c-176">Это URL-адрес, который вы получаете при щелкните правой кнопкой мыши группы в клиенте Microsoft группы и выберите **получить ссылку на группы**.</span><span class="sxs-lookup"><span data-stu-id="15b5c-176">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="15b5c-177">Этот URL-адрес должен быть обрабатываются как непрозрачный больших двоичных объектов и не синтаксический анализ.</span><span class="sxs-lookup"><span data-stu-id="15b5c-177">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="15b5c-178">Связи</span><span class="sxs-lookup"><span data-stu-id="15b5c-178">Relationships</span></span>

| <span data-ttu-id="15b5c-179">Связь</span><span class="sxs-lookup"><span data-stu-id="15b5c-179">Relationship</span></span> | <span data-ttu-id="15b5c-180">Тип</span><span class="sxs-lookup"><span data-stu-id="15b5c-180">Type</span></span>   | <span data-ttu-id="15b5c-181">Описание</span><span class="sxs-lookup"><span data-stu-id="15b5c-181">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="15b5c-182">apps</span><span class="sxs-lookup"><span data-stu-id="15b5c-182">apps</span></span>|<span data-ttu-id="15b5c-183">[teamsApp](teamsapp.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="15b5c-183">[teamsApp](teamsapp.md) collection</span></span>| <span data-ttu-id="15b5c-184">(Устаревший) Приложения, установленные в этой группе.</span><span class="sxs-lookup"><span data-stu-id="15b5c-184">(Obsolete) The apps installed in this team.</span></span>|
|<span data-ttu-id="15b5c-185">каналы</span><span class="sxs-lookup"><span data-stu-id="15b5c-185">channels</span></span>|<span data-ttu-id="15b5c-186">Коллекция [канала](channel.md)</span><span class="sxs-lookup"><span data-stu-id="15b5c-186">[channel](channel.md) collection</span></span>|<span data-ttu-id="15b5c-187">Коллекция каналы & сообщения, связанный с группой.</span><span class="sxs-lookup"><span data-stu-id="15b5c-187">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="15b5c-188">installedApps</span><span class="sxs-lookup"><span data-stu-id="15b5c-188">installedApps</span></span>|<span data-ttu-id="15b5c-189">[teamsAppInstallation](teamsappinstallation.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="15b5c-189">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="15b5c-190">Приложения, установленные в этой группе.</span><span class="sxs-lookup"><span data-stu-id="15b5c-190">The apps installed in this team.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="15b5c-191">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15b5c-191">JSON representation</span></span>

<span data-ttu-id="15b5c-192">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15b5c-192">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.team",
  "baseType": "microsoft.graph.entity"
}-->

```json
{  
  "guestSettings": {"@odata.type": "microsoft.graph.teamGuestSettings"},
  "memberSettings": {"@odata.type": "microsoft.graph.teamMemberSettings"},
  "messagingSettings": {"@odata.type": "microsoft.graph.teamMessagingSettings"},
  "funSettings": {"@odata.type": "microsoft.graph.teamFunSettings"},
  "isArchived": false,
  "webUrl": "https://...longUrl..."
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="15b5c-193">См. также</span><span class="sxs-lookup"><span data-stu-id="15b5c-193">See Also</span></span>
- [<span data-ttu-id="15b5c-194">Создание группы с группой</span><span class="sxs-lookup"><span data-stu-id="15b5c-194">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="15b5c-195">Обзор API групп</span><span class="sxs-lookup"><span data-stu-id="15b5c-195">Teams API Overview</span></span>](teams-api-overview.md)
