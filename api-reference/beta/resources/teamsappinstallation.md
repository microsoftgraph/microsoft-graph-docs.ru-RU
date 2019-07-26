---
title: Тип ресурса Теамсаппинсталлатион
description: 'TeamsApp, установленный в команде, в чате или в личной области пользователя. '
author: clearab
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 55e1246616b7a3d76c6170a02286a2cde2a15d3a
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908511"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="ee9a3-103">Тип ресурса Теамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="ee9a3-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee9a3-104">[TeamsApp](teamsapp.md) , установленный в [команде](team.md), в [чате](chat.md)или в личной области [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="ee9a3-104">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="ee9a3-105">Все боты, которые входят в состав приложения, станут частью любой группы, чата или пользователя, к которому добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="ee9a3-105">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="ee9a3-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ee9a3-106">Methods</span></span>

| <span data-ttu-id="ee9a3-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ee9a3-107">Method</span></span>       | <span data-ttu-id="ee9a3-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ee9a3-108">Return Type</span></span>  |<span data-ttu-id="ee9a3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ee9a3-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ee9a3-110">Список приложений, установленных в Team</span><span class="sxs-lookup"><span data-stu-id="ee9a3-110">List apps installed in team</span></span>](../api/teamsappinstallation-list.md) | <span data-ttu-id="ee9a3-111">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="ee9a3-111">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="ee9a3-112">Список приложений, установленных в команде.</span><span class="sxs-lookup"><span data-stu-id="ee9a3-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="ee9a3-113">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="ee9a3-113">Add app to team</span></span>](../api/teamsappinstallation-add.md) |<span data-ttu-id="ee9a3-114">Нет</span><span class="sxs-lookup"><span data-stu-id="ee9a3-114">None</span></span> | <span data-ttu-id="ee9a3-115">Добавляет (устанавливает) приложение в команду.</span><span class="sxs-lookup"><span data-stu-id="ee9a3-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="ee9a3-116">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="ee9a3-116">Remove app from team</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="ee9a3-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ee9a3-117">None</span></span> | <span data-ttu-id="ee9a3-118">Удаляет приложение из команды.</span><span class="sxs-lookup"><span data-stu-id="ee9a3-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="ee9a3-119">Обновление приложения, установленного в команде</span><span class="sxs-lookup"><span data-stu-id="ee9a3-119">Upgrade app installed in team</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="ee9a3-120">Нет</span><span class="sxs-lookup"><span data-stu-id="ee9a3-120">None</span></span> | <span data-ttu-id="ee9a3-121">Обновление до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="ee9a3-121">Upgrades to the latest version of the app.</span></span>|
|[<span data-ttu-id="ee9a3-122">Список приложений, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="ee9a3-122">List apps installed for user</span></span>](../api/user-list-teamsappinstallation.md) | <span data-ttu-id="ee9a3-123">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="ee9a3-123">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="ee9a3-124">Список приложений, установленных в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="ee9a3-124">Lists apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="ee9a3-125">Добавление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="ee9a3-125">Add app for user</span></span>](../api/user-add-teamsappinstallation.md) | | <span data-ttu-id="ee9a3-126">Добавляет (устанавливает) приложение в личную область пользователя.</span><span class="sxs-lookup"><span data-stu-id="ee9a3-126">Adds (installs) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="ee9a3-127">Удаление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="ee9a3-127">Remove app for user</span></span>](../api/user-delete-teamsappinstallation.md) | <span data-ttu-id="ee9a3-128">Нет</span><span class="sxs-lookup"><span data-stu-id="ee9a3-128">None</span></span> | <span data-ttu-id="ee9a3-129">Удаляет приложение из персональной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="ee9a3-129">Removes (uninstalls) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="ee9a3-130">Обновление приложения, установленного для пользователя</span><span class="sxs-lookup"><span data-stu-id="ee9a3-130">Upgrade app installed for user</span></span>](../api/user-upgrade-teamsappinstallation.md) | <span data-ttu-id="ee9a3-131">Нет</span><span class="sxs-lookup"><span data-stu-id="ee9a3-131">None</span></span> | <span data-ttu-id="ee9a3-132">Обновление до последней версии приложения, установленного в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="ee9a3-132">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="ee9a3-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee9a3-133">Properties</span></span>

| <span data-ttu-id="ee9a3-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee9a3-134">Property</span></span>            | <span data-ttu-id="ee9a3-135">Тип</span><span class="sxs-lookup"><span data-stu-id="ee9a3-135">Type</span></span>     | <span data-ttu-id="ee9a3-136">Описание</span><span class="sxs-lookup"><span data-stu-id="ee9a3-136">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="ee9a3-137">id</span><span class="sxs-lookup"><span data-stu-id="ee9a3-137">id</span></span>                  | <span data-ttu-id="ee9a3-138">string</span><span class="sxs-lookup"><span data-stu-id="ee9a3-138">string</span></span>   | <span data-ttu-id="ee9a3-139">Уникальный идентификатор (не идентификатор AP группы).</span><span class="sxs-lookup"><span data-stu-id="ee9a3-139">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="ee9a3-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="ee9a3-140">Relationships</span></span>

| <span data-ttu-id="ee9a3-141">Отношение</span><span class="sxs-lookup"><span data-stu-id="ee9a3-141">Relationship</span></span>   | <span data-ttu-id="ee9a3-142">Тип</span><span class="sxs-lookup"><span data-stu-id="ee9a3-142">Type</span></span>    | <span data-ttu-id="ee9a3-143">Описание</span><span class="sxs-lookup"><span data-stu-id="ee9a3-143">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ee9a3-144">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ee9a3-144">teamsApp</span></span>|[<span data-ttu-id="ee9a3-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ee9a3-145">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="ee9a3-146">Установленное приложение.</span><span class="sxs-lookup"><span data-stu-id="ee9a3-146">The app that is installed.</span></span> |
|<span data-ttu-id="ee9a3-147">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="ee9a3-147">teamsAppDefinition</span></span>|[<span data-ttu-id="ee9a3-148">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="ee9a3-148">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="ee9a3-149">Сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="ee9a3-149">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ee9a3-150">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ee9a3-150">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="ee9a3-151">См. также</span><span class="sxs-lookup"><span data-stu-id="ee9a3-151">See also</span></span>

- [<span data-ttu-id="ee9a3-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ee9a3-152">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="ee9a3-153">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="ee9a3-153">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="ee9a3-154">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ee9a3-154">teamsTab</span></span>](../resources/teamstab.md)

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
