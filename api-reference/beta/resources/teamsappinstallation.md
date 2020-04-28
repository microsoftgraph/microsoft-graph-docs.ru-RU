---
title: Тип ресурса Теамсаппинсталлатион
description: 'TeamsApp, установленный в команде, в чате или в личной области пользователя. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 10a7d5d58a18e23c47d603e7b05c9981ddfeed76
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519913"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="83569-103">Тип ресурса Теамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="83569-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="83569-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83569-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83569-105">[TeamsApp](teamsapp.md) , установленный в [команде](team.md), в [чате](chat.md)или в личной области [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="83569-105">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="83569-106">Все боты, которые входят в состав приложения, станут частью любой группы, чата или пользователя, к которому добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="83569-106">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="83569-107">Методы</span><span class="sxs-lookup"><span data-stu-id="83569-107">Methods</span></span>

| <span data-ttu-id="83569-108">Метод</span><span class="sxs-lookup"><span data-stu-id="83569-108">Method</span></span>       | <span data-ttu-id="83569-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="83569-109">Return Type</span></span>  |<span data-ttu-id="83569-110">Описание</span><span class="sxs-lookup"><span data-stu-id="83569-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="83569-111">Список приложений, установленных в Team</span><span class="sxs-lookup"><span data-stu-id="83569-111">List apps installed in team</span></span>](../api/teamsappinstallation-list.md) | <span data-ttu-id="83569-112">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="83569-112">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="83569-113">Список приложений, установленных в команде.</span><span class="sxs-lookup"><span data-stu-id="83569-113">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="83569-114">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="83569-114">Add app to team</span></span>](../api/teamsappinstallation-add.md) |<span data-ttu-id="83569-115">Нет</span><span class="sxs-lookup"><span data-stu-id="83569-115">None</span></span> | <span data-ttu-id="83569-116">Добавляет (устанавливает) приложение в команду.</span><span class="sxs-lookup"><span data-stu-id="83569-116">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="83569-117">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="83569-117">Remove app from team</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="83569-118">Нет</span><span class="sxs-lookup"><span data-stu-id="83569-118">None</span></span> | <span data-ttu-id="83569-119">Удаляет приложение из команды.</span><span class="sxs-lookup"><span data-stu-id="83569-119">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="83569-120">Обновление приложения, установленного в команде</span><span class="sxs-lookup"><span data-stu-id="83569-120">Upgrade app installed in team</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="83569-121">Нет</span><span class="sxs-lookup"><span data-stu-id="83569-121">None</span></span> | <span data-ttu-id="83569-122">Обновление до последней версии приложения, установленного в команде.</span><span class="sxs-lookup"><span data-stu-id="83569-122">Upgrades to the latest version of the app installed in team.</span></span>|
|[<span data-ttu-id="83569-123">Перечисление приложений, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="83569-123">List apps installed for user</span></span>](../api/user-list-teamsappinstallation.md) | <span data-ttu-id="83569-124">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="83569-124">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="83569-125">Список приложений, установленных в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="83569-125">Lists apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="83569-126">Добавление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="83569-126">Add app for user</span></span>](../api/user-add-teamsappinstallation.md) | | <span data-ttu-id="83569-127">Добавляет (устанавливает) приложение в личную область пользователя.</span><span class="sxs-lookup"><span data-stu-id="83569-127">Adds (installs) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="83569-128">Удаление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="83569-128">Remove app for user</span></span>](../api/user-delete-teamsappinstallation.md) | <span data-ttu-id="83569-129">Нет</span><span class="sxs-lookup"><span data-stu-id="83569-129">None</span></span> | <span data-ttu-id="83569-130">Удаляет приложение из персональной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="83569-130">Removes (uninstalls) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="83569-131">Обновление приложения, установленного для пользователя</span><span class="sxs-lookup"><span data-stu-id="83569-131">Upgrade app installed for user</span></span>](../api/user-upgrade-teamsappinstallation.md) | <span data-ttu-id="83569-132">Нет</span><span class="sxs-lookup"><span data-stu-id="83569-132">None</span></span> | <span data-ttu-id="83569-133">Обновление до последней версии приложения, установленного в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="83569-133">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="83569-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="83569-134">Properties</span></span>

| <span data-ttu-id="83569-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="83569-135">Property</span></span>            | <span data-ttu-id="83569-136">Тип</span><span class="sxs-lookup"><span data-stu-id="83569-136">Type</span></span>     | <span data-ttu-id="83569-137">Описание</span><span class="sxs-lookup"><span data-stu-id="83569-137">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="83569-138">id</span><span class="sxs-lookup"><span data-stu-id="83569-138">id</span></span>                  | <span data-ttu-id="83569-139">string</span><span class="sxs-lookup"><span data-stu-id="83569-139">string</span></span>   | <span data-ttu-id="83569-140">Уникальный идентификатор (не идентификатор AP группы).</span><span class="sxs-lookup"><span data-stu-id="83569-140">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="83569-141">Связи</span><span class="sxs-lookup"><span data-stu-id="83569-141">Relationships</span></span>

| <span data-ttu-id="83569-142">Связь</span><span class="sxs-lookup"><span data-stu-id="83569-142">Relationship</span></span>   | <span data-ttu-id="83569-143">Тип</span><span class="sxs-lookup"><span data-stu-id="83569-143">Type</span></span>    | <span data-ttu-id="83569-144">Описание</span><span class="sxs-lookup"><span data-stu-id="83569-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="83569-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="83569-145">teamsApp</span></span>|[<span data-ttu-id="83569-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="83569-146">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="83569-147">Установленное приложение.</span><span class="sxs-lookup"><span data-stu-id="83569-147">The app that is installed.</span></span> |
|<span data-ttu-id="83569-148">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="83569-148">teamsAppDefinition</span></span>|[<span data-ttu-id="83569-149">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="83569-149">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="83569-150">Сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="83569-150">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="83569-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="83569-151">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="83569-152">См. также</span><span class="sxs-lookup"><span data-stu-id="83569-152">See also</span></span>

- [<span data-ttu-id="83569-153">teamsApp</span><span class="sxs-lookup"><span data-stu-id="83569-153">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="83569-154">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="83569-154">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="83569-155">teamsTab</span><span class="sxs-lookup"><span data-stu-id="83569-155">teamsTab</span></span>](../resources/teamstab.md)

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
