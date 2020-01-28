---
title: Тип ресурса Теамсаппинсталлатион
description: 'TeamsApp, установленный в команде, в чате или в личной области пользователя. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9aa86509fdbcdaa49d07987eacbfe763b848408a
ms.sourcegitcommit: 0f39f39a1c0300ef013ebd12e4df2b5ba4dabbf8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2020
ms.locfileid: "41559049"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="d2814-103">Тип ресурса Теамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="d2814-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2814-104">[TeamsApp](teamsapp.md) , установленный в [команде](team.md), в [чате](chat.md)или в личной области [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="d2814-104">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="d2814-105">Все боты, которые входят в состав приложения, станут частью любой группы, чата или пользователя, к которому добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="d2814-105">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="d2814-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d2814-106">Methods</span></span>

| <span data-ttu-id="d2814-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d2814-107">Method</span></span>       | <span data-ttu-id="d2814-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d2814-108">Return Type</span></span>  |<span data-ttu-id="d2814-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d2814-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2814-110">Список приложений, установленных в Team</span><span class="sxs-lookup"><span data-stu-id="d2814-110">List apps installed in team</span></span>](../api/teamsappinstallation-list.md) | <span data-ttu-id="d2814-111">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="d2814-111">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="d2814-112">Список приложений, установленных в команде.</span><span class="sxs-lookup"><span data-stu-id="d2814-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="d2814-113">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="d2814-113">Add app to team</span></span>](../api/teamsappinstallation-add.md) |<span data-ttu-id="d2814-114">Нет</span><span class="sxs-lookup"><span data-stu-id="d2814-114">None</span></span> | <span data-ttu-id="d2814-115">Добавляет (устанавливает) приложение в команду.</span><span class="sxs-lookup"><span data-stu-id="d2814-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="d2814-116">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="d2814-116">Remove app from team</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="d2814-117">Нет</span><span class="sxs-lookup"><span data-stu-id="d2814-117">None</span></span> | <span data-ttu-id="d2814-118">Удаляет приложение из команды.</span><span class="sxs-lookup"><span data-stu-id="d2814-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="d2814-119">Обновление приложения, установленного в команде</span><span class="sxs-lookup"><span data-stu-id="d2814-119">Upgrade app installed in team</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="d2814-120">Нет</span><span class="sxs-lookup"><span data-stu-id="d2814-120">None</span></span> | <span data-ttu-id="d2814-121">Обновление до последней версии приложения, установленного в команде.</span><span class="sxs-lookup"><span data-stu-id="d2814-121">Upgrades to the latest version of the app installed in team.</span></span>|
|[<span data-ttu-id="d2814-122">Перечисление приложений, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="d2814-122">List apps installed for user</span></span>](../api/user-list-teamsappinstallation.md) | <span data-ttu-id="d2814-123">[teamsAppInstallation](teamsappinstallation.md) collection</span><span class="sxs-lookup"><span data-stu-id="d2814-123">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="d2814-124">Список приложений, установленных в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2814-124">Lists apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="d2814-125">Добавление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="d2814-125">Add app for user</span></span>](../api/user-add-teamsappinstallation.md) | | <span data-ttu-id="d2814-126">Добавляет (устанавливает) приложение в личную область пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2814-126">Adds (installs) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="d2814-127">Удаление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="d2814-127">Remove app for user</span></span>](../api/user-delete-teamsappinstallation.md) | <span data-ttu-id="d2814-128">Нет</span><span class="sxs-lookup"><span data-stu-id="d2814-128">None</span></span> | <span data-ttu-id="d2814-129">Удаляет приложение из персональной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2814-129">Removes (uninstalls) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="d2814-130">Обновление приложения, установленного для пользователя</span><span class="sxs-lookup"><span data-stu-id="d2814-130">Upgrade app installed for user</span></span>](../api/user-upgrade-teamsappinstallation.md) | <span data-ttu-id="d2814-131">Нет</span><span class="sxs-lookup"><span data-stu-id="d2814-131">None</span></span> | <span data-ttu-id="d2814-132">Обновление до последней версии приложения, установленного в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2814-132">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2814-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2814-133">Properties</span></span>

| <span data-ttu-id="d2814-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2814-134">Property</span></span>            | <span data-ttu-id="d2814-135">Тип</span><span class="sxs-lookup"><span data-stu-id="d2814-135">Type</span></span>     | <span data-ttu-id="d2814-136">Описание</span><span class="sxs-lookup"><span data-stu-id="d2814-136">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="d2814-137">id</span><span class="sxs-lookup"><span data-stu-id="d2814-137">id</span></span>                  | <span data-ttu-id="d2814-138">string</span><span class="sxs-lookup"><span data-stu-id="d2814-138">string</span></span>   | <span data-ttu-id="d2814-139">Уникальный идентификатор (не идентификатор AP группы).</span><span class="sxs-lookup"><span data-stu-id="d2814-139">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="d2814-140">Связи</span><span class="sxs-lookup"><span data-stu-id="d2814-140">Relationships</span></span>

| <span data-ttu-id="d2814-141">Связь</span><span class="sxs-lookup"><span data-stu-id="d2814-141">Relationship</span></span>   | <span data-ttu-id="d2814-142">Тип</span><span class="sxs-lookup"><span data-stu-id="d2814-142">Type</span></span>    | <span data-ttu-id="d2814-143">Описание</span><span class="sxs-lookup"><span data-stu-id="d2814-143">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d2814-144">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d2814-144">teamsApp</span></span>|[<span data-ttu-id="d2814-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d2814-145">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="d2814-146">Установленное приложение.</span><span class="sxs-lookup"><span data-stu-id="d2814-146">The app that is installed.</span></span> |
|<span data-ttu-id="d2814-147">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d2814-147">teamsAppDefinition</span></span>|[<span data-ttu-id="d2814-148">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d2814-148">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="d2814-149">Сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="d2814-149">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d2814-150">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d2814-150">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="d2814-151">См. также</span><span class="sxs-lookup"><span data-stu-id="d2814-151">See also</span></span>

- [<span data-ttu-id="d2814-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d2814-152">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="d2814-153">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d2814-153">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="d2814-154">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d2814-154">teamsTab</span></span>](../resources/teamstab.md)

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
