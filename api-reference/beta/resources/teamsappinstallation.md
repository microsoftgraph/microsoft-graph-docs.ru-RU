---
title: Тип ресурса Теамсаппинсталлатион
description: 'TeamsApp, установленный в команде, в чате или в личной области пользователя. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9b34450f29ccb1fb02cf1751c78f312c71fdefc9
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606960"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="af5a9-103">Тип ресурса Теамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="af5a9-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="af5a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af5a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af5a9-105">[TeamsApp](teamsapp.md) , установленный в [команде](team.md), в [чате](chat.md)или в личной области [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="af5a9-105">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="af5a9-106">Все боты, которые входят в состав приложения, станут частью любой группы, чата или пользователя, к которому добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="af5a9-106">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

> [!NOTE]
> <span data-ttu-id="af5a9-107">`id`Ресурс **теамсаппинсталлатион** имеет не то же значение, что и `id` связанный ресурс **teamsApp** .</span><span class="sxs-lookup"><span data-stu-id="af5a9-107">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="methods"></a><span data-ttu-id="af5a9-108">Методы</span><span class="sxs-lookup"><span data-stu-id="af5a9-108">Methods</span></span>

| <span data-ttu-id="af5a9-109">Метод</span><span class="sxs-lookup"><span data-stu-id="af5a9-109">Method</span></span>       | <span data-ttu-id="af5a9-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="af5a9-110">Return Type</span></span>  |<span data-ttu-id="af5a9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="af5a9-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="af5a9-112">Список приложений, установленных в Team</span><span class="sxs-lookup"><span data-stu-id="af5a9-112">List apps installed in team</span></span>](../api/team-list-installedapps.md) | <span data-ttu-id="af5a9-113">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="af5a9-113">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="af5a9-114">Список приложений, установленных в команде.</span><span class="sxs-lookup"><span data-stu-id="af5a9-114">List apps installed in a team.</span></span>|
|[<span data-ttu-id="af5a9-115">Получение приложения, установленного в команде</span><span class="sxs-lookup"><span data-stu-id="af5a9-115">Get app installed in a team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="af5a9-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="af5a9-116">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="af5a9-117">Получение указанного приложения, установленного в команде.</span><span class="sxs-lookup"><span data-stu-id="af5a9-117">Get the specified app installed in a team.</span></span>|
|[<span data-ttu-id="af5a9-118">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="af5a9-118">Add app to team</span></span>](../api/team-post-installedapps.md) |<span data-ttu-id="af5a9-119">Нет</span><span class="sxs-lookup"><span data-stu-id="af5a9-119">None</span></span> | <span data-ttu-id="af5a9-120">Добавление приложения в группу (установка).</span><span class="sxs-lookup"><span data-stu-id="af5a9-120">Add (install) an app to a team.</span></span>|
|[<span data-ttu-id="af5a9-121">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="af5a9-121">Remove app from team</span></span>](../api/team-delete-installedapps.md) | <span data-ttu-id="af5a9-122">Нет</span><span class="sxs-lookup"><span data-stu-id="af5a9-122">None</span></span> | <span data-ttu-id="af5a9-123">Удаление приложения из команды (удаление).</span><span class="sxs-lookup"><span data-stu-id="af5a9-123">Remove (uninstall) an app from a team.</span></span>|
|[<span data-ttu-id="af5a9-124">Обновление приложения, установленного в команде</span><span class="sxs-lookup"><span data-stu-id="af5a9-124">Upgrade app installed in team</span></span>](../api/team-teamsappinstallation-upgrade.md) | <span data-ttu-id="af5a9-125">Нет</span><span class="sxs-lookup"><span data-stu-id="af5a9-125">None</span></span> | <span data-ttu-id="af5a9-126">Обновите приложение, установленное в команде, до последней версии.</span><span class="sxs-lookup"><span data-stu-id="af5a9-126">Upgrade the app installed in a team to the latest version.</span></span>|
|[<span data-ttu-id="af5a9-127">Перечисление приложений, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="af5a9-127">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md) | <span data-ttu-id="af5a9-128">Коллекция [усерскопетеамсаппинсталлатион](userscopeteamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="af5a9-128">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="af5a9-129">Список приложений, установленных в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="af5a9-129">List apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="af5a9-130">Получение приложения, установленного для пользователя</span><span class="sxs-lookup"><span data-stu-id="af5a9-130">Get the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="af5a9-131">усерскопетеамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="af5a9-131">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="af5a9-132">Получение указанного приложения, установленного в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="af5a9-132">Get the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="af5a9-133">Добавление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="af5a9-133">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | | <span data-ttu-id="af5a9-134">Добавление (установка) приложения в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="af5a9-134">Add (install) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="af5a9-135">Удаление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="af5a9-135">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="af5a9-136">Нет</span><span class="sxs-lookup"><span data-stu-id="af5a9-136">None</span></span> | <span data-ttu-id="af5a9-137">Удалить (удалить) приложение в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="af5a9-137">Remove (uninstall) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="af5a9-138">Обновление приложения, установленного для пользователя</span><span class="sxs-lookup"><span data-stu-id="af5a9-138">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="af5a9-139">Нет</span><span class="sxs-lookup"><span data-stu-id="af5a9-139">None</span></span> | <span data-ttu-id="af5a9-140">Обновление приложения, установленного в личной области пользователя, до последней версии.</span><span class="sxs-lookup"><span data-stu-id="af5a9-140">Upgrade the app installed in the personal scope of a user to the latest version.</span></span>|
|[<span data-ttu-id="af5a9-141">Перечисление приложений в чате</span><span class="sxs-lookup"><span data-stu-id="af5a9-141">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="af5a9-142">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="af5a9-142">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="af5a9-143">Список приложений, установленных в чате.</span><span class="sxs-lookup"><span data-stu-id="af5a9-143">List apps installed in a chat.</span></span>|
|[<span data-ttu-id="af5a9-144">Получение приложения в чате</span><span class="sxs-lookup"><span data-stu-id="af5a9-144">Get app in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="af5a9-145">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="af5a9-145">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="af5a9-146">Получение указанного приложения, установленного в чате.</span><span class="sxs-lookup"><span data-stu-id="af5a9-146">Get the specified app installed in a chat.</span></span>|
|[<span data-ttu-id="af5a9-147">Добавление приложения в чат</span><span class="sxs-lookup"><span data-stu-id="af5a9-147">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="af5a9-148">Добавление приложения в чат (установка).</span><span class="sxs-lookup"><span data-stu-id="af5a9-148">Add (install) an app to a chat.</span></span>|
|[<span data-ttu-id="af5a9-149">Удаление приложения из чата</span><span class="sxs-lookup"><span data-stu-id="af5a9-149">Remove app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="af5a9-150">Нет</span><span class="sxs-lookup"><span data-stu-id="af5a9-150">None</span></span> | <span data-ttu-id="af5a9-151">Удаление (удаление) приложения из чата.</span><span class="sxs-lookup"><span data-stu-id="af5a9-151">Remove (uninstall) app from a chat.</span></span>|
|[<span data-ttu-id="af5a9-152">Обновление приложения в чате</span><span class="sxs-lookup"><span data-stu-id="af5a9-152">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="af5a9-153">Нет</span><span class="sxs-lookup"><span data-stu-id="af5a9-153">None</span></span> | <span data-ttu-id="af5a9-154">Обновление приложения, установленного в чате, до последней версии.</span><span class="sxs-lookup"><span data-stu-id="af5a9-154">Upgrade the app installed in a chat to the latest version.</span></span>|

## <a name="properties"></a><span data-ttu-id="af5a9-155">Свойства</span><span class="sxs-lookup"><span data-stu-id="af5a9-155">Properties</span></span>

| <span data-ttu-id="af5a9-156">Свойство</span><span class="sxs-lookup"><span data-stu-id="af5a9-156">Property</span></span>            | <span data-ttu-id="af5a9-157">Тип</span><span class="sxs-lookup"><span data-stu-id="af5a9-157">Type</span></span>     | <span data-ttu-id="af5a9-158">Описание</span><span class="sxs-lookup"><span data-stu-id="af5a9-158">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="af5a9-159">id</span><span class="sxs-lookup"><span data-stu-id="af5a9-159">id</span></span>                  | <span data-ttu-id="af5a9-160">string</span><span class="sxs-lookup"><span data-stu-id="af5a9-160">string</span></span>   | <span data-ttu-id="af5a9-161">Уникальный идентификатор (не идентификатор AP группы).</span><span class="sxs-lookup"><span data-stu-id="af5a9-161">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="af5a9-162">Связи</span><span class="sxs-lookup"><span data-stu-id="af5a9-162">Relationships</span></span>

| <span data-ttu-id="af5a9-163">Связь</span><span class="sxs-lookup"><span data-stu-id="af5a9-163">Relationship</span></span>   | <span data-ttu-id="af5a9-164">Тип</span><span class="sxs-lookup"><span data-stu-id="af5a9-164">Type</span></span>    | <span data-ttu-id="af5a9-165">Описание</span><span class="sxs-lookup"><span data-stu-id="af5a9-165">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="af5a9-166">teamsApp</span><span class="sxs-lookup"><span data-stu-id="af5a9-166">teamsApp</span></span>|[<span data-ttu-id="af5a9-167">teamsApp</span><span class="sxs-lookup"><span data-stu-id="af5a9-167">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="af5a9-168">Установленное приложение.</span><span class="sxs-lookup"><span data-stu-id="af5a9-168">The app that is installed.</span></span> |
|<span data-ttu-id="af5a9-169">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="af5a9-169">teamsAppDefinition</span></span>|[<span data-ttu-id="af5a9-170">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="af5a9-170">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="af5a9-171">Сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="af5a9-171">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="af5a9-172">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="af5a9-172">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="af5a9-173">См. также</span><span class="sxs-lookup"><span data-stu-id="af5a9-173">See also</span></span>

- [<span data-ttu-id="af5a9-174">teamsApp</span><span class="sxs-lookup"><span data-stu-id="af5a9-174">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="af5a9-175">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="af5a9-175">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="af5a9-176">teamsTab</span><span class="sxs-lookup"><span data-stu-id="af5a9-176">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="af5a9-177">усерскопетеамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="af5a9-177">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


