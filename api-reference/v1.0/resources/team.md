---
title: Тип ресурса team
description: 'Команда в Microsoft Teams — это коллекция каналов. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 460bbfaa522cf4767d7f35992a4371bf870c8948
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793684"
---
# <a name="team-resource-type"></a><span data-ttu-id="4254b-103">Тип ресурса team</span><span class="sxs-lookup"><span data-stu-id="4254b-103">team resource type</span></span>

<span data-ttu-id="4254b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4254b-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="4254b-105">Команда в Microsoft Teams — это коллекция объектов [channel](channel.md).</span><span class="sxs-lookup"><span data-stu-id="4254b-105">A team in Microsoft Teams is a collection of [channel](channel.md) objects.</span></span>
<span data-ttu-id="4254b-106">Канал представляет тему и логически обособляет обсуждение в команде.</span><span class="sxs-lookup"><span data-stu-id="4254b-106">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="4254b-107">Каждая команда связана с [группой](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="4254b-107">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="4254b-108">У группы такой же идентификатор, как у команды. Например, /groups/{id}/team совпадает с /teams/{id}.</span><span class="sxs-lookup"><span data-stu-id="4254b-108">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="4254b-109">Дополнительные сведения о работе с группами и участниками в командах см. в статье [Работа с Microsoft Teams при помощи REST API Microsoft Graph](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="4254b-109">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4254b-110">Методы</span><span class="sxs-lookup"><span data-stu-id="4254b-110">Methods</span></span>

| <span data-ttu-id="4254b-111">Метод</span><span class="sxs-lookup"><span data-stu-id="4254b-111">Method</span></span>       | <span data-ttu-id="4254b-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4254b-112">Return Type</span></span>  |<span data-ttu-id="4254b-113">Описание</span><span class="sxs-lookup"><span data-stu-id="4254b-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4254b-114">Создание команды</span><span class="sxs-lookup"><span data-stu-id="4254b-114">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="4254b-115">team</span><span class="sxs-lookup"><span data-stu-id="4254b-115">team</span></span>](team.md) | <span data-ttu-id="4254b-116">Создание команды или добавление команды в существующую группу.</span><span class="sxs-lookup"><span data-stu-id="4254b-116">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="4254b-117">Получение команды</span><span class="sxs-lookup"><span data-stu-id="4254b-117">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="4254b-118">team</span><span class="sxs-lookup"><span data-stu-id="4254b-118">team</span></span>](team.md) | <span data-ttu-id="4254b-119">Получение свойств и связей указанной команды.</span><span class="sxs-lookup"><span data-stu-id="4254b-119">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="4254b-120">Обновление команды</span><span class="sxs-lookup"><span data-stu-id="4254b-120">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="4254b-121">team</span><span class="sxs-lookup"><span data-stu-id="4254b-121">team</span></span>](team.md) |<span data-ttu-id="4254b-122">Обновление свойств указанной команды.</span><span class="sxs-lookup"><span data-stu-id="4254b-122">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="4254b-123">Удаление команды</span><span class="sxs-lookup"><span data-stu-id="4254b-123">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="4254b-124">Нет</span><span class="sxs-lookup"><span data-stu-id="4254b-124">None</span></span> |<span data-ttu-id="4254b-125">Удаление команды и ее связанной группы.</span><span class="sxs-lookup"><span data-stu-id="4254b-125">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="4254b-126">Клонирование команды</span><span class="sxs-lookup"><span data-stu-id="4254b-126">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="4254b-127">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="4254b-127">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="4254b-128">Копирование команды и ее связанной группы.</span><span class="sxs-lookup"><span data-stu-id="4254b-128">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="4254b-129">Архивация команды</span><span class="sxs-lookup"><span data-stu-id="4254b-129">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="4254b-130">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="4254b-130">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="4254b-131">Перевод команды в состояние только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4254b-131">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="4254b-132">Распаковка команды</span><span class="sxs-lookup"><span data-stu-id="4254b-132">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="4254b-133">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="4254b-133">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="4254b-134">Восстановление команды в состояние чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="4254b-134">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="4254b-135">Перечисление ваших команд</span><span class="sxs-lookup"><span data-stu-id="4254b-135">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="4254b-136">Коллекция [team](team.md)</span><span class="sxs-lookup"><span data-stu-id="4254b-136">[team](team.md) collection</span></span> | <span data-ttu-id="4254b-137">Перечисление команд, в которых вы являетесь участником.</span><span class="sxs-lookup"><span data-stu-id="4254b-137">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="4254b-138">Перечисление всех команд</span><span class="sxs-lookup"><span data-stu-id="4254b-138">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="4254b-139">Коллекция [group](group.md)</span><span class="sxs-lookup"><span data-stu-id="4254b-139">[group](group.md) collection</span></span> | <span data-ttu-id="4254b-140">Перечисление всех групп, содержащих команды.</span><span class="sxs-lookup"><span data-stu-id="4254b-140">List all groups that have teams.</span></span> |
|[<span data-ttu-id="4254b-141">Публикация приложений в организации</span><span class="sxs-lookup"><span data-stu-id="4254b-141">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="4254b-142">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4254b-142">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="4254b-143">Создание приложений Teams, видимых только для вашей организации.</span><span class="sxs-lookup"><span data-stu-id="4254b-143">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="4254b-144">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="4254b-144">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="4254b-145">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="4254b-145">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="4254b-146">Добавляет (устанавливает) приложение в команду.</span><span class="sxs-lookup"><span data-stu-id="4254b-146">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="4254b-147">Добавление вкладки в канал</span><span class="sxs-lookup"><span data-stu-id="4254b-147">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="4254b-148">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4254b-148">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="4254b-149">Добавляет (устанавливает) вкладку в канал команды.</span><span class="sxs-lookup"><span data-stu-id="4254b-149">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="4254b-150">Свойства</span><span class="sxs-lookup"><span data-stu-id="4254b-150">Properties</span></span>

| <span data-ttu-id="4254b-151">Свойство</span><span class="sxs-lookup"><span data-stu-id="4254b-151">Property</span></span> | <span data-ttu-id="4254b-152">Тип</span><span class="sxs-lookup"><span data-stu-id="4254b-152">Type</span></span>   | <span data-ttu-id="4254b-153">Описание</span><span class="sxs-lookup"><span data-stu-id="4254b-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4254b-154">funSettings</span><span class="sxs-lookup"><span data-stu-id="4254b-154">funSettings</span></span>|[<span data-ttu-id="4254b-155">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="4254b-155">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="4254b-156">Параметры для настройки использования Giphy, мемов и наклеек в команде.</span><span class="sxs-lookup"><span data-stu-id="4254b-156">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="4254b-157">guestSettings</span><span class="sxs-lookup"><span data-stu-id="4254b-157">guestSettings</span></span>|[<span data-ttu-id="4254b-158">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="4254b-158">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="4254b-159">Параметры для настройки того, могут ли гости создавать, изменять или удалять каналы в команде.</span><span class="sxs-lookup"><span data-stu-id="4254b-159">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="4254b-160">internalId</span><span class="sxs-lookup"><span data-stu-id="4254b-160">internalId</span></span> | <span data-ttu-id="4254b-161">string</span><span class="sxs-lookup"><span data-stu-id="4254b-161">string</span></span> | <span data-ttu-id="4254b-162">Уникальный идентификатор для команды, используемый в нескольких местах, например в журнале аудита или [API действий управления Office 365](/office/office-365-management-api/office-365-management-activity-api-reference).</span><span class="sxs-lookup"><span data-stu-id="4254b-162">A unique ID for the team that has been used in a few places such as the audit log/[Office 365 Management Activity API](/office/office-365-management-api/office-365-management-activity-api-reference).</span></span> |
|<span data-ttu-id="4254b-163">isArchived</span><span class="sxs-lookup"><span data-stu-id="4254b-163">isArchived</span></span>|<span data-ttu-id="4254b-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="4254b-164">Boolean</span></span>|<span data-ttu-id="4254b-165">Находится ли команда в режиме только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4254b-165">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="4254b-166">memberSettings</span><span class="sxs-lookup"><span data-stu-id="4254b-166">memberSettings</span></span>|[<span data-ttu-id="4254b-167">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="4254b-167">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="4254b-168">Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.</span><span class="sxs-lookup"><span data-stu-id="4254b-168">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="4254b-169">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="4254b-169">messagingSettings</span></span>|[<span data-ttu-id="4254b-170">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="4254b-170">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="4254b-171">Параметры для настройки обмена сообщениями и упоминаний в команде.</span><span class="sxs-lookup"><span data-stu-id="4254b-171">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="4254b-172">webUrl</span><span class="sxs-lookup"><span data-stu-id="4254b-172">webUrl</span></span>|<span data-ttu-id="4254b-173">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="4254b-173">string (readonly)</span></span> | <span data-ttu-id="4254b-174">Гиперссылка, ведущая к команде в клиенте Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4254b-174">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="4254b-175">Это URL-адрес, получаемый при щелчке правой кнопкой мыши по команде в клиенте Microsoft Teams и выборе пункта **Получить ссылку на команду**.</span><span class="sxs-lookup"><span data-stu-id="4254b-175">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="4254b-176">Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться.</span><span class="sxs-lookup"><span data-stu-id="4254b-176">This URL should be treated as an opaque blob, and not parsed.</span></span> |
|<span data-ttu-id="4254b-177">classSettings</span><span class="sxs-lookup"><span data-stu-id="4254b-177">classSettings</span></span>|[<span data-ttu-id="4254b-178">teamClassSettings</span><span class="sxs-lookup"><span data-stu-id="4254b-178">teamClassSettings</span></span>](teamclasssettings.md) |<span data-ttu-id="4254b-179">Настройка параметров класса.</span><span class="sxs-lookup"><span data-stu-id="4254b-179">Configure settings of a class.</span></span> <span data-ttu-id="4254b-180">Доступна только в том случае, если команда представляет класс.</span><span class="sxs-lookup"><span data-stu-id="4254b-180">Available only when the team represents a class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4254b-181">Связи</span><span class="sxs-lookup"><span data-stu-id="4254b-181">Relationships</span></span>

| <span data-ttu-id="4254b-182">Связь</span><span class="sxs-lookup"><span data-stu-id="4254b-182">Relationship</span></span> | <span data-ttu-id="4254b-183">Тип</span><span class="sxs-lookup"><span data-stu-id="4254b-183">Type</span></span>   | <span data-ttu-id="4254b-184">Описание</span><span class="sxs-lookup"><span data-stu-id="4254b-184">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4254b-185">channels</span><span class="sxs-lookup"><span data-stu-id="4254b-185">channels</span></span>|<span data-ttu-id="4254b-186">Коллекция [channel](channel.md)</span><span class="sxs-lookup"><span data-stu-id="4254b-186">[channel](channel.md) collection</span></span>|<span data-ttu-id="4254b-187">Коллекция каналов и сообщений, связанных с командой.</span><span class="sxs-lookup"><span data-stu-id="4254b-187">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="4254b-188">installedApps</span><span class="sxs-lookup"><span data-stu-id="4254b-188">installedApps</span></span>|<span data-ttu-id="4254b-189">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="4254b-189">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="4254b-190">Приложения, установленные в команде.</span><span class="sxs-lookup"><span data-stu-id="4254b-190">The apps installed in this team.</span></span>|
|[<span data-ttu-id="4254b-191">primaryChannel</span><span class="sxs-lookup"><span data-stu-id="4254b-191">primaryChannel</span></span>](../api/team-get-primarychannel.md)|[<span data-ttu-id="4254b-192">channel</span><span class="sxs-lookup"><span data-stu-id="4254b-192">channel</span></span>](channel.md)| <span data-ttu-id="4254b-193">Общий канал для команды.</span><span class="sxs-lookup"><span data-stu-id="4254b-193">The general channel for the team.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="4254b-194">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4254b-194">JSON representation</span></span>

<span data-ttu-id="4254b-195">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4254b-195">The following is a JSON representation of the resource.</span></span>

><span data-ttu-id="4254b-196">**Примечание.** Если команда относится к типу class, к ней применяется свойство **classSettings**.</span><span class="sxs-lookup"><span data-stu-id="4254b-196">**Note:** If the team is of type class, a **classSettings** property is applied on the team.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="4254b-197">См. также</span><span class="sxs-lookup"><span data-stu-id="4254b-197">See Also</span></span>
- [<span data-ttu-id="4254b-198">Создание группы с командой</span><span class="sxs-lookup"><span data-stu-id="4254b-198">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="4254b-199">Использование API Teams</span><span class="sxs-lookup"><span data-stu-id="4254b-199">Using Teams APIs</span></span>](teams-api-overview.md)
