---
title: Тип ресурса Теамсаппинсталлатион
description: Представляет teamsApp, установленный в команде или персональную область пользователя.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1c872d41ebc09978d9dc54ac01d82cb33258541d
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607037"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="0fc11-103">Тип ресурса Теамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="0fc11-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="0fc11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fc11-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0fc11-105">Представляет [teamsApp](teamsapp.md) , установленный в [команде](team.md) или персональную область [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="0fc11-105">Represents a [teamsApp](teamsapp.md) installed in a [team](team.md) or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="0fc11-106">Все боты, которые входят в состав приложения, станут частью любой рабочей группы или пользователя, к которому добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="0fc11-106">Any bots that are part of the app will become part of any team or user's personal scope that the app is added to.</span></span>

> [!NOTE]
> <span data-ttu-id="0fc11-107">`id`Ресурс **теамсаппинсталлатион** имеет не то же значение, что и `id` связанный ресурс **teamsApp** .</span><span class="sxs-lookup"><span data-stu-id="0fc11-107">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="methods"></a><span data-ttu-id="0fc11-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0fc11-108">Methods</span></span>

| <span data-ttu-id="0fc11-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0fc11-109">Method</span></span>       | <span data-ttu-id="0fc11-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0fc11-110">Return Type</span></span>  |<span data-ttu-id="0fc11-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0fc11-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0fc11-112">Список приложений, установленных в Team</span><span class="sxs-lookup"><span data-stu-id="0fc11-112">List apps installed in team</span></span>](../api/team-list-installedapps.md) | <span data-ttu-id="0fc11-113">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="0fc11-113">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="0fc11-114">Список приложений, установленных в команде.</span><span class="sxs-lookup"><span data-stu-id="0fc11-114">List apps installed in a team.</span></span>|
|[<span data-ttu-id="0fc11-115">Получение приложения, установленного в команде</span><span class="sxs-lookup"><span data-stu-id="0fc11-115">Get app installed in a team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="0fc11-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="0fc11-116">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="0fc11-117">Получение указанного приложения, установленного в команде.</span><span class="sxs-lookup"><span data-stu-id="0fc11-117">Get the specified app installed in a team.</span></span>|
|[<span data-ttu-id="0fc11-118">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="0fc11-118">Add app to team</span></span>](../api/team-post-installedapps.md) |<span data-ttu-id="0fc11-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0fc11-119">None</span></span> | <span data-ttu-id="0fc11-120">Добавление приложения в группу (установка).</span><span class="sxs-lookup"><span data-stu-id="0fc11-120">Add (install) an app to a team.</span></span>|
|[<span data-ttu-id="0fc11-121">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="0fc11-121">Remove app from team</span></span>](../api/team-delete-installedapps.md) | <span data-ttu-id="0fc11-122">Нет</span><span class="sxs-lookup"><span data-stu-id="0fc11-122">None</span></span> | <span data-ttu-id="0fc11-123">Удаление приложения из команды (удаление).</span><span class="sxs-lookup"><span data-stu-id="0fc11-123">Remove (uninstall) an app from a team.</span></span>|
|[<span data-ttu-id="0fc11-124">Обновление приложения, установленного в команде</span><span class="sxs-lookup"><span data-stu-id="0fc11-124">Upgrade app installed in team</span></span>](../api/team-teamsappinstallation-upgrade.md) | <span data-ttu-id="0fc11-125">Нет</span><span class="sxs-lookup"><span data-stu-id="0fc11-125">None</span></span> | <span data-ttu-id="0fc11-126">Обновите приложение, установленное в команде, до последней версии.</span><span class="sxs-lookup"><span data-stu-id="0fc11-126">Upgrade the app installed in a team to the latest version.</span></span>|
|[<span data-ttu-id="0fc11-127">Перечисление приложений, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="0fc11-127">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md) | <span data-ttu-id="0fc11-128">Коллекция [усерскопетеамсаппинсталлатион](userscopeteamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="0fc11-128">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="0fc11-129">Список приложений, установленных в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="0fc11-129">List apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="0fc11-130">Получение приложения, установленного для пользователя</span><span class="sxs-lookup"><span data-stu-id="0fc11-130">Get the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="0fc11-131">усерскопетеамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="0fc11-131">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="0fc11-132">Получение указанного приложения, установленного в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="0fc11-132">Get the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="0fc11-133">Добавление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="0fc11-133">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | | <span data-ttu-id="0fc11-134">Добавление (установка) приложения в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="0fc11-134">Add (install) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="0fc11-135">Удаление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="0fc11-135">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="0fc11-136">Нет</span><span class="sxs-lookup"><span data-stu-id="0fc11-136">None</span></span> | <span data-ttu-id="0fc11-137">Удалить (удалить) приложение в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="0fc11-137">Remove (uninstall) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="0fc11-138">Обновление приложения, установленного для пользователя</span><span class="sxs-lookup"><span data-stu-id="0fc11-138">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="0fc11-139">Нет</span><span class="sxs-lookup"><span data-stu-id="0fc11-139">None</span></span> | <span data-ttu-id="0fc11-140">Обновление приложения, установленного в личной области пользователя, до последней версии.</span><span class="sxs-lookup"><span data-stu-id="0fc11-140">Upgrade the app installed in the personal scope of a user to the latest version.</span></span>|


## <a name="properties"></a><span data-ttu-id="0fc11-141">Свойства</span><span class="sxs-lookup"><span data-stu-id="0fc11-141">Properties</span></span>

| <span data-ttu-id="0fc11-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="0fc11-142">Property</span></span>            | <span data-ttu-id="0fc11-143">Тип</span><span class="sxs-lookup"><span data-stu-id="0fc11-143">Type</span></span>     | <span data-ttu-id="0fc11-144">Описание</span><span class="sxs-lookup"><span data-stu-id="0fc11-144">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="0fc11-145">id</span><span class="sxs-lookup"><span data-stu-id="0fc11-145">id</span></span>                  | <span data-ttu-id="0fc11-146">string</span><span class="sxs-lookup"><span data-stu-id="0fc11-146">string</span></span>   | <span data-ttu-id="0fc11-147">Уникальный идентификатор (не идентификатор приложения Teams).</span><span class="sxs-lookup"><span data-stu-id="0fc11-147">A unique ID (not the Teams app ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="0fc11-148">Связи</span><span class="sxs-lookup"><span data-stu-id="0fc11-148">Relationships</span></span>

| <span data-ttu-id="0fc11-149">Связь</span><span class="sxs-lookup"><span data-stu-id="0fc11-149">Relationship</span></span>   | <span data-ttu-id="0fc11-150">Тип</span><span class="sxs-lookup"><span data-stu-id="0fc11-150">Type</span></span>    | <span data-ttu-id="0fc11-151">Описание</span><span class="sxs-lookup"><span data-stu-id="0fc11-151">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0fc11-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0fc11-152">teamsApp</span></span>|[<span data-ttu-id="0fc11-153">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0fc11-153">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="0fc11-154">Установленное приложение.</span><span class="sxs-lookup"><span data-stu-id="0fc11-154">The app that is installed.</span></span> |
|<span data-ttu-id="0fc11-155">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="0fc11-155">teamsAppDefinition</span></span>|[<span data-ttu-id="0fc11-156">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="0fc11-156">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="0fc11-157">Сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="0fc11-157">The details of this version of the app.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="0fc11-158">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0fc11-158">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="0fc11-159">См. также</span><span class="sxs-lookup"><span data-stu-id="0fc11-159">See also</span></span>

- [<span data-ttu-id="0fc11-160">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0fc11-160">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="0fc11-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="0fc11-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="0fc11-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0fc11-162">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="0fc11-163">усерскопетеамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="0fc11-163">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

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

