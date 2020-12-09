---
title: Тип ресурса Усерскопетеамсаппинсталлатион
description: Представляет teamsApp, установленный в личной области пользователя.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 70ebdcb30c67d59e3a12c4a0514314015e163c17
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607023"
---
# <a name="userscopeteamsappinstallation-resource-type"></a><span data-ttu-id="ff1df-103">Тип ресурса Усерскопетеамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="ff1df-103">userScopeTeamsAppInstallation resource type</span></span>

<span data-ttu-id="ff1df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff1df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff1df-105">Представляет [teamsApp](teamsapp.md) , установленный в личной области [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="ff1df-105">Represents a [teamsApp](teamsapp.md) installed in the personal scope of a [user](user.md).</span></span> <span data-ttu-id="ff1df-106">Все боты, которые входят в состав приложения, станут частью личной области пользователя, в которую добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="ff1df-106">Any bots that are part of the app will become part of a user's personal scope that the app is added to.</span></span>
<span data-ttu-id="ff1df-107">Этот тип наследуется от [теамсаппинсталлатион](teamsappinstallation.md).</span><span class="sxs-lookup"><span data-stu-id="ff1df-107">This type inherits from [teamsAppInstallation](teamsappinstallation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ff1df-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ff1df-108">Methods</span></span>

| <span data-ttu-id="ff1df-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ff1df-109">Method</span></span>       | <span data-ttu-id="ff1df-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ff1df-110">Return Type</span></span>  |<span data-ttu-id="ff1df-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ff1df-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff1df-112">Перечисление приложений, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="ff1df-112">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md)| <span data-ttu-id="ff1df-113">Коллекция [усерскопетеамсаппинсталлатион](userscopeteamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="ff1df-113">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="ff1df-114">Список приложений, установленных в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="ff1df-114">List apps installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="ff1df-115">Получение приложения, установленного для пользователя</span><span class="sxs-lookup"><span data-stu-id="ff1df-115">Get the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="ff1df-116">усерскопетеамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="ff1df-116">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="ff1df-117">Список указанного приложения, установленного в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="ff1df-117">List the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="ff1df-118">Добавление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="ff1df-118">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | <span data-ttu-id="ff1df-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ff1df-119">None</span></span> | <span data-ttu-id="ff1df-120">Добавляет (устанавливает) приложение в личную область пользователя.</span><span class="sxs-lookup"><span data-stu-id="ff1df-120">Adds (installs) an app in the personal scope of a user.</span></span> |
|[<span data-ttu-id="ff1df-121">Удаление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="ff1df-121">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="ff1df-122">Нет</span><span class="sxs-lookup"><span data-stu-id="ff1df-122">None</span></span> | <span data-ttu-id="ff1df-123">Удаляет приложение из персональной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="ff1df-123">Removes (uninstalls) an app in the personal scope of a user.</span></span> |
|[<span data-ttu-id="ff1df-124">Обновление приложения, установленного для пользователя</span><span class="sxs-lookup"><span data-stu-id="ff1df-124">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="ff1df-125">Нет</span><span class="sxs-lookup"><span data-stu-id="ff1df-125">None</span></span> | <span data-ttu-id="ff1df-126">Обновление до последней версии приложения, установленного в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="ff1df-126">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="ff1df-127">Получение разговора между пользователем и приложением</span><span class="sxs-lookup"><span data-stu-id="ff1df-127">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="ff1df-128">chat</span><span class="sxs-lookup"><span data-stu-id="ff1df-128">chat</span></span>](chat.md) | <span data-ttu-id="ff1df-129">Перечисление одного сеанса разговора между пользователем и приложением.</span><span class="sxs-lookup"><span data-stu-id="ff1df-129">Lists one-on-one chat between the user and the app.</span></span> |

## <a name="properties"></a><span data-ttu-id="ff1df-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff1df-130">Properties</span></span>

| <span data-ttu-id="ff1df-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff1df-131">Property</span></span>            | <span data-ttu-id="ff1df-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ff1df-132">Type</span></span>     | <span data-ttu-id="ff1df-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ff1df-133">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="ff1df-134">id</span><span class="sxs-lookup"><span data-stu-id="ff1df-134">id</span></span>                  | <span data-ttu-id="ff1df-135">string</span><span class="sxs-lookup"><span data-stu-id="ff1df-135">string</span></span>   | <span data-ttu-id="ff1df-136">Уникальный идентификатор (не идентификатор приложения Teams).</span><span class="sxs-lookup"><span data-stu-id="ff1df-136">A unique ID (not the Teams app ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="ff1df-137">Связи</span><span class="sxs-lookup"><span data-stu-id="ff1df-137">Relationships</span></span>

| <span data-ttu-id="ff1df-138">Связь</span><span class="sxs-lookup"><span data-stu-id="ff1df-138">Relationship</span></span>   | <span data-ttu-id="ff1df-139">Тип</span><span class="sxs-lookup"><span data-stu-id="ff1df-139">Type</span></span>    | <span data-ttu-id="ff1df-140">Описание</span><span class="sxs-lookup"><span data-stu-id="ff1df-140">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ff1df-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ff1df-141">teamsApp</span></span>|[<span data-ttu-id="ff1df-142">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ff1df-142">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="ff1df-143">Установленное приложение.</span><span class="sxs-lookup"><span data-stu-id="ff1df-143">The app that is installed.</span></span> |
|<span data-ttu-id="ff1df-144">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="ff1df-144">teamsAppDefinition</span></span>|[<span data-ttu-id="ff1df-145">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="ff1df-145">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="ff1df-146">Сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="ff1df-146">The details of this version of the app.</span></span> |
|<span data-ttu-id="ff1df-147">чат</span><span class="sxs-lookup"><span data-stu-id="ff1df-147">chat</span></span> |[<span data-ttu-id="ff1df-148">chat</span><span class="sxs-lookup"><span data-stu-id="ff1df-148">chat</span></span>](chat.md) | <span data-ttu-id="ff1df-149">Чат между пользователем и приложением Teams.</span><span class="sxs-lookup"><span data-stu-id="ff1df-149">The chat between the user and Teams app.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="ff1df-150">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ff1df-150">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userScopeTeamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="ff1df-151">См. также</span><span class="sxs-lookup"><span data-stu-id="ff1df-151">See also</span></span>

- [<span data-ttu-id="ff1df-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ff1df-152">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="ff1df-153">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="ff1df-153">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="ff1df-154">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ff1df-154">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userScopeTeamsAppInstallation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
  "suppressions": []
}-->

