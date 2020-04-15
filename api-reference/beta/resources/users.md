---
title: Работа с пользователями в Microsoft Graph
description: Создавайте впечатляющие приложения, основанные на пользователях, их отношениях с другими пользователями и группами, а также их почтой, календарем и файлами.
localization_priority: Priority
author: krbain
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: d69870512f8a8e86ddda77fb99a41019879edaa1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422462"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="b9e24-103">Работа с пользователями в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b9e24-103">Working with users in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9e24-104">Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.</span><span class="sxs-lookup"><span data-stu-id="b9e24-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="b9e24-105">Вы можете получить доступ к пользователям через Microsoft Graph двумя указанными ниже способами.</span><span class="sxs-lookup"><span data-stu-id="b9e24-105">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="b9e24-106">По идентификатору пользователя (`/users/{id}`).</span><span class="sxs-lookup"><span data-stu-id="b9e24-106">By their ID, `/users/{id}`</span></span>
- <span data-ttu-id="b9e24-107">С помощью псевдонима `/me` (который совпадает с `/users/{signed-in user's id}`) для пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="b9e24-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="b9e24-108">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9e24-108">Authorization</span></span>

<span data-ttu-id="b9e24-p101">Для операций доступа к пользователям необходимо одно из указанных ниже [разрешений](https://developer.microsoft.com/graph/docs/authorization/permission_scopes). Первые три разрешения могут быть предоставлены приложению пользователем. Остальные разрешения могут быть предоставлены приложению администратором.</span><span class="sxs-lookup"><span data-stu-id="b9e24-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="b9e24-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="b9e24-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="b9e24-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="b9e24-113">User.Read</span></span>
- <span data-ttu-id="b9e24-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9e24-114">User.ReadWrite</span></span>
- <span data-ttu-id="b9e24-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e24-115">User.Read.All</span></span>
- <span data-ttu-id="b9e24-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9e24-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="b9e24-117">User.ManageIdentities.All</span><span class="sxs-lookup"><span data-stu-id="b9e24-117">User.ManageIdentities.All</span></span>
- <span data-ttu-id="b9e24-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e24-118">Directory.Read.All</span></span>
- <span data-ttu-id="b9e24-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9e24-119">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="b9e24-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b9e24-120">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="b9e24-121">Общие свойства</span><span class="sxs-lookup"><span data-stu-id="b9e24-121">Common properties</span></span>

| <span data-ttu-id="b9e24-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9e24-122">Property</span></span> | <span data-ttu-id="b9e24-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b9e24-123">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="b9e24-124">displayName</span><span class="sxs-lookup"><span data-stu-id="b9e24-124">displayName</span></span> | <span data-ttu-id="b9e24-125">Имя, отображаемое в адресной книге, для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9e24-125">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="b9e24-126">givenName</span><span class="sxs-lookup"><span data-stu-id="b9e24-126">givenName</span></span>| <span data-ttu-id="b9e24-127">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9e24-127">The first name of the user.</span></span> |
|<span data-ttu-id="b9e24-128">surname</span><span class="sxs-lookup"><span data-stu-id="b9e24-128">surname</span></span>| <span data-ttu-id="b9e24-129">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9e24-129">The last name of the user.</span></span> |
|<span data-ttu-id="b9e24-130">mail</span><span class="sxs-lookup"><span data-stu-id="b9e24-130">mail</span></span>| <span data-ttu-id="b9e24-131">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9e24-131">The user's email address.</span></span> |
|<span data-ttu-id="b9e24-132">photo</span><span class="sxs-lookup"><span data-stu-id="b9e24-132">photo</span></span>| <span data-ttu-id="b9e24-133">Фотография профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9e24-133">The user's profile photo.</span></span> |

<span data-ttu-id="b9e24-134">Дополнительные сведения и список всех свойств см. в статье об объекте [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="b9e24-134">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="b9e24-135">Стандартные действия</span><span class="sxs-lookup"><span data-stu-id="b9e24-135">Common operations</span></span>

><span data-ttu-id="b9e24-136">**Примечание.** Для выполнения некоторых из этих операций необходимы дополнительные разрешения.</span><span class="sxs-lookup"><span data-stu-id="b9e24-136">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="b9e24-137">Path</span><span class="sxs-lookup"><span data-stu-id="b9e24-137">Path</span></span>    | <span data-ttu-id="b9e24-138">Описание</span><span class="sxs-lookup"><span data-stu-id="b9e24-138">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="b9e24-139">Вывод списка пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="b9e24-139">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="b9e24-140">Получение определенного пользователя по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="b9e24-140">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="b9e24-141">Получение фотографии профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9e24-141">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="b9e24-142">Получение сведений о руководителе пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9e24-142">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="b9e24-143">Вывод списка электронных писем пользователя в его основном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="b9e24-143">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="b9e24-144">Вывод списка предстоящих событий пользователя из его календаря.</span><span class="sxs-lookup"><span data-stu-id="b9e24-144">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="b9e24-145">Получение хранилища файлов OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9e24-145">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="b9e24-146">Вывод списка групп, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="b9e24-146">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="b9e24-147">Вывод списка команд Microsoft Teams, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="b9e24-147">Lists the Microsoft Teams that the user is a member of.</span></span> |
