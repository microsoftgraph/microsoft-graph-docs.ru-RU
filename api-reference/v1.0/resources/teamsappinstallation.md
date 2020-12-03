---
title: Тип ресурса Теамсаппинсталлатион
description: Представляет teamsApp, установленный в команде или персональную область пользователя.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0d15f65273504b3b7577c875fec69c5a212a8c76
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563753"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="05b65-103">Тип ресурса Теамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="05b65-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="05b65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05b65-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05b65-105">Представляет [teamsApp](teamsapp.md) , установленный в [команде](team.md) или персональную область [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="05b65-105">Represents a [teamsApp](teamsapp.md) installed in a [team](team.md) or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="05b65-106">Все боты, которые входят в состав приложения, станут частью любой рабочей группы или пользователя, к которому добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="05b65-106">Any bots that are part of the app will become part of any team or user's personal scope that the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="05b65-107">Методы</span><span class="sxs-lookup"><span data-stu-id="05b65-107">Methods</span></span>

| <span data-ttu-id="05b65-108">Метод</span><span class="sxs-lookup"><span data-stu-id="05b65-108">Method</span></span>       | <span data-ttu-id="05b65-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="05b65-109">Return Type</span></span>  |<span data-ttu-id="05b65-110">Описание</span><span class="sxs-lookup"><span data-stu-id="05b65-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="05b65-111">Список приложений, установленных в Team</span><span class="sxs-lookup"><span data-stu-id="05b65-111">List apps installed in team</span></span>](../api/teamsappinstallation-list.md) | <span data-ttu-id="05b65-112">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="05b65-112">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="05b65-113">Список приложений, установленных в команде.</span><span class="sxs-lookup"><span data-stu-id="05b65-113">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="05b65-114">Получение приложения, установленного в команде</span><span class="sxs-lookup"><span data-stu-id="05b65-114">Get app installed in a team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="05b65-115">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="05b65-115">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="05b65-116">Список приложений, установленных в команде.</span><span class="sxs-lookup"><span data-stu-id="05b65-116">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="05b65-117">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="05b65-117">Add app to team</span></span>](../api/teamsappinstallation-add.md) | <span data-ttu-id="05b65-118">Нет</span><span class="sxs-lookup"><span data-stu-id="05b65-118">None</span></span> | <span data-ttu-id="05b65-119">Добавляет (устанавливает) приложение в команду.</span><span class="sxs-lookup"><span data-stu-id="05b65-119">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="05b65-120">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="05b65-120">Remove app from team</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="05b65-121">Нет</span><span class="sxs-lookup"><span data-stu-id="05b65-121">None</span></span> | <span data-ttu-id="05b65-122">Удаляет приложение из команды.</span><span class="sxs-lookup"><span data-stu-id="05b65-122">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="05b65-123">Обновление приложения, установленного в команде</span><span class="sxs-lookup"><span data-stu-id="05b65-123">Upgrade app installed in team</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="05b65-124">Нет</span><span class="sxs-lookup"><span data-stu-id="05b65-124">None</span></span> | <span data-ttu-id="05b65-125">Обновление до последней версии приложения, установленного в команде.</span><span class="sxs-lookup"><span data-stu-id="05b65-125">Upgrades to the latest version of the app installed in team.</span></span>|
|[<span data-ttu-id="05b65-126">Перечисление приложений, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="05b65-126">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md)| <span data-ttu-id="05b65-127">Коллекция [усерскопетеамсаппинсталлатион](userscopeteamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="05b65-127">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="05b65-128">Список приложений, установленных в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="05b65-128">Lists apps installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="05b65-129">Получает установленное приложение для пользователя</span><span class="sxs-lookup"><span data-stu-id="05b65-129">Gets the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="05b65-130">усерскопетеамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="05b65-130">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="05b65-131">Перечисление указанного приложения, установленного в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="05b65-131">Lists the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="05b65-132">Добавление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="05b65-132">Add app for user</span></span>](../api/userteamwork-add-installedapps.md) | <span data-ttu-id="05b65-133">Нет</span><span class="sxs-lookup"><span data-stu-id="05b65-133">None</span></span> | <span data-ttu-id="05b65-134">Добавляет (устанавливает) приложение в личную область пользователя.</span><span class="sxs-lookup"><span data-stu-id="05b65-134">Adds (installs) an app in the personal scope of a user.</span></span> |
|[<span data-ttu-id="05b65-135">Удаление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="05b65-135">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="05b65-136">Нет</span><span class="sxs-lookup"><span data-stu-id="05b65-136">None</span></span> | <span data-ttu-id="05b65-137">Удаляет приложение из персональной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="05b65-137">Removes (uninstalls) an app from the personal scope of a user.</span></span> |
|[<span data-ttu-id="05b65-138">Обновление приложения, установленного для пользователя</span><span class="sxs-lookup"><span data-stu-id="05b65-138">Upgrade app installed for user</span></span>](../api/userteamwork-upgrade-installedapps.md) | <span data-ttu-id="05b65-139">Нет</span><span class="sxs-lookup"><span data-stu-id="05b65-139">None</span></span> | <span data-ttu-id="05b65-140">Обновление до последней версии приложения, установленного в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="05b65-140">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="05b65-141">Свойства</span><span class="sxs-lookup"><span data-stu-id="05b65-141">Properties</span></span>

| <span data-ttu-id="05b65-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="05b65-142">Property</span></span>            | <span data-ttu-id="05b65-143">Тип</span><span class="sxs-lookup"><span data-stu-id="05b65-143">Type</span></span>     | <span data-ttu-id="05b65-144">Описание</span><span class="sxs-lookup"><span data-stu-id="05b65-144">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="05b65-145">id</span><span class="sxs-lookup"><span data-stu-id="05b65-145">id</span></span>                  | <span data-ttu-id="05b65-146">string</span><span class="sxs-lookup"><span data-stu-id="05b65-146">string</span></span>   | <span data-ttu-id="05b65-147">Уникальный идентификатор (а не идентификаторы Teams).</span><span class="sxs-lookup"><span data-stu-id="05b65-147">A unique ID (not the Teams appID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="05b65-148">Связи</span><span class="sxs-lookup"><span data-stu-id="05b65-148">Relationships</span></span>

| <span data-ttu-id="05b65-149">Связь</span><span class="sxs-lookup"><span data-stu-id="05b65-149">Relationship</span></span>   | <span data-ttu-id="05b65-150">Тип</span><span class="sxs-lookup"><span data-stu-id="05b65-150">Type</span></span>    | <span data-ttu-id="05b65-151">Описание</span><span class="sxs-lookup"><span data-stu-id="05b65-151">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="05b65-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="05b65-152">teamsApp</span></span>|[<span data-ttu-id="05b65-153">teamsApp</span><span class="sxs-lookup"><span data-stu-id="05b65-153">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="05b65-154">Установленное приложение.</span><span class="sxs-lookup"><span data-stu-id="05b65-154">The app that is installed.</span></span> |
|<span data-ttu-id="05b65-155">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="05b65-155">teamsAppDefinition</span></span>|[<span data-ttu-id="05b65-156">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="05b65-156">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="05b65-157">Сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="05b65-157">The details of this version of the app.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="05b65-158">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="05b65-158">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="05b65-159">См. также</span><span class="sxs-lookup"><span data-stu-id="05b65-159">See also</span></span>

- [<span data-ttu-id="05b65-160">teamsApp</span><span class="sxs-lookup"><span data-stu-id="05b65-160">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="05b65-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="05b65-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="05b65-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="05b65-162">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="05b65-163">усерскопетеамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="05b65-163">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

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

