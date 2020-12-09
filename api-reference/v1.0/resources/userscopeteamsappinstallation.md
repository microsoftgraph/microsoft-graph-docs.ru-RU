---
title: Тип ресурса Усерскопетеамсаппинсталлатион
description: Представляет teamsApp, установленный в личной области пользователя.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 30df2c14f8723dedd25fb7c4e5b2a00481338dc3
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606862"
---
# <a name="userscopeteamsappinstallation-resource-type"></a><span data-ttu-id="58a15-103">Тип ресурса Усерскопетеамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="58a15-103">userScopeTeamsAppInstallation resource type</span></span>

<span data-ttu-id="58a15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58a15-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="58a15-105">Представляет [teamsApp](teamsapp.md) , установленный в личной области [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="58a15-105">Represents a [teamsApp](teamsapp.md) installed in the personal scope of a [user](user.md).</span></span> <span data-ttu-id="58a15-106">Все боты, которые входят в состав приложения, станут частью личной области пользователя, в которую добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="58a15-106">Any bots that are part of the app will become part of a user's personal scope that the app is added to.</span></span>
<span data-ttu-id="58a15-107">Этот тип наследуется от [теамсаппинсталлатион](teamsappinstallation.md).</span><span class="sxs-lookup"><span data-stu-id="58a15-107">This type inherits from [teamsAppInstallation](teamsappinstallation.md).</span></span>

> [!NOTE]
> <span data-ttu-id="58a15-108">`id`Ресурс **теамсаппинсталлатион** имеет не то же значение, что и `id` связанный ресурс **teamsApp** .</span><span class="sxs-lookup"><span data-stu-id="58a15-108">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="methods"></a><span data-ttu-id="58a15-109">Методы</span><span class="sxs-lookup"><span data-stu-id="58a15-109">Methods</span></span>

| <span data-ttu-id="58a15-110">Метод</span><span class="sxs-lookup"><span data-stu-id="58a15-110">Method</span></span>       | <span data-ttu-id="58a15-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="58a15-111">Return Type</span></span>  |<span data-ttu-id="58a15-112">Описание</span><span class="sxs-lookup"><span data-stu-id="58a15-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58a15-113">Перечисление приложений, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="58a15-113">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md)| <span data-ttu-id="58a15-114">Коллекция [усерскопетеамсаппинсталлатион](userscopeteamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="58a15-114">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="58a15-115">Список приложений, установленных в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="58a15-115">List apps installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="58a15-116">Получает установленное приложение для пользователя</span><span class="sxs-lookup"><span data-stu-id="58a15-116">Gets the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="58a15-117">усерскопетеамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="58a15-117">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="58a15-118">Список указанного приложения, установленного в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="58a15-118">List the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="58a15-119">Добавление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="58a15-119">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | <span data-ttu-id="58a15-120">Нет</span><span class="sxs-lookup"><span data-stu-id="58a15-120">None</span></span> | <span data-ttu-id="58a15-121">Добавление (установка) приложения в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="58a15-121">Add (install) an app in the personal scope of a user.</span></span> |
|[<span data-ttu-id="58a15-122">Удаление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="58a15-122">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="58a15-123">Нет</span><span class="sxs-lookup"><span data-stu-id="58a15-123">None</span></span> | <span data-ttu-id="58a15-124">Удалить (удалить) приложение в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="58a15-124">Remove (uninstall) an app in the personal scope of a user.</span></span> |
|[<span data-ttu-id="58a15-125">Обновление приложения, установленного для пользователя</span><span class="sxs-lookup"><span data-stu-id="58a15-125">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="58a15-126">Нет</span><span class="sxs-lookup"><span data-stu-id="58a15-126">None</span></span> | <span data-ttu-id="58a15-127">Выполните обновление до последней версии приложения, установленного в личной области пользователя.</span><span class="sxs-lookup"><span data-stu-id="58a15-127">Upgrade to the latest version of the app installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="58a15-128">Получение разговора между пользователем и приложением</span><span class="sxs-lookup"><span data-stu-id="58a15-128">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="58a15-129">chat</span><span class="sxs-lookup"><span data-stu-id="58a15-129">chat</span></span>](chat.md) | <span data-ttu-id="58a15-130">Перечисление сеансов одного пользователя и приложения.</span><span class="sxs-lookup"><span data-stu-id="58a15-130">List one-on-one chats between a user and the app.</span></span> |

## <a name="properties"></a><span data-ttu-id="58a15-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="58a15-131">Properties</span></span>

| <span data-ttu-id="58a15-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="58a15-132">Property</span></span>            | <span data-ttu-id="58a15-133">Тип</span><span class="sxs-lookup"><span data-stu-id="58a15-133">Type</span></span>     | <span data-ttu-id="58a15-134">Описание</span><span class="sxs-lookup"><span data-stu-id="58a15-134">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="58a15-135">id</span><span class="sxs-lookup"><span data-stu-id="58a15-135">id</span></span>                  | <span data-ttu-id="58a15-136">string</span><span class="sxs-lookup"><span data-stu-id="58a15-136">string</span></span>   | <span data-ttu-id="58a15-137">Уникальный идентификатор (не идентификатор приложения Teams).</span><span class="sxs-lookup"><span data-stu-id="58a15-137">A unique ID (not the Teams app ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="58a15-138">Связи</span><span class="sxs-lookup"><span data-stu-id="58a15-138">Relationships</span></span>

| <span data-ttu-id="58a15-139">Связь</span><span class="sxs-lookup"><span data-stu-id="58a15-139">Relationship</span></span>   | <span data-ttu-id="58a15-140">Тип</span><span class="sxs-lookup"><span data-stu-id="58a15-140">Type</span></span>    | <span data-ttu-id="58a15-141">Описание</span><span class="sxs-lookup"><span data-stu-id="58a15-141">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="58a15-142">teamsApp</span><span class="sxs-lookup"><span data-stu-id="58a15-142">teamsApp</span></span>|[<span data-ttu-id="58a15-143">teamsApp</span><span class="sxs-lookup"><span data-stu-id="58a15-143">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="58a15-144">Установленное приложение.</span><span class="sxs-lookup"><span data-stu-id="58a15-144">The app that is installed.</span></span> |
|<span data-ttu-id="58a15-145">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="58a15-145">teamsAppDefinition</span></span>|[<span data-ttu-id="58a15-146">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="58a15-146">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="58a15-147">Сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="58a15-147">The details of this version of the app.</span></span> |
|<span data-ttu-id="58a15-148">чат</span><span class="sxs-lookup"><span data-stu-id="58a15-148">chat</span></span> |[<span data-ttu-id="58a15-149">chat</span><span class="sxs-lookup"><span data-stu-id="58a15-149">chat</span></span>](chat.md) | <span data-ttu-id="58a15-150">Чат между пользователем и приложением Teams.</span><span class="sxs-lookup"><span data-stu-id="58a15-150">The chat between the user and Teams app.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="58a15-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="58a15-151">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="58a15-152">См. также</span><span class="sxs-lookup"><span data-stu-id="58a15-152">See also</span></span>

- [<span data-ttu-id="58a15-153">teamsApp</span><span class="sxs-lookup"><span data-stu-id="58a15-153">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="58a15-154">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="58a15-154">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="58a15-155">teamsTab</span><span class="sxs-lookup"><span data-stu-id="58a15-155">teamsTab</span></span>](../resources/teamstab.md)

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

