---
title: Работа с пользователями в Microsoft Graph
description: Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5f1a08e008f1de343ca6cf4986006c43c7e115af
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642060"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="ab7ce-103">Работа с пользователями в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ab7ce-103">Working with users in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab7ce-104">Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="ab7ce-105">Вы можете получить доступ к пользователям через Microsoft Graph двумя указанными ниже способами.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-105">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="ab7ce-106">По идентификатору пользователя (`/users/{id}`).</span><span class="sxs-lookup"><span data-stu-id="ab7ce-106">By their ID, `/users/{id}`</span></span> 
- <span data-ttu-id="ab7ce-107">С помощью псевдонима `/me` (который совпадает с `/users/{signed-in user's id}`) для пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="ab7ce-108">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab7ce-108">Authorization</span></span>
<span data-ttu-id="ab7ce-p101">Для операций доступа к пользователям необходимо одно из указанных ниже [разрешений](https://developer.microsoft.com/graph/docs/authorization/permission_scopes). Первые три разрешения могут быть предоставлены приложению пользователем. Остальные разрешения могут быть предоставлены приложению администратором.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="ab7ce-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="ab7ce-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="ab7ce-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="ab7ce-113">User.Read</span></span>
- <span data-ttu-id="ab7ce-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab7ce-114">User.ReadWrite</span></span>
- <span data-ttu-id="ab7ce-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab7ce-115">User.Read.All</span></span>
- <span data-ttu-id="ab7ce-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab7ce-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="ab7ce-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab7ce-117">Directory.Read.All</span></span>
- <span data-ttu-id="ab7ce-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab7ce-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="ab7ce-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ab7ce-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="ab7ce-120">Общие свойства</span><span class="sxs-lookup"><span data-stu-id="ab7ce-120">Common properties</span></span>

| <span data-ttu-id="ab7ce-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab7ce-121">Property</span></span> | <span data-ttu-id="ab7ce-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ab7ce-122">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="ab7ce-123">displayName</span><span class="sxs-lookup"><span data-stu-id="ab7ce-123">displayName</span></span> | <span data-ttu-id="ab7ce-124">Имя, отображаемое в адресной книге, для пользователя.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-124">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="ab7ce-125">givenName</span><span class="sxs-lookup"><span data-stu-id="ab7ce-125">givenName</span></span>| <span data-ttu-id="ab7ce-126">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-126">The first name of the user.</span></span> |
|<span data-ttu-id="ab7ce-127">surname</span><span class="sxs-lookup"><span data-stu-id="ab7ce-127">surname</span></span>| <span data-ttu-id="ab7ce-128">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-128">The last name of the user.</span></span> |
|<span data-ttu-id="ab7ce-129">mail</span><span class="sxs-lookup"><span data-stu-id="ab7ce-129">mail</span></span>| <span data-ttu-id="ab7ce-130">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-130">The user's email address.</span></span> |
|<span data-ttu-id="ab7ce-131">photo</span><span class="sxs-lookup"><span data-stu-id="ab7ce-131">photo</span></span>| <span data-ttu-id="ab7ce-132">Фотография профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-132">The user's profile photo.</span></span> |

<span data-ttu-id="ab7ce-133">Дополнительные сведения и список всех свойств см. в статье об объекте [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="ab7ce-133">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="ab7ce-134">Стандартные действия</span><span class="sxs-lookup"><span data-stu-id="ab7ce-134">Common operations</span></span>
><span data-ttu-id="ab7ce-135">**Примечание.** Для выполнения некоторых из этих операций необходимы дополнительные разрешения.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-135">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="ab7ce-136">Path</span><span class="sxs-lookup"><span data-stu-id="ab7ce-136">Path</span></span>    | <span data-ttu-id="ab7ce-137">Описание</span><span class="sxs-lookup"><span data-stu-id="ab7ce-137">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="ab7ce-138">Вывод списка пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-138">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="ab7ce-139">Получение определенного пользователя по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-139">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="ab7ce-140">Получение фотографии профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-140">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="ab7ce-141">Получение сведений о руководителе пользователя.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-141">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="ab7ce-142">Вывод списка электронных писем пользователя в его основном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-142">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="ab7ce-143">Вывод списка предстоящих событий пользователя из его календаря.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-143">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="ab7ce-144">Получение хранилища файлов OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-144">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="ab7ce-145">Вывод списка групп, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-145">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="ab7ce-146">Вывод списка команд Microsoft Teams, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="ab7ce-146">Lists the Microsoft Teams that the user is a member of.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/users.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
