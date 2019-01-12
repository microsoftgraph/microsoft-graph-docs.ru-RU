---
title: Тип ресурса группы
description: 'Группы в группах Microsoft — это коллекция каналов. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 7dff1bb05b2abe604963657d4691766eeeaae4ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976935"
---
# <a name="team-resource-type"></a><span data-ttu-id="c33f2-103">Тип ресурса группы</span><span class="sxs-lookup"><span data-stu-id="c33f2-103">team resource type</span></span>



<span data-ttu-id="c33f2-104">Группы в группах Microsoft — это коллекция [каналов](channel.md).</span><span class="sxs-lookup"><span data-stu-id="c33f2-104">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="c33f2-105">Канал представляет раздел и логическая изоляции обсуждения в группе.</span><span class="sxs-lookup"><span data-stu-id="c33f2-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="c33f2-106">Для любой группы связан с [группы](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="c33f2-106">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="c33f2-107">Группа имеет тот же идентификатор, как команда — например, /groups/ {идентификатор} / team совпадает с /teams/ {идентификатор}.</span><span class="sxs-lookup"><span data-stu-id="c33f2-107">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="c33f2-108">Дополнительные сведения о работе с группами и участниками групп показано [Использование интерфейса API REST графическое представление Microsoft для работы с группами Майкрософт](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="c33f2-108">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c33f2-109">Методы</span><span class="sxs-lookup"><span data-stu-id="c33f2-109">Methods</span></span>

