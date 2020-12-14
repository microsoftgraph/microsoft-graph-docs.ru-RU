---
title: Тип ресурса teamsAppInstallation
description: 'Приложение teamsApp, установленное в команде, чате или личной области пользователя. '
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 66cf31f21a105934181aee5e506cc2215f9ce7a9
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663913"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="8d1af-103">Тип ресурса teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="8d1af-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="8d1af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d1af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d1af-105">Приложение [teamsApp,](teamsapp.md) установленное в [команде,](team.md) [чате](chat.md)или личной области [пользователя.](user.md)</span><span class="sxs-lookup"><span data-stu-id="8d1af-105">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="8d1af-106">Все боты, которые являются частью приложения, становятся частью любой команды, чата или личной области пользователя, в которую добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="8d1af-106">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

> [!NOTE]
> <span data-ttu-id="8d1af-107">`id`Ресурс **teamsAppInstallation** имеет не то же значение, что и `id` связанный ресурс **teamsApp**.</span><span class="sxs-lookup"><span data-stu-id="8d1af-107">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="methods"></a><span data-ttu-id="8d1af-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8d1af-108">Methods</span></span>

| <span data-ttu-id="8d1af-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8d1af-109">Method</span></span>       | <span data-ttu-id="8d1af-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8d1af-110">Return Type</span></span>  |<span data-ttu-id="8d1af-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8d1af-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8d1af-112">Список приложений, установленных в команде</span><span class="sxs-lookup"><span data-stu-id="8d1af-112">List apps installed in team</span></span>](../api/team-list-installedapps.md) | <span data-ttu-id="8d1af-113">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="8d1af-113">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="8d1af-114">Список приложений, установленных в команде.</span><span class="sxs-lookup"><span data-stu-id="8d1af-114">List apps installed in a team.</span></span>|
|[<span data-ttu-id="8d1af-115">Как установить приложение в команде</span><span class="sxs-lookup"><span data-stu-id="8d1af-115">Get app installed in team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="8d1af-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="8d1af-116">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="8d1af-117">Получите указанное приложение, установленное в команде.</span><span class="sxs-lookup"><span data-stu-id="8d1af-117">Get the specified app installed in a team.</span></span>|
|[<span data-ttu-id="8d1af-118">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="8d1af-118">Add app to team</span></span>](../api/team-post-installedapps.md) |<span data-ttu-id="8d1af-119">Нет</span><span class="sxs-lookup"><span data-stu-id="8d1af-119">None</span></span> | <span data-ttu-id="8d1af-120">Добавление (установка) приложения в команду.</span><span class="sxs-lookup"><span data-stu-id="8d1af-120">Add (install) an app to a team.</span></span>|
|[<span data-ttu-id="8d1af-121">Обновление приложения, установленного в команде</span><span class="sxs-lookup"><span data-stu-id="8d1af-121">Upgrade app installed in team</span></span>](../api/team-teamsappinstallation-upgrade.md) | <span data-ttu-id="8d1af-122">Нет</span><span class="sxs-lookup"><span data-stu-id="8d1af-122">None</span></span> | <span data-ttu-id="8d1af-123">Обновив приложение, установленное в команде, до последней версии.</span><span class="sxs-lookup"><span data-stu-id="8d1af-123">Upgrade the app installed in a team to the latest version.</span></span>|
|[<span data-ttu-id="8d1af-124">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="8d1af-124">Remove app from team</span></span>](../api/team-delete-installedapps.md) | <span data-ttu-id="8d1af-125">Нет</span><span class="sxs-lookup"><span data-stu-id="8d1af-125">None</span></span> | <span data-ttu-id="8d1af-126">Удалите (удалите) приложение из команды.</span><span class="sxs-lookup"><span data-stu-id="8d1af-126">Remove (uninstall) an app from a team.</span></span>|
|[<span data-ttu-id="8d1af-127">Перечисление приложений, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="8d1af-127">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md) | <span data-ttu-id="8d1af-128">Коллекция [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="8d1af-128">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="8d1af-129">Список приложений, установленных в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="8d1af-129">List apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="8d1af-130">Как установить приложение для пользователя</span><span class="sxs-lookup"><span data-stu-id="8d1af-130">Get app installed for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="8d1af-131">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="8d1af-131">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="8d1af-132">Получите указанное приложение, установленное в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="8d1af-132">Get the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="8d1af-133">Добавление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="8d1af-133">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | | <span data-ttu-id="8d1af-134">Добавление (установка) приложения в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="8d1af-134">Add (install) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="8d1af-135">Обновление приложения, установленного для пользователя</span><span class="sxs-lookup"><span data-stu-id="8d1af-135">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="8d1af-136">Нет</span><span class="sxs-lookup"><span data-stu-id="8d1af-136">None</span></span> | <span data-ttu-id="8d1af-137">Обновив приложение, установленное в личной области пользователя, до последней версии.</span><span class="sxs-lookup"><span data-stu-id="8d1af-137">Upgrade the app installed in the personal scope of a user to the latest version.</span></span>|
|[<span data-ttu-id="8d1af-138">Удаление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="8d1af-138">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="8d1af-139">Нет</span><span class="sxs-lookup"><span data-stu-id="8d1af-139">None</span></span> | <span data-ttu-id="8d1af-140">Удалите (удалите) приложение в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="8d1af-140">Remove (uninstall) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="8d1af-141">Список приложений в каталоге</span><span class="sxs-lookup"><span data-stu-id="8d1af-141">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="8d1af-142">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="8d1af-142">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="8d1af-143">Список приложений, установленных в чате.</span><span class="sxs-lookup"><span data-stu-id="8d1af-143">List apps installed in a chat.</span></span>|
|[<span data-ttu-id="8d1af-144">Как установить приложение в чате</span><span class="sxs-lookup"><span data-stu-id="8d1af-144">Get app installed in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="8d1af-145">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="8d1af-145">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="8d1af-146">Получите указанное приложение, установленное в чате.</span><span class="sxs-lookup"><span data-stu-id="8d1af-146">Get the specified app installed in a chat.</span></span>|
|[<span data-ttu-id="8d1af-147">Добавление приложения в чате</span><span class="sxs-lookup"><span data-stu-id="8d1af-147">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="8d1af-148">Добавление (установка) приложения в чат.</span><span class="sxs-lookup"><span data-stu-id="8d1af-148">Add (install) an app to a chat.</span></span>|
|[<span data-ttu-id="8d1af-149">Обновление приложения в чате</span><span class="sxs-lookup"><span data-stu-id="8d1af-149">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="8d1af-150">Нет</span><span class="sxs-lookup"><span data-stu-id="8d1af-150">None</span></span> | <span data-ttu-id="8d1af-151">Обновив приложение, установленное в чате, до последней версии.</span><span class="sxs-lookup"><span data-stu-id="8d1af-151">Upgrade the app installed in a chat to the latest version.</span></span>|
|[<span data-ttu-id="8d1af-152">Удаление приложения из чата</span><span class="sxs-lookup"><span data-stu-id="8d1af-152">Remove app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="8d1af-153">Нет</span><span class="sxs-lookup"><span data-stu-id="8d1af-153">None</span></span> | <span data-ttu-id="8d1af-154">Удаление приложения из чата.</span><span class="sxs-lookup"><span data-stu-id="8d1af-154">Remove (uninstall) app from a chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="8d1af-155">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d1af-155">Properties</span></span>

| <span data-ttu-id="8d1af-156">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d1af-156">Property</span></span>            | <span data-ttu-id="8d1af-157">Тип</span><span class="sxs-lookup"><span data-stu-id="8d1af-157">Type</span></span>     | <span data-ttu-id="8d1af-158">Описание</span><span class="sxs-lookup"><span data-stu-id="8d1af-158">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="8d1af-159">id</span><span class="sxs-lookup"><span data-stu-id="8d1af-159">id</span></span>                  | <span data-ttu-id="8d1af-160">string</span><span class="sxs-lookup"><span data-stu-id="8d1af-160">string</span></span>   | <span data-ttu-id="8d1af-161">Уникальный ИД (а не ap-ИД команды).</span><span class="sxs-lookup"><span data-stu-id="8d1af-161">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="8d1af-162">Связи</span><span class="sxs-lookup"><span data-stu-id="8d1af-162">Relationships</span></span>

| <span data-ttu-id="8d1af-163">Связь</span><span class="sxs-lookup"><span data-stu-id="8d1af-163">Relationship</span></span>   | <span data-ttu-id="8d1af-164">Тип</span><span class="sxs-lookup"><span data-stu-id="8d1af-164">Type</span></span>    | <span data-ttu-id="8d1af-165">Описание</span><span class="sxs-lookup"><span data-stu-id="8d1af-165">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8d1af-166">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8d1af-166">teamsApp</span></span>|[<span data-ttu-id="8d1af-167">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8d1af-167">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="8d1af-168">Установленное приложение.</span><span class="sxs-lookup"><span data-stu-id="8d1af-168">The app that is installed.</span></span> |
|<span data-ttu-id="8d1af-169">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="8d1af-169">teamsAppDefinition</span></span>|[<span data-ttu-id="8d1af-170">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="8d1af-170">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="8d1af-171">Сведения об этой версии приложения.</span><span class="sxs-lookup"><span data-stu-id="8d1af-171">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8d1af-172">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8d1af-172">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="8d1af-173">См. также</span><span class="sxs-lookup"><span data-stu-id="8d1af-173">See also</span></span>

- [<span data-ttu-id="8d1af-174">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8d1af-174">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="8d1af-175">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="8d1af-175">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="8d1af-176">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8d1af-176">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="8d1af-177">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="8d1af-177">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

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


