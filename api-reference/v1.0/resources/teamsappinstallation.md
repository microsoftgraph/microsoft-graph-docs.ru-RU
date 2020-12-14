---
title: Тип ресурса teamsAppInstallation
description: Представляет приложение teamsApp, установленное в команде или в личной области пользователя.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: da55c4cf7b20558258493c69c46e2b26107f4aed
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660074"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="7af5e-103">Тип ресурса teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="7af5e-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="7af5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7af5e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7af5e-105">Представляет приложение [teamsApp,](teamsapp.md) установленное в [команде](team.md) или в личной области [пользователя.](user.md)</span><span class="sxs-lookup"><span data-stu-id="7af5e-105">Represents a [teamsApp](teamsapp.md) installed in a [team](team.md) or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="7af5e-106">Все боты, которые являются частью приложения, становятся частью любой команды или личной области пользователя, в которую добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="7af5e-106">Any bots that are part of the app will become part of any team or user's personal scope that the app is added to.</span></span>

> [!NOTE]
> <span data-ttu-id="7af5e-107">`id`Ресурс **teamsAppInstallation** имеет не то же значение, что и `id` связанный ресурс **teamsApp**.</span><span class="sxs-lookup"><span data-stu-id="7af5e-107">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="methods"></a><span data-ttu-id="7af5e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="7af5e-108">Methods</span></span>