| <span data-ttu-id="c33f2-110">Метод</span><span class="sxs-lookup"><span data-stu-id="c33f2-110">Method</span></span>       | <span data-ttu-id="c33f2-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c33f2-111">Return Type</span></span>  |<span data-ttu-id="c33f2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c33f2-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c33f2-113">Создание группы</span><span class="sxs-lookup"><span data-stu-id="c33f2-113">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="c33f2-114">Группа</span><span class="sxs-lookup"><span data-stu-id="c33f2-114">team</span></span>](team.md) | <span data-ttu-id="c33f2-115">Создание новой группы или добавление группы к существующей группе.</span><span class="sxs-lookup"><span data-stu-id="c33f2-115">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="c33f2-116">Получение группы</span><span class="sxs-lookup"><span data-stu-id="c33f2-116">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="c33f2-117">Группа</span><span class="sxs-lookup"><span data-stu-id="c33f2-117">team</span></span>](team.md) | <span data-ttu-id="c33f2-118">Извлечение свойств и связи из указанной группы.</span><span class="sxs-lookup"><span data-stu-id="c33f2-118">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="c33f2-119">Группа обновления</span><span class="sxs-lookup"><span data-stu-id="c33f2-119">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="c33f2-120">Группа</span><span class="sxs-lookup"><span data-stu-id="c33f2-120">team</span></span>](team.md) |<span data-ttu-id="c33f2-121">Обновление свойств указанной группы.</span><span class="sxs-lookup"><span data-stu-id="c33f2-121">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="c33f2-122">Удаление группы</span><span class="sxs-lookup"><span data-stu-id="c33f2-122">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="c33f2-123">Нет</span><span class="sxs-lookup"><span data-stu-id="c33f2-123">None</span></span> |<span data-ttu-id="c33f2-124">Удаление группы и его связанную группу.</span><span class="sxs-lookup"><span data-stu-id="c33f2-124">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="c33f2-125">Клонирование группы</span><span class="sxs-lookup"><span data-stu-id="c33f2-125">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="c33f2-126">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="c33f2-126">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="c33f2-127">Скопируйте группа и его связанную группу.</span><span class="sxs-lookup"><span data-stu-id="c33f2-127">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="c33f2-128">Группа архива</span><span class="sxs-lookup"><span data-stu-id="c33f2-128">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="c33f2-129">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="c33f2-129">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="c33f2-130">Поместите группа в состояние только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c33f2-130">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="c33f2-131">Unarchive группы</span><span class="sxs-lookup"><span data-stu-id="c33f2-131">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="c33f2-132">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="c33f2-132">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="c33f2-133">Восстановите группа в состояние чтение запись.</span><span class="sxs-lookup"><span data-stu-id="c33f2-133">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="c33f2-134">Список рабочих групп</span><span class="sxs-lookup"><span data-stu-id="c33f2-134">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="c33f2-135">семейства сайтов [групп](team.md)</span><span class="sxs-lookup"><span data-stu-id="c33f2-135">[team](team.md) collection</span></span> | <span data-ttu-id="c33f2-136">Список групп, которые вы являетесь членом.</span><span class="sxs-lookup"><span data-stu-id="c33f2-136">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="c33f2-137">Список всех групп</span><span class="sxs-lookup"><span data-stu-id="c33f2-137">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="c33f2-138">Коллекция объектов [group](group.md)</span><span class="sxs-lookup"><span data-stu-id="c33f2-138">[group](group.md) collection</span></span> | <span data-ttu-id="c33f2-139">Список всех групп, которые имеют группами.</span><span class="sxs-lookup"><span data-stu-id="c33f2-139">List all groups that have teams.</span></span> |
|[<span data-ttu-id="c33f2-140">Публикация приложений для вашей организации</span><span class="sxs-lookup"><span data-stu-id="c33f2-140">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="c33f2-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c33f2-141">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="c33f2-142">Создание групп приложений видимым только для вашей организации.</span><span class="sxs-lookup"><span data-stu-id="c33f2-142">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="c33f2-143">Добавление приложения в группу</span><span class="sxs-lookup"><span data-stu-id="c33f2-143">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="c33f2-144">teamsappinstallation</span><span class="sxs-lookup"><span data-stu-id="c33f2-144">teamsappinstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="c33f2-145">Добавляет (установить) приложения в группу.</span><span class="sxs-lookup"><span data-stu-id="c33f2-145">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="c33f2-146">Добавление вкладки канала</span><span class="sxs-lookup"><span data-stu-id="c33f2-146">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="c33f2-147">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c33f2-147">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="c33f2-148">Добавляет (установить) вкладки канал группы.</span><span class="sxs-lookup"><span data-stu-id="c33f2-148">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="c33f2-149">Свойства</span><span class="sxs-lookup"><span data-stu-id="c33f2-149">Properties</span></span>

| <span data-ttu-id="c33f2-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="c33f2-150">Property</span></span> | <span data-ttu-id="c33f2-151">Тип</span><span class="sxs-lookup"><span data-stu-id="c33f2-151">Type</span></span>   | <span data-ttu-id="c33f2-152">Описание</span><span class="sxs-lookup"><span data-stu-id="c33f2-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c33f2-153">funSettings</span><span class="sxs-lookup"><span data-stu-id="c33f2-153">funSettings</span></span>|[<span data-ttu-id="c33f2-154">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="c33f2-154">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="c33f2-155">Параметры для настройки использования Giphy, memes и наклейки рабочих групп.</span><span class="sxs-lookup"><span data-stu-id="c33f2-155">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="c33f2-156">guestSettings</span><span class="sxs-lookup"><span data-stu-id="c33f2-156">guestSettings</span></span>|[<span data-ttu-id="c33f2-157">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="c33f2-157">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="c33f2-158">Параметры для настройки ли гости могут создать, обновить или удалить каналы рабочих групп.</span><span class="sxs-lookup"><span data-stu-id="c33f2-158">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="c33f2-159">isArchived</span><span class="sxs-lookup"><span data-stu-id="c33f2-159">isArchived</span></span>|<span data-ttu-id="c33f2-160">Логический</span><span class="sxs-lookup"><span data-stu-id="c33f2-160">Boolean</span></span>|<span data-ttu-id="c33f2-161">Является ли эта группа в режиме только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c33f2-161">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="c33f2-162">memberSettings</span><span class="sxs-lookup"><span data-stu-id="c33f2-162">memberSettings</span></span>|[<span data-ttu-id="c33f2-163">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="c33f2-163">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="c33f2-164">Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, рабочих групп.</span><span class="sxs-lookup"><span data-stu-id="c33f2-164">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="c33f2-165">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="c33f2-165">messagingSettings</span></span>|[<span data-ttu-id="c33f2-166">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="c33f2-166">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="c33f2-167">Параметры для настройки системы обмена сообщениями и упоминания рабочих групп.</span><span class="sxs-lookup"><span data-stu-id="c33f2-167">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="c33f2-168">webUrl</span><span class="sxs-lookup"><span data-stu-id="c33f2-168">webUrl</span></span>|<span data-ttu-id="c33f2-169">String (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="c33f2-169">string (readonly)</span></span> | <span data-ttu-id="c33f2-170">Гиперссылка, будут поступать на группы в клиенте группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="c33f2-170">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="c33f2-171">Это URL-адрес, который вы получаете при щелкните правой кнопкой мыши группы в клиенте Microsoft группы и выберите **получить ссылку на группы**.</span><span class="sxs-lookup"><span data-stu-id="c33f2-171">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="c33f2-172">Этот URL-адрес должен быть обрабатываются как непрозрачный больших двоичных объектов и не синтаксический анализ.</span><span class="sxs-lookup"><span data-stu-id="c33f2-172">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c33f2-173">Связи</span><span class="sxs-lookup"><span data-stu-id="c33f2-173">Relationships</span></span>

| <span data-ttu-id="c33f2-174">Связь</span><span class="sxs-lookup"><span data-stu-id="c33f2-174">Relationship</span></span> | <span data-ttu-id="c33f2-175">Тип</span><span class="sxs-lookup"><span data-stu-id="c33f2-175">Type</span></span>   | <span data-ttu-id="c33f2-176">Описание</span><span class="sxs-lookup"><span data-stu-id="c33f2-176">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c33f2-177">каналы</span><span class="sxs-lookup"><span data-stu-id="c33f2-177">channels</span></span>|<span data-ttu-id="c33f2-178">Коллекция [канала](channel.md)</span><span class="sxs-lookup"><span data-stu-id="c33f2-178">[channel](channel.md) collection</span></span>|<span data-ttu-id="c33f2-179">Коллекция каналы & сообщения, связанный с группой.</span><span class="sxs-lookup"><span data-stu-id="c33f2-179">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="c33f2-180">installedApps</span><span class="sxs-lookup"><span data-stu-id="c33f2-180">installedApps</span></span>|<span data-ttu-id="c33f2-181">[teamsAppInstallation](teamsappinstallation.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c33f2-181">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="c33f2-182">Приложения, установленные в этой группе.</span><span class="sxs-lookup"><span data-stu-id="c33f2-182">The apps installed in this team.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c33f2-183">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c33f2-183">JSON representation</span></span>

<span data-ttu-id="c33f2-184">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c33f2-184">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="c33f2-185">См. также</span><span class="sxs-lookup"><span data-stu-id="c33f2-185">See Also</span></span>
- [<span data-ttu-id="c33f2-186">Создание группы с группой</span><span class="sxs-lookup"><span data-stu-id="c33f2-186">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="c33f2-187">Использование интерфейсов API групп</span><span class="sxs-lookup"><span data-stu-id="c33f2-187">Using Teams APIs</span></span>](teams-api-overview.md)
