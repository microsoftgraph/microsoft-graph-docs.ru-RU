---
title: Работа с пользователями в Microsoft Graph
description: Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.
localization_priority: Priority
ms.openlocfilehash: d9b699c008186f165a8be43ab4254213697710dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860832"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="96a07-103">Работа с пользователями в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="96a07-103">Working with users in Microsoft Graph</span></span>

> <span data-ttu-id="96a07-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="96a07-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96a07-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96a07-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96a07-106">Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.</span><span class="sxs-lookup"><span data-stu-id="96a07-106">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="96a07-107">Вы можете получить доступ к пользователям через Microsoft Graph двумя указанными ниже способами.</span><span class="sxs-lookup"><span data-stu-id="96a07-107">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="96a07-108">По идентификатору пользователя (`/users/{id}`).</span><span class="sxs-lookup"><span data-stu-id="96a07-108">By their ID, `/users/{id}`</span></span> 
- <span data-ttu-id="96a07-109">С помощью псевдонима `/me` (который совпадает с `/users/{signed-in user's id}`) для пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="96a07-109">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="96a07-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="96a07-110">Authorization</span></span>
<span data-ttu-id="96a07-p102">Для операций доступа к пользователям необходимо одно из указанных ниже [разрешений](https://developer.microsoft.com/graph/docs/authorization/permission_scopes). Первые три разрешения могут быть предоставлены приложению пользователем. Остальные разрешения могут быть предоставлены приложению администратором.</span><span class="sxs-lookup"><span data-stu-id="96a07-p102">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="96a07-114">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="96a07-114">User.ReadBasic.All</span></span>
- <span data-ttu-id="96a07-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="96a07-115">User.Read</span></span>
- <span data-ttu-id="96a07-116">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96a07-116">User.ReadWrite</span></span>
- <span data-ttu-id="96a07-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="96a07-117">User.Read.All</span></span>
- <span data-ttu-id="96a07-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96a07-118">User.ReadWrite.All</span></span>
- <span data-ttu-id="96a07-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="96a07-119">Directory.Read.All</span></span>
- <span data-ttu-id="96a07-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96a07-120">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="96a07-121">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="96a07-121">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="96a07-122">Общие свойства</span><span class="sxs-lookup"><span data-stu-id="96a07-122">Common properties</span></span>

| <span data-ttu-id="96a07-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="96a07-123">Property</span></span> | <span data-ttu-id="96a07-124">Описание</span><span class="sxs-lookup"><span data-stu-id="96a07-124">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="96a07-125">displayName</span><span class="sxs-lookup"><span data-stu-id="96a07-125">displayName</span></span> | <span data-ttu-id="96a07-126">Имя, отображаемое в адресной книге, для пользователя.</span><span class="sxs-lookup"><span data-stu-id="96a07-126">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="96a07-127">givenName</span><span class="sxs-lookup"><span data-stu-id="96a07-127">givenName</span></span>| <span data-ttu-id="96a07-128">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="96a07-128">The first name of the user.</span></span> |
|<span data-ttu-id="96a07-129">surname</span><span class="sxs-lookup"><span data-stu-id="96a07-129">surname</span></span>| <span data-ttu-id="96a07-130">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="96a07-130">The last name of the user.</span></span> |
|<span data-ttu-id="96a07-131">mail</span><span class="sxs-lookup"><span data-stu-id="96a07-131">mail</span></span>| <span data-ttu-id="96a07-132">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="96a07-132">The user's email address.</span></span> |
|<span data-ttu-id="96a07-133">photo;</span><span class="sxs-lookup"><span data-stu-id="96a07-133">photo</span></span>| <span data-ttu-id="96a07-134">Фотографий профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="96a07-134">The user's profile photo.</span></span> |

<span data-ttu-id="96a07-135">Дополнительные сведения и список всех свойств см. в статье об объекте [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="96a07-135">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="96a07-136">Стандартные действия</span><span class="sxs-lookup"><span data-stu-id="96a07-136">Common operations</span></span>
><span data-ttu-id="96a07-137">**Примечание.** Для выполнения некоторых из этих операций необходимы дополнительные разрешения.</span><span class="sxs-lookup"><span data-stu-id="96a07-137">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="96a07-138">Путь</span><span class="sxs-lookup"><span data-stu-id="96a07-138">Path</span></span>    | <span data-ttu-id="96a07-139">Описание</span><span class="sxs-lookup"><span data-stu-id="96a07-139">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="96a07-140">Вывод списка пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="96a07-140">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="96a07-141">Получение определенного пользователя по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="96a07-141">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="96a07-142">Получение фотографии профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="96a07-142">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="96a07-143">Получение сведений о руководителе пользователя.</span><span class="sxs-lookup"><span data-stu-id="96a07-143">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="96a07-144">Вывод списка электронных писем пользователя в его основном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="96a07-144">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="96a07-145">Вывод списка предстоящих событий пользователя из его календаря.</span><span class="sxs-lookup"><span data-stu-id="96a07-145">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="96a07-146">Получение хранилища файлов OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="96a07-146">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="96a07-147">Вывод списка групп, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="96a07-147">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="96a07-148">Список групп Майкрософт, который входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="96a07-148">Lists the Microsoft Teams that the user is a member of.</span></span> |
