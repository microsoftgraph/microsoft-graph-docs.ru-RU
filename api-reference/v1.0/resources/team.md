---
title: Тип ресурса team
description: 'Команда в Microsoft Teams — это коллекция каналов. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 7c3dd42c25ce8c48722ab857f61e0c6a9a275581
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964138"
---
# <a name="team-resource-type"></a><span data-ttu-id="f9c8a-103">Тип ресурса team</span><span class="sxs-lookup"><span data-stu-id="f9c8a-103">team resource type</span></span>



<span data-ttu-id="f9c8a-104">Команда в Microsoft Teams — это коллекция объектов [channel](channel.md).</span><span class="sxs-lookup"><span data-stu-id="f9c8a-104">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="f9c8a-105">Канал представляет тему и логически обособляет обсуждение в команде.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="f9c8a-106">Каждая команда связана с [группой](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="f9c8a-106">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="f9c8a-107">У группы такой же идентификатор, как у команды. Например, /groups/{id}/team совпадает с /teams/{id}.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-107">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="f9c8a-108">Дополнительные сведения о работе с группами и участниками в командах см. в статье [Работа с Microsoft Teams при помощи REST API Microsoft Graph](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="f9c8a-108">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f9c8a-109">Методы</span><span class="sxs-lookup"><span data-stu-id="f9c8a-109">Methods</span></span>

| <span data-ttu-id="f9c8a-110">Метод</span><span class="sxs-lookup"><span data-stu-id="f9c8a-110">Method</span></span>       | <span data-ttu-id="f9c8a-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f9c8a-111">Return Type</span></span>  |<span data-ttu-id="f9c8a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f9c8a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f9c8a-113">Создание команды</span><span class="sxs-lookup"><span data-stu-id="f9c8a-113">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="f9c8a-114">team</span><span class="sxs-lookup"><span data-stu-id="f9c8a-114">team</span></span>](team.md) | <span data-ttu-id="f9c8a-115">Создание команды или добавление команды в существующую группу.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-115">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="f9c8a-116">Получение команды</span><span class="sxs-lookup"><span data-stu-id="f9c8a-116">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="f9c8a-117">team</span><span class="sxs-lookup"><span data-stu-id="f9c8a-117">team</span></span>](team.md) | <span data-ttu-id="f9c8a-118">Получение свойств и связей указанной команды.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-118">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="f9c8a-119">Обновление команды</span><span class="sxs-lookup"><span data-stu-id="f9c8a-119">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="f9c8a-120">team</span><span class="sxs-lookup"><span data-stu-id="f9c8a-120">team</span></span>](team.md) |<span data-ttu-id="f9c8a-121">Обновление свойств указанной команды.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-121">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="f9c8a-122">Удаление команды</span><span class="sxs-lookup"><span data-stu-id="f9c8a-122">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="f9c8a-123">Нет</span><span class="sxs-lookup"><span data-stu-id="f9c8a-123">None</span></span> |<span data-ttu-id="f9c8a-124">Удаление команды и ее связанной группы.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-124">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="f9c8a-125">Клонирование команды</span><span class="sxs-lookup"><span data-stu-id="f9c8a-125">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="f9c8a-126">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="f9c8a-126">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="f9c8a-127">Копирование команды и ее связанной группы.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-127">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="f9c8a-128">Архивация команды</span><span class="sxs-lookup"><span data-stu-id="f9c8a-128">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="f9c8a-129">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="f9c8a-129">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="f9c8a-130">Перевод команды в состояние только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-130">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="f9c8a-131">Распаковка команды</span><span class="sxs-lookup"><span data-stu-id="f9c8a-131">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="f9c8a-132">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="f9c8a-132">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="f9c8a-133">Восстановление команды в состояние чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-133">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="f9c8a-134">Перечисление ваших команд</span><span class="sxs-lookup"><span data-stu-id="f9c8a-134">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="f9c8a-135">Коллекция [team](team.md)</span><span class="sxs-lookup"><span data-stu-id="f9c8a-135">[team](team.md) collection</span></span> | <span data-ttu-id="f9c8a-136">Перечисление команд, в которых вы являетесь участником.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-136">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="f9c8a-137">Перечисление всех команд</span><span class="sxs-lookup"><span data-stu-id="f9c8a-137">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="f9c8a-138">Коллекция [group](group.md)</span><span class="sxs-lookup"><span data-stu-id="f9c8a-138">[group](group.md) collection</span></span> | <span data-ttu-id="f9c8a-139">Перечисление всех групп, содержащих команды.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-139">List all groups that have teams.</span></span> |
|[<span data-ttu-id="f9c8a-140">Публикация приложений в организации</span><span class="sxs-lookup"><span data-stu-id="f9c8a-140">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="f9c8a-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="f9c8a-141">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="f9c8a-142">Создание приложений Teams, видимых только для вашей организации.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-142">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="f9c8a-143">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="f9c8a-143">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="f9c8a-144">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="f9c8a-144">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="f9c8a-145">Добавляет (устанавливает) приложение в команду.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-145">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="f9c8a-146">Добавление вкладки в канал</span><span class="sxs-lookup"><span data-stu-id="f9c8a-146">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="f9c8a-147">teamsTab</span><span class="sxs-lookup"><span data-stu-id="f9c8a-147">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="f9c8a-148">Добавляет (устанавливает) вкладку в канал команды.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-148">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="f9c8a-149">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9c8a-149">Properties</span></span>

| <span data-ttu-id="f9c8a-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9c8a-150">Property</span></span> | <span data-ttu-id="f9c8a-151">Тип</span><span class="sxs-lookup"><span data-stu-id="f9c8a-151">Type</span></span>   | <span data-ttu-id="f9c8a-152">Описание</span><span class="sxs-lookup"><span data-stu-id="f9c8a-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f9c8a-153">funSettings</span><span class="sxs-lookup"><span data-stu-id="f9c8a-153">funSettings</span></span>|[<span data-ttu-id="f9c8a-154">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="f9c8a-154">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="f9c8a-155">Параметры для настройки использования Giphy, мемов и наклеек в команде.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-155">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="f9c8a-156">guestSettings</span><span class="sxs-lookup"><span data-stu-id="f9c8a-156">guestSettings</span></span>|[<span data-ttu-id="f9c8a-157">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="f9c8a-157">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="f9c8a-158">Параметры для настройки того, могут ли гости создавать, изменять или удалять каналы в команде.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-158">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="f9c8a-159">internalId</span><span class="sxs-lookup"><span data-stu-id="f9c8a-159">internalId</span></span> | <span data-ttu-id="f9c8a-160">string</span><span class="sxs-lookup"><span data-stu-id="f9c8a-160">string</span></span> | <span data-ttu-id="f9c8a-161">Уникальный идентификатор для команды, используемый в нескольких местах, например в журнале аудита или [API действий управления Office 365](https://docs.microsoft.com/ru-RU/office/office-365-management-api/office-365-management-activity-api-reference).</span><span class="sxs-lookup"><span data-stu-id="f9c8a-161">A unique ID for the team that has been used in a few places such as the audit log/[Office 365 Management Activity API](https://docs.microsoft.com/ru-RU/office/office-365-management-api/office-365-management-activity-api-reference).</span></span> |
|<span data-ttu-id="f9c8a-162">isArchived</span><span class="sxs-lookup"><span data-stu-id="f9c8a-162">isArchived</span></span>|<span data-ttu-id="f9c8a-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9c8a-163">Boolean</span></span>|<span data-ttu-id="f9c8a-164">Находится ли команда в режиме только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-164">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="f9c8a-165">memberSettings</span><span class="sxs-lookup"><span data-stu-id="f9c8a-165">memberSettings</span></span>|[<span data-ttu-id="f9c8a-166">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="f9c8a-166">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="f9c8a-167">Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-167">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="f9c8a-168">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="f9c8a-168">messagingSettings</span></span>|[<span data-ttu-id="f9c8a-169">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="f9c8a-169">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="f9c8a-170">Параметры для настройки обмена сообщениями и упоминаний в команде.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-170">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="f9c8a-171">webUrl</span><span class="sxs-lookup"><span data-stu-id="f9c8a-171">webUrl</span></span>|<span data-ttu-id="f9c8a-172">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="f9c8a-172">string (readonly)</span></span> | <span data-ttu-id="f9c8a-173">Гиперссылка, ведущая к команде в клиенте Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-173">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="f9c8a-174">Это URL-адрес, получаемый при щелчке правой кнопкой мыши по команде в клиенте Microsoft Teams и выборе пункта **Получить ссылку на команду**.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-174">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="f9c8a-175">Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-175">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f9c8a-176">Связи</span><span class="sxs-lookup"><span data-stu-id="f9c8a-176">Relationships</span></span>

| <span data-ttu-id="f9c8a-177">Отношение</span><span class="sxs-lookup"><span data-stu-id="f9c8a-177">Relationship</span></span> | <span data-ttu-id="f9c8a-178">Тип</span><span class="sxs-lookup"><span data-stu-id="f9c8a-178">Type</span></span>   | <span data-ttu-id="f9c8a-179">Описание</span><span class="sxs-lookup"><span data-stu-id="f9c8a-179">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f9c8a-180">channels</span><span class="sxs-lookup"><span data-stu-id="f9c8a-180">channels</span></span>|<span data-ttu-id="f9c8a-181">Коллекция [channel](channel.md)</span><span class="sxs-lookup"><span data-stu-id="f9c8a-181">[channel](channel.md) collection</span></span>|<span data-ttu-id="f9c8a-182">Коллекция каналов и сообщений, связанных с командой.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-182">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="f9c8a-183">installedApps</span><span class="sxs-lookup"><span data-stu-id="f9c8a-183">installedApps</span></span>|<span data-ttu-id="f9c8a-184">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="f9c8a-184">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="f9c8a-185">Приложения, установленные в команде.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-185">The apps installed in this team.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9c8a-186">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f9c8a-186">JSON representation</span></span>

<span data-ttu-id="f9c8a-187">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9c8a-187">The following is a JSON representation of the resource.</span></span>

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
  "internalId": "19:...big.number...@thread.skype",
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

## <a name="see-also"></a><span data-ttu-id="f9c8a-188">См. также</span><span class="sxs-lookup"><span data-stu-id="f9c8a-188">See Also</span></span>
- [<span data-ttu-id="f9c8a-189">Создание группы с командой</span><span class="sxs-lookup"><span data-stu-id="f9c8a-189">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="f9c8a-190">Использование API Teams</span><span class="sxs-lookup"><span data-stu-id="f9c8a-190">Using Teams APIs</span></span>](teams-api-overview.md)
