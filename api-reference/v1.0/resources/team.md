---
title: Тип ресурса team
description: 'Команда в Microsoft Teams — это коллекция каналов. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1a3b05eb0f055cd1cbed84f0e98c1496015f8801
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050913"
---
# <a name="team-resource-type"></a><span data-ttu-id="16fb5-103">Тип ресурса team</span><span class="sxs-lookup"><span data-stu-id="16fb5-103">team resource type</span></span>

<span data-ttu-id="16fb5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16fb5-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="16fb5-105">Команда в Microsoft Teams — это коллекция объектов [channel](channel.md).</span><span class="sxs-lookup"><span data-stu-id="16fb5-105">A team in Microsoft Teams is a collection of [channel](channel.md) objects.</span></span>
<span data-ttu-id="16fb5-106">Канал представляет тему и логически обособляет обсуждение в команде.</span><span class="sxs-lookup"><span data-stu-id="16fb5-106">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="16fb5-107">Каждая команда связана с [группой](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="16fb5-107">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="16fb5-108">У группы такой же идентификатор, как у команды. Например, /groups/{id}/team совпадает с /teams/{id}.</span><span class="sxs-lookup"><span data-stu-id="16fb5-108">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="16fb5-109">Дополнительные сведения о работе с группами и участниками в командах см. в статье [Работа с Microsoft Teams при помощи REST API Microsoft Graph](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="16fb5-109">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="16fb5-110">Методы</span><span class="sxs-lookup"><span data-stu-id="16fb5-110">Methods</span></span>

| <span data-ttu-id="16fb5-111">Метод</span><span class="sxs-lookup"><span data-stu-id="16fb5-111">Method</span></span>       | <span data-ttu-id="16fb5-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="16fb5-112">Return Type</span></span>  |<span data-ttu-id="16fb5-113">Описание</span><span class="sxs-lookup"><span data-stu-id="16fb5-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="16fb5-114">Создание команды</span><span class="sxs-lookup"><span data-stu-id="16fb5-114">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="16fb5-115">team</span><span class="sxs-lookup"><span data-stu-id="16fb5-115">team</span></span>](team.md) | <span data-ttu-id="16fb5-116">Создание команды или добавление команды в существующую группу.</span><span class="sxs-lookup"><span data-stu-id="16fb5-116">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="16fb5-117">Получение команды</span><span class="sxs-lookup"><span data-stu-id="16fb5-117">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="16fb5-118">team</span><span class="sxs-lookup"><span data-stu-id="16fb5-118">team</span></span>](team.md) | <span data-ttu-id="16fb5-119">Получение свойств и связей указанной команды.</span><span class="sxs-lookup"><span data-stu-id="16fb5-119">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="16fb5-120">Обновление команды</span><span class="sxs-lookup"><span data-stu-id="16fb5-120">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="16fb5-121">team</span><span class="sxs-lookup"><span data-stu-id="16fb5-121">team</span></span>](team.md) |<span data-ttu-id="16fb5-122">Обновление свойств указанной команды.</span><span class="sxs-lookup"><span data-stu-id="16fb5-122">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="16fb5-123">Удаление команды</span><span class="sxs-lookup"><span data-stu-id="16fb5-123">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="16fb5-124">Нет</span><span class="sxs-lookup"><span data-stu-id="16fb5-124">None</span></span> |<span data-ttu-id="16fb5-125">Удаление команды и ее связанной группы.</span><span class="sxs-lookup"><span data-stu-id="16fb5-125">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="16fb5-126">Клонирование команды</span><span class="sxs-lookup"><span data-stu-id="16fb5-126">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="16fb5-127">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="16fb5-127">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="16fb5-128">Копирование команды и ее связанной группы.</span><span class="sxs-lookup"><span data-stu-id="16fb5-128">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="16fb5-129">Архивация команды</span><span class="sxs-lookup"><span data-stu-id="16fb5-129">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="16fb5-130">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="16fb5-130">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="16fb5-131">Перевод команды в состояние только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16fb5-131">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="16fb5-132">Распаковка команды</span><span class="sxs-lookup"><span data-stu-id="16fb5-132">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="16fb5-133">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="16fb5-133">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="16fb5-134">Восстановление команды в состояние чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="16fb5-134">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="16fb5-135">Перечисление ваших команд</span><span class="sxs-lookup"><span data-stu-id="16fb5-135">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="16fb5-136">Коллекция [team](team.md)</span><span class="sxs-lookup"><span data-stu-id="16fb5-136">[team](team.md) collection</span></span> | <span data-ttu-id="16fb5-137">Перечисление команд, в которых вы являетесь участником.</span><span class="sxs-lookup"><span data-stu-id="16fb5-137">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="16fb5-138">Перечисление всех команд</span><span class="sxs-lookup"><span data-stu-id="16fb5-138">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="16fb5-139">Коллекция [group](group.md)</span><span class="sxs-lookup"><span data-stu-id="16fb5-139">[group](group.md) collection</span></span> | <span data-ttu-id="16fb5-140">Перечисление всех групп, содержащих команды.</span><span class="sxs-lookup"><span data-stu-id="16fb5-140">List all groups that have teams.</span></span> |
|[<span data-ttu-id="16fb5-141">Публикация приложений в организации</span><span class="sxs-lookup"><span data-stu-id="16fb5-141">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="16fb5-142">teamsApp</span><span class="sxs-lookup"><span data-stu-id="16fb5-142">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="16fb5-143">Создание приложений Teams, видимых только для вашей организации.</span><span class="sxs-lookup"><span data-stu-id="16fb5-143">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="16fb5-144">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="16fb5-144">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="16fb5-145">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="16fb5-145">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="16fb5-146">Добавляет (устанавливает) приложение в команду.</span><span class="sxs-lookup"><span data-stu-id="16fb5-146">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="16fb5-147">Добавление вкладки в канал</span><span class="sxs-lookup"><span data-stu-id="16fb5-147">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="16fb5-148">teamsTab</span><span class="sxs-lookup"><span data-stu-id="16fb5-148">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="16fb5-149">Добавляет (устанавливает) вкладку в канал команды.</span><span class="sxs-lookup"><span data-stu-id="16fb5-149">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="16fb5-150">Свойства</span><span class="sxs-lookup"><span data-stu-id="16fb5-150">Properties</span></span>

| <span data-ttu-id="16fb5-151">Свойство</span><span class="sxs-lookup"><span data-stu-id="16fb5-151">Property</span></span> | <span data-ttu-id="16fb5-152">Тип</span><span class="sxs-lookup"><span data-stu-id="16fb5-152">Type</span></span>   | <span data-ttu-id="16fb5-153">Описание</span><span class="sxs-lookup"><span data-stu-id="16fb5-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="16fb5-154">funSettings</span><span class="sxs-lookup"><span data-stu-id="16fb5-154">funSettings</span></span>|[<span data-ttu-id="16fb5-155">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="16fb5-155">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="16fb5-156">Параметры для настройки использования Giphy, мемов и наклеек в команде.</span><span class="sxs-lookup"><span data-stu-id="16fb5-156">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="16fb5-157">guestSettings</span><span class="sxs-lookup"><span data-stu-id="16fb5-157">guestSettings</span></span>|[<span data-ttu-id="16fb5-158">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="16fb5-158">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="16fb5-159">Параметры для настройки того, могут ли гости создавать, изменять или удалять каналы в команде.</span><span class="sxs-lookup"><span data-stu-id="16fb5-159">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="16fb5-160">internalId</span><span class="sxs-lookup"><span data-stu-id="16fb5-160">internalId</span></span> | <span data-ttu-id="16fb5-161">string</span><span class="sxs-lookup"><span data-stu-id="16fb5-161">string</span></span> | <span data-ttu-id="16fb5-162">Уникальный идентификатор для команды, используемый в нескольких местах, например в журнале аудита или [API действий управления Office 365](/office/office-365-management-api/office-365-management-activity-api-reference).</span><span class="sxs-lookup"><span data-stu-id="16fb5-162">A unique ID for the team that has been used in a few places such as the audit log/[Office 365 Management Activity API](/office/office-365-management-api/office-365-management-activity-api-reference).</span></span> |
|<span data-ttu-id="16fb5-163">isArchived</span><span class="sxs-lookup"><span data-stu-id="16fb5-163">isArchived</span></span>|<span data-ttu-id="16fb5-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="16fb5-164">Boolean</span></span>|<span data-ttu-id="16fb5-165">Находится ли команда в режиме только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16fb5-165">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="16fb5-166">memberSettings</span><span class="sxs-lookup"><span data-stu-id="16fb5-166">memberSettings</span></span>|[<span data-ttu-id="16fb5-167">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="16fb5-167">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="16fb5-168">Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.</span><span class="sxs-lookup"><span data-stu-id="16fb5-168">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="16fb5-169">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="16fb5-169">messagingSettings</span></span>|[<span data-ttu-id="16fb5-170">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="16fb5-170">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="16fb5-171">Параметры для настройки обмена сообщениями и упоминаний в команде.</span><span class="sxs-lookup"><span data-stu-id="16fb5-171">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="16fb5-172">webUrl</span><span class="sxs-lookup"><span data-stu-id="16fb5-172">webUrl</span></span>|<span data-ttu-id="16fb5-173">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="16fb5-173">string (readonly)</span></span> | <span data-ttu-id="16fb5-174">Гиперссылка, ведущая к команде в клиенте Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="16fb5-174">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="16fb5-175">Это URL-адрес, получаемый при щелчке правой кнопкой мыши по команде в клиенте Microsoft Teams и выборе пункта **Получить ссылку на команду**.</span><span class="sxs-lookup"><span data-stu-id="16fb5-175">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="16fb5-176">Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться.</span><span class="sxs-lookup"><span data-stu-id="16fb5-176">This URL should be treated as an opaque blob, and not parsed.</span></span> |
|<span data-ttu-id="16fb5-177">classSettings</span><span class="sxs-lookup"><span data-stu-id="16fb5-177">classSettings</span></span>|[<span data-ttu-id="16fb5-178">teamClassSettings</span><span class="sxs-lookup"><span data-stu-id="16fb5-178">teamClassSettings</span></span>](teamclasssettings.md) |<span data-ttu-id="16fb5-179">Настройка параметров класса.</span><span class="sxs-lookup"><span data-stu-id="16fb5-179">Configure settings of a class.</span></span> <span data-ttu-id="16fb5-180">Доступна только в том случае, если команда представляет класс.</span><span class="sxs-lookup"><span data-stu-id="16fb5-180">Available only when the team represents a class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16fb5-181">Связи</span><span class="sxs-lookup"><span data-stu-id="16fb5-181">Relationships</span></span>

| <span data-ttu-id="16fb5-182">Связь</span><span class="sxs-lookup"><span data-stu-id="16fb5-182">Relationship</span></span> | <span data-ttu-id="16fb5-183">Тип</span><span class="sxs-lookup"><span data-stu-id="16fb5-183">Type</span></span>   | <span data-ttu-id="16fb5-184">Описание</span><span class="sxs-lookup"><span data-stu-id="16fb5-184">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="16fb5-185">channels</span><span class="sxs-lookup"><span data-stu-id="16fb5-185">channels</span></span>|<span data-ttu-id="16fb5-186">Коллекция [channel](channel.md)</span><span class="sxs-lookup"><span data-stu-id="16fb5-186">[channel](channel.md) collection</span></span>|<span data-ttu-id="16fb5-187">Коллекция каналов и сообщений, связанных с командой.</span><span class="sxs-lookup"><span data-stu-id="16fb5-187">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="16fb5-188">installedApps</span><span class="sxs-lookup"><span data-stu-id="16fb5-188">installedApps</span></span>|<span data-ttu-id="16fb5-189">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="16fb5-189">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="16fb5-190">Приложения, установленные в команде.</span><span class="sxs-lookup"><span data-stu-id="16fb5-190">The apps installed in this team.</span></span>|
|[<span data-ttu-id="16fb5-191">primaryChannel</span><span class="sxs-lookup"><span data-stu-id="16fb5-191">primaryChannel</span></span>](../api/team-get-primarychannel.md)|[<span data-ttu-id="16fb5-192">channel</span><span class="sxs-lookup"><span data-stu-id="16fb5-192">channel</span></span>](channel.md)| <span data-ttu-id="16fb5-193">Общий канал для команды.</span><span class="sxs-lookup"><span data-stu-id="16fb5-193">The general channel for the team.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="16fb5-194">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16fb5-194">JSON representation</span></span>

<span data-ttu-id="16fb5-195">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16fb5-195">The following is a JSON representation of the resource.</span></span>

><span data-ttu-id="16fb5-196">**Примечание.** Если команда относится к типу class, к ней применяется свойство **classSettings**.</span><span class="sxs-lookup"><span data-stu-id="16fb5-196">**Note:** If the team is of type class, a **classSettings** property is applied on the team.</span></span>

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
  "internalId": "string",
  "isArchived": false,
  "webUrl": "string (URL)",
  "classSettings": {"@odata.type": "microsoft.graph.teamClassSettings"}
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

## <a name="see-also"></a><span data-ttu-id="16fb5-197">См. также</span><span class="sxs-lookup"><span data-stu-id="16fb5-197">See Also</span></span>
- [<span data-ttu-id="16fb5-198">Создание группы с командой</span><span class="sxs-lookup"><span data-stu-id="16fb5-198">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="16fb5-199">Использование API Teams</span><span class="sxs-lookup"><span data-stu-id="16fb5-199">Using Teams APIs</span></span>](teams-api-overview.md)
