---
title: Тип ресурса Теамсаппинсталлатион
description: 'TeamsApp, установленный в команде, в чате или в личной области пользователя. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f5775514eb242f540bc6740d8e21620448f2d280
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563641"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="5f652-103">Тип ресурса Теамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="5f652-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="5f652-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f652-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f652-105">[TeamsApp](teamsapp.md) , установленный в [команде](team.md), в [чате](chat.md)или в личной области [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="5f652-105">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="5f652-106">Все боты, которые входят в состав приложения, станут частью любой группы, чата или пользователя, к которому добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="5f652-106">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="5f652-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5f652-107">Methods</span></span>

| <span data-ttu-id="5f652-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5f652-108">Method</span></span>       | <span data-ttu-id="5f652-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5f652-109">Return Type</span></span>  |<span data-ttu-id="5f652-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5f652-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5f652-111">Список приложений, установленных в Team</span><span class="sxs-lookup"><span data-stu-id="5f652-111">List apps installed in team</span></span>](../api/teamsappinstallation-list.md) | <span data-ttu-id="5f652-112">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="5f652-112">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="5f652-113">Список приложений, установленных в команде.</span><span class="sxs-lookup"><span data-stu-id="5f652-113">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="5f652-114">Получение приложения, установленного в команде</span><span class="sxs-lookup"><span data-stu-id="5f652-114">Get app installed in a team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="5f652-115">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="5f652-115">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="5f652-116">Список приложений, установленных в команде.</span><span class="sxs-lookup"><span data-stu-id="5f652-116">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="5f652-117">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="5f652-117">Add app to team</span></span>](../api/teamsappinstallation-add.md) |<span data-ttu-id="5f652-118">Нет</span><span class="sxs-lookup"><span data-stu-id="5f652-118">None</span></span> | <span data-ttu-id="5f652-119">Добавляет (устанавливает) приложение в команду.</span><span class="sxs-lookup"><span data-stu-id="5f652-119">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="5f652-120">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="5f652-120">Remove app from team</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="5f652-121">Нет</span><span class="sxs-lookup"><span data-stu-id="5f652-121">None</span></span> | <span data-ttu-id="5f652-122">Удаляет приложение из команды.</span><span class="sxs-lookup"><span data-stu-id="5f652-122">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="5f652-123">Обновление приложения, установленного в команде</span><span class="sxs-lookup"><span data-stu-id="5f652-123">Upgrade app installed in team</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="5f652-124">Нет</span><span class="sxs-lookup"><span data-stu-id="5f652-124">None</span></span> | <span data-ttu-id="5f652-125">Обновление до последней версии приложения, установленного в команде.</span><span class="sxs-lookup"><span data-stu-id="5f652-125">Upgrades to the latest version of the app installed in team.</span></span>|
|[<span data-ttu-id="5f652-126">Перечисление приложений, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="5f652-126">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md) | <span data-ttu-id="5f652-127">Коллекция [усерскопетеамсаппинсталлатион](userscopeteamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="5f652-127">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="5f652-128">Список приложений, установленных в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="5f652-128">Lists apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="5f652-129">Получает установленное приложение для пользователя</span><span class="sxs-lookup"><span data-stu-id="5f652-129">Gets the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="5f652-130">усерскопетеамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="5f652-130">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="5f652-131">Перечисление указанного приложения, установленного в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="5f652-131">Lists the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="5f652-132">Добавление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="5f652-132">Add app for user</span></span>](../api/userteamwork-add-installedapps.md) | | <span data-ttu-id="5f652-133">Добавляет (устанавливает) приложение в личную область пользователя.</span><span class="sxs-lookup"><span data-stu-id="5f652-133">Adds (installs) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="5f652-134">Удаление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="5f652-134">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="5f652-135">Нет</span><span class="sxs-lookup"><span data-stu-id="5f652-135">None</span></span> | <span data-ttu-id="5f652-136">Удаляет приложение из персональной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="5f652-136">Removes (uninstalls) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="5f652-137">Обновление приложения, установленного для пользователя</span><span class="sxs-lookup"><span data-stu-id="5f652-137">Upgrade app installed for user</span></span>](../api/userteamwork-upgrade-installedapps.md) | <span data-ttu-id="5f652-138">Нет</span><span class="sxs-lookup"><span data-stu-id="5f652-138">None</span></span> | <span data-ttu-id="5f652-139">Обновление до последней версии приложения, установленного в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="5f652-139">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="5f652-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f652-140">Properties</span></span>

| <span data-ttu-id="5f652-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f652-141">Property</span></span>            | <span data-ttu-id="5f652-142">Тип</span><span class="sxs-lookup"><span data-stu-id="5f652-142">Type</span></span>     | <span data-ttu-id="5f652-143">Описание</span><span class="sxs-lookup"><span data-stu-id="5f652-143">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="5f652-144">id</span><span class="sxs-lookup"><span data-stu-id="5f652-144">id</span></span>                  | <span data-ttu-id="5f652-145">string</span><span class="sxs-lookup"><span data-stu-id="5f652-145">string</span></span>   | <span data-ttu-id="5f652-146">Уникальный идентификатор (не идентификатор AP группы).</span><span class="sxs-lookup"><span data-stu-id="5f652-146">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="5f652-147">Связи</span><span class="sxs-lookup"><span data-stu-id="5f652-147">Relationships</span></span>

| <span data-ttu-id="5f652-148">Связь</span><span class="sxs-lookup"><span data-stu-id="5f652-148">Relationship</span></span>   | <span data-ttu-id="5f652-149">Тип</span><span class="sxs-lookup"><span data-stu-id="5f652-149">Type</span></span>    | <span data-ttu-id="5f652-150">Описание</span><span class="sxs-lookup"><span data-stu-id="5f652-150">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5f652-151">teamsApp</span><span class="sxs-lookup"><span data-stu-id="5f652-151">teamsApp</span></span>|[<span data-ttu-id="5f652-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="5f652-152">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="5f652-153">Установленное приложение.</span><span class="sxs-lookup"><span data-stu-id="5f652-153">The app that is installed.</span></span> |
|<span data-ttu-id="5f652-154">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="5f652-154">teamsAppDefinition</span></span>|[<span data-ttu-id="5f652-155">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="5f652-155">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="5f652-156">Сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="5f652-156">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5f652-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5f652-157">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="5f652-158">См. также</span><span class="sxs-lookup"><span data-stu-id="5f652-158">See also</span></span>

- [<span data-ttu-id="5f652-159">teamsApp</span><span class="sxs-lookup"><span data-stu-id="5f652-159">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="5f652-160">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="5f652-160">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="5f652-161">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5f652-161">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="5f652-162">усерскопетеамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="5f652-162">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

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


