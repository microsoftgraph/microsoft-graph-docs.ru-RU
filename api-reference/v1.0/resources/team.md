---
title: Тип ресурса группы
description: 'Группы в группах Microsoft — это коллекция каналов. '
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 85694e18771ac17873f97cedf68d074ee550f787
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878549"
---
# <a name="team-resource-type"></a><span data-ttu-id="e3a86-103">Тип ресурса группы</span><span class="sxs-lookup"><span data-stu-id="e3a86-103">team resource type</span></span>



<span data-ttu-id="e3a86-104">Группы в группах Microsoft — это коллекция [каналов](channel.md).</span><span class="sxs-lookup"><span data-stu-id="e3a86-104">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="e3a86-105">Канал представляет раздел и логическая изоляции обсуждения в группе.</span><span class="sxs-lookup"><span data-stu-id="e3a86-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="e3a86-106">Для любой группы связан с [группы](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="e3a86-106">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="e3a86-107">Группа имеет тот же идентификатор, как команда — например, /groups/ {идентификатор} / team совпадает с /teams/ {идентификатор}.</span><span class="sxs-lookup"><span data-stu-id="e3a86-107">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="e3a86-108">Дополнительные сведения о работе с группами и участниками групп показано [Использование интерфейса API REST графическое представление Microsoft для работы с группами Майкрософт](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="e3a86-108">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e3a86-109">Методы</span><span class="sxs-lookup"><span data-stu-id="e3a86-109">Methods</span></span>