| <span data-ttu-id="7af5e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="7af5e-109">Method</span></span>       | <span data-ttu-id="7af5e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7af5e-110">Return Type</span></span>  |<span data-ttu-id="7af5e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7af5e-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7af5e-112">Список приложений, установленных в команде</span><span class="sxs-lookup"><span data-stu-id="7af5e-112">List apps installed in team</span></span>](../api/team-list-installedapps.md) | <span data-ttu-id="7af5e-113">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="7af5e-113">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="7af5e-114">Список приложений, установленных в команде.</span><span class="sxs-lookup"><span data-stu-id="7af5e-114">List apps installed in a team.</span></span>|
|[<span data-ttu-id="7af5e-115">Как установить приложение в команде</span><span class="sxs-lookup"><span data-stu-id="7af5e-115">Get app installed in team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="7af5e-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="7af5e-116">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="7af5e-117">Получите указанное приложение, установленное в команде.</span><span class="sxs-lookup"><span data-stu-id="7af5e-117">Get the specified app installed in a team.</span></span>|
|[<span data-ttu-id="7af5e-118">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="7af5e-118">Add app to team</span></span>](../api/team-post-installedapps.md) |<span data-ttu-id="7af5e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="7af5e-119">None</span></span> | <span data-ttu-id="7af5e-120">Добавление (установка) приложения в команду.</span><span class="sxs-lookup"><span data-stu-id="7af5e-120">Add (install) an app to a team.</span></span>|
|[<span data-ttu-id="7af5e-121">Обновление приложения, установленного в команде</span><span class="sxs-lookup"><span data-stu-id="7af5e-121">Upgrade app installed in team</span></span>](../api/team-teamsappinstallation-upgrade.md) | <span data-ttu-id="7af5e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="7af5e-122">None</span></span> | <span data-ttu-id="7af5e-123">Обновив приложение, установленное в команде, до последней версии.</span><span class="sxs-lookup"><span data-stu-id="7af5e-123">Upgrade the app installed in a team to the latest version.</span></span>|
|[<span data-ttu-id="7af5e-124">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="7af5e-124">Remove app from team</span></span>](../api/team-delete-installedapps.md) | <span data-ttu-id="7af5e-125">Нет</span><span class="sxs-lookup"><span data-stu-id="7af5e-125">None</span></span> | <span data-ttu-id="7af5e-126">Удалите (удалите) приложение из команды.</span><span class="sxs-lookup"><span data-stu-id="7af5e-126">Remove (uninstall) an app from a team.</span></span>|
|[<span data-ttu-id="7af5e-127">Перечисление приложений, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="7af5e-127">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md) | <span data-ttu-id="7af5e-128">Коллекция [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="7af5e-128">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="7af5e-129">Список приложений, установленных в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="7af5e-129">List apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="7af5e-130">Как установить приложение для пользователя</span><span class="sxs-lookup"><span data-stu-id="7af5e-130">Get app installed for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="7af5e-131">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="7af5e-131">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="7af5e-132">Получите указанное приложение, установленное в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="7af5e-132">Get the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="7af5e-133">Добавление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="7af5e-133">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | | <span data-ttu-id="7af5e-134">Добавление (установка) приложения в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="7af5e-134">Add (install) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="7af5e-135">Обновление приложения, установленного для пользователя</span><span class="sxs-lookup"><span data-stu-id="7af5e-135">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="7af5e-136">Нет</span><span class="sxs-lookup"><span data-stu-id="7af5e-136">None</span></span> | <span data-ttu-id="7af5e-137">Обновив приложение, установленное в личной области пользователя, до последней версии.</span><span class="sxs-lookup"><span data-stu-id="7af5e-137">Upgrade the app installed in the personal scope of a user to the latest version.</span></span>|
|[<span data-ttu-id="7af5e-138">Удаление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="7af5e-138">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="7af5e-139">Нет</span><span class="sxs-lookup"><span data-stu-id="7af5e-139">None</span></span> | <span data-ttu-id="7af5e-140">Удалите (удалите) приложение в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="7af5e-140">Remove (uninstall) an app in the personal scope of a user.</span></span>|


## <a name="properties"></a><span data-ttu-id="7af5e-141">Свойства</span><span class="sxs-lookup"><span data-stu-id="7af5e-141">Properties</span></span>

| <span data-ttu-id="7af5e-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="7af5e-142">Property</span></span>            | <span data-ttu-id="7af5e-143">Тип</span><span class="sxs-lookup"><span data-stu-id="7af5e-143">Type</span></span>     | <span data-ttu-id="7af5e-144">Описание</span><span class="sxs-lookup"><span data-stu-id="7af5e-144">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="7af5e-145">id</span><span class="sxs-lookup"><span data-stu-id="7af5e-145">id</span></span>                  | <span data-ttu-id="7af5e-146">string</span><span class="sxs-lookup"><span data-stu-id="7af5e-146">string</span></span>   | <span data-ttu-id="7af5e-147">Уникальный ИД (а не ИД приложения Teams).</span><span class="sxs-lookup"><span data-stu-id="7af5e-147">A unique ID (not the Teams app ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="7af5e-148">Связи</span><span class="sxs-lookup"><span data-stu-id="7af5e-148">Relationships</span></span>

| <span data-ttu-id="7af5e-149">Связь</span><span class="sxs-lookup"><span data-stu-id="7af5e-149">Relationship</span></span>   | <span data-ttu-id="7af5e-150">Тип</span><span class="sxs-lookup"><span data-stu-id="7af5e-150">Type</span></span>    | <span data-ttu-id="7af5e-151">Описание</span><span class="sxs-lookup"><span data-stu-id="7af5e-151">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7af5e-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="7af5e-152">teamsApp</span></span>|[<span data-ttu-id="7af5e-153">teamsApp</span><span class="sxs-lookup"><span data-stu-id="7af5e-153">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="7af5e-154">Установленное приложение.</span><span class="sxs-lookup"><span data-stu-id="7af5e-154">The app that is installed.</span></span> |
|<span data-ttu-id="7af5e-155">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="7af5e-155">teamsAppDefinition</span></span>|[<span data-ttu-id="7af5e-156">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="7af5e-156">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="7af5e-157">Сведения об этой версии приложения.</span><span class="sxs-lookup"><span data-stu-id="7af5e-157">The details of this version of the app.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="7af5e-158">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7af5e-158">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="7af5e-159">См. также</span><span class="sxs-lookup"><span data-stu-id="7af5e-159">See also</span></span>

- [<span data-ttu-id="7af5e-160">teamsApp</span><span class="sxs-lookup"><span data-stu-id="7af5e-160">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="7af5e-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="7af5e-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="7af5e-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7af5e-162">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="7af5e-163">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="7af5e-163">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
  "suppressions": []
}-->