| <span data-ttu-id="e3a86-110">Метод</span><span class="sxs-lookup"><span data-stu-id="e3a86-110">Method</span></span>       | <span data-ttu-id="e3a86-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e3a86-111">Return Type</span></span>  |<span data-ttu-id="e3a86-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e3a86-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e3a86-113">Создание группы</span><span class="sxs-lookup"><span data-stu-id="e3a86-113">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="e3a86-114">Группа</span><span class="sxs-lookup"><span data-stu-id="e3a86-114">team</span></span>](team.md) | <span data-ttu-id="e3a86-115">Создание новой группы или добавление группы к существующей группе.</span><span class="sxs-lookup"><span data-stu-id="e3a86-115">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="e3a86-116">Получение группы</span><span class="sxs-lookup"><span data-stu-id="e3a86-116">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="e3a86-117">Группа</span><span class="sxs-lookup"><span data-stu-id="e3a86-117">team</span></span>](team.md) | <span data-ttu-id="e3a86-118">Извлечение свойств и связи из указанной группы.</span><span class="sxs-lookup"><span data-stu-id="e3a86-118">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="e3a86-119">Группа обновления</span><span class="sxs-lookup"><span data-stu-id="e3a86-119">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="e3a86-120">Группа</span><span class="sxs-lookup"><span data-stu-id="e3a86-120">team</span></span>](team.md) |<span data-ttu-id="e3a86-121">Обновление свойств указанной группы.</span><span class="sxs-lookup"><span data-stu-id="e3a86-121">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="e3a86-122">Удаление группы</span><span class="sxs-lookup"><span data-stu-id="e3a86-122">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="e3a86-123">Нет</span><span class="sxs-lookup"><span data-stu-id="e3a86-123">None</span></span> |<span data-ttu-id="e3a86-124">Удаление группы и его связанную группу.</span><span class="sxs-lookup"><span data-stu-id="e3a86-124">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="e3a86-125">Клонирование группы</span><span class="sxs-lookup"><span data-stu-id="e3a86-125">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="e3a86-126">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="e3a86-126">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="e3a86-127">Скопируйте группа и его связанную группу.</span><span class="sxs-lookup"><span data-stu-id="e3a86-127">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="e3a86-128">Группа архива</span><span class="sxs-lookup"><span data-stu-id="e3a86-128">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="e3a86-129">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="e3a86-129">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="e3a86-130">Поместите группа в состояние только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3a86-130">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="e3a86-131">Unarchive группы</span><span class="sxs-lookup"><span data-stu-id="e3a86-131">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="e3a86-132">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="e3a86-132">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="e3a86-133">Восстановите группа в состояние чтение запись.</span><span class="sxs-lookup"><span data-stu-id="e3a86-133">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="e3a86-134">Список рабочих групп</span><span class="sxs-lookup"><span data-stu-id="e3a86-134">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="e3a86-135">семейства сайтов [групп](team.md)</span><span class="sxs-lookup"><span data-stu-id="e3a86-135">[team](team.md) collection</span></span> | <span data-ttu-id="e3a86-136">Список групп, которые вы являетесь членом.</span><span class="sxs-lookup"><span data-stu-id="e3a86-136">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="e3a86-137">Список всех групп</span><span class="sxs-lookup"><span data-stu-id="e3a86-137">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="e3a86-138">Коллекция объектов [group](group.md)</span><span class="sxs-lookup"><span data-stu-id="e3a86-138">[group](group.md) collection</span></span> | <span data-ttu-id="e3a86-139">Список всех групп, которые имеют группами.</span><span class="sxs-lookup"><span data-stu-id="e3a86-139">List all groups that have teams.</span></span> |
|[<span data-ttu-id="e3a86-140">Публикация приложений для вашей организации</span><span class="sxs-lookup"><span data-stu-id="e3a86-140">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="e3a86-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e3a86-141">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="e3a86-142">Создание групп приложений видимым только для вашей организации.</span><span class="sxs-lookup"><span data-stu-id="e3a86-142">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="e3a86-143">Добавление приложения в группу</span><span class="sxs-lookup"><span data-stu-id="e3a86-143">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="e3a86-144">teamsappinstallation</span><span class="sxs-lookup"><span data-stu-id="e3a86-144">teamsappinstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="e3a86-145">Добавляет (установить) приложения в группу.</span><span class="sxs-lookup"><span data-stu-id="e3a86-145">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="e3a86-146">Добавление вкладки канала</span><span class="sxs-lookup"><span data-stu-id="e3a86-146">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="e3a86-147">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e3a86-147">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="e3a86-148">Добавляет (установить) вкладки канал группы.</span><span class="sxs-lookup"><span data-stu-id="e3a86-148">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="e3a86-149">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3a86-149">Properties</span></span>

| <span data-ttu-id="e3a86-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3a86-150">Property</span></span> | <span data-ttu-id="e3a86-151">Тип</span><span class="sxs-lookup"><span data-stu-id="e3a86-151">Type</span></span>   | <span data-ttu-id="e3a86-152">Описание</span><span class="sxs-lookup"><span data-stu-id="e3a86-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e3a86-153">funSettings</span><span class="sxs-lookup"><span data-stu-id="e3a86-153">funSettings</span></span>|[<span data-ttu-id="e3a86-154">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="e3a86-154">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="e3a86-155">Параметры для настройки использования Giphy, memes и наклейки рабочих групп.</span><span class="sxs-lookup"><span data-stu-id="e3a86-155">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="e3a86-156">guestSettings</span><span class="sxs-lookup"><span data-stu-id="e3a86-156">guestSettings</span></span>|[<span data-ttu-id="e3a86-157">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="e3a86-157">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="e3a86-158">Параметры для настройки ли гости могут создать, обновить или удалить каналы рабочих групп.</span><span class="sxs-lookup"><span data-stu-id="e3a86-158">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="e3a86-159">isArchived</span><span class="sxs-lookup"><span data-stu-id="e3a86-159">isArchived</span></span>|<span data-ttu-id="e3a86-160">Логический</span><span class="sxs-lookup"><span data-stu-id="e3a86-160">Boolean</span></span>|<span data-ttu-id="e3a86-161">Является ли эта группа в режиме только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3a86-161">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="e3a86-162">memberSettings</span><span class="sxs-lookup"><span data-stu-id="e3a86-162">memberSettings</span></span>|[<span data-ttu-id="e3a86-163">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="e3a86-163">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="e3a86-164">Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, рабочих групп.</span><span class="sxs-lookup"><span data-stu-id="e3a86-164">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="e3a86-165">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="e3a86-165">messagingSettings</span></span>|[<span data-ttu-id="e3a86-166">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="e3a86-166">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="e3a86-167">Параметры для настройки системы обмена сообщениями и упоминания рабочих групп.</span><span class="sxs-lookup"><span data-stu-id="e3a86-167">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="e3a86-168">webUrl</span><span class="sxs-lookup"><span data-stu-id="e3a86-168">webUrl</span></span>|<span data-ttu-id="e3a86-169">String (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="e3a86-169">string (readonly)</span></span> | <span data-ttu-id="e3a86-170">Гиперссылка, будут поступать на группы в клиенте группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="e3a86-170">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="e3a86-171">Это URL-адрес, который вы получаете при щелкните правой кнопкой мыши группы в клиенте Microsoft группы и выберите **получить ссылку на группы**.</span><span class="sxs-lookup"><span data-stu-id="e3a86-171">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="e3a86-172">Этот URL-адрес должен быть обрабатываются как непрозрачный больших двоичных объектов и не синтаксический анализ.</span><span class="sxs-lookup"><span data-stu-id="e3a86-172">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e3a86-173">Связи</span><span class="sxs-lookup"><span data-stu-id="e3a86-173">Relationships</span></span>

| <span data-ttu-id="e3a86-174">Связь</span><span class="sxs-lookup"><span data-stu-id="e3a86-174">Relationship</span></span> | <span data-ttu-id="e3a86-175">Тип</span><span class="sxs-lookup"><span data-stu-id="e3a86-175">Type</span></span>   | <span data-ttu-id="e3a86-176">Описание</span><span class="sxs-lookup"><span data-stu-id="e3a86-176">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e3a86-177">каналы</span><span class="sxs-lookup"><span data-stu-id="e3a86-177">channels</span></span>|<span data-ttu-id="e3a86-178">Коллекция [канала](channel.md)</span><span class="sxs-lookup"><span data-stu-id="e3a86-178">[channel](channel.md) collection</span></span>|<span data-ttu-id="e3a86-179">Коллекция каналы & сообщения, связанный с группой.</span><span class="sxs-lookup"><span data-stu-id="e3a86-179">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="e3a86-180">installedApps</span><span class="sxs-lookup"><span data-stu-id="e3a86-180">installedApps</span></span>|<span data-ttu-id="e3a86-181">[teamsAppInstallation](teamsappinstallation.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e3a86-181">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="e3a86-182">Приложения, установленные в этой группе.</span><span class="sxs-lookup"><span data-stu-id="e3a86-182">The apps installed in this team.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3a86-183">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3a86-183">JSON representation</span></span>

<span data-ttu-id="e3a86-184">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3a86-184">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="e3a86-185">См. также</span><span class="sxs-lookup"><span data-stu-id="e3a86-185">See Also</span></span>
- [<span data-ttu-id="e3a86-186">Создание группы с группой</span><span class="sxs-lookup"><span data-stu-id="e3a86-186">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="e3a86-187">Использование интерфейсов API групп</span><span class="sxs-lookup"><span data-stu-id="e3a86-187">Using Teams APIs</span></span>](teams-api-overview.md)
