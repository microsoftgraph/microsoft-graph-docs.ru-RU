---
title: Работа с пользователями в Microsoft Graph
description: Создавайте впечатляющие приложения, учитывающие пользователей, их связи с другими пользователями и группами, а также их почту, календарь и файлы.
localization_priority: Priority
author: jpettere
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: c18731042d9d86479c5658f0a0f38a38d23bdb0d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719824"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="d9d54-103">Работа с пользователями в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d9d54-103">Working with users in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9d54-104">Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.</span><span class="sxs-lookup"><span data-stu-id="d9d54-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="d9d54-105">Вы можете получить доступ к пользователям через Microsoft Graph двумя указанными ниже способами.</span><span class="sxs-lookup"><span data-stu-id="d9d54-105">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="d9d54-106">По идентификатору пользователя (`/users/{id}`).</span><span class="sxs-lookup"><span data-stu-id="d9d54-106">By their ID, `/users/{id}`</span></span>
- <span data-ttu-id="d9d54-107">С помощью псевдонима `/me` (который совпадает с `/users/{signed-in user's id}`) для пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="d9d54-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="d9d54-108">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9d54-108">Authorization</span></span>

<span data-ttu-id="d9d54-p101">Для операций доступа к пользователям необходимо одно из указанных ниже [разрешений](/graph/permissions-reference). Первые три разрешения могут быть предоставлены приложению пользователем. Остальные разрешения могут быть предоставлены приложению администратором.</span><span class="sxs-lookup"><span data-stu-id="d9d54-p101">One of the following [permissions](/graph/permissions-reference) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="d9d54-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="d9d54-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="d9d54-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="d9d54-113">User.Read</span></span>
- <span data-ttu-id="d9d54-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9d54-114">User.ReadWrite</span></span>
- <span data-ttu-id="d9d54-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9d54-115">User.Read.All</span></span>
- <span data-ttu-id="d9d54-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9d54-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="d9d54-117">User.ManageIdentities.All</span><span class="sxs-lookup"><span data-stu-id="d9d54-117">User.ManageIdentities.All</span></span>
- <span data-ttu-id="d9d54-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9d54-118">Directory.Read.All</span></span>
- <span data-ttu-id="d9d54-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9d54-119">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="d9d54-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d9d54-120">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="d9d54-121">Общие свойства</span><span class="sxs-lookup"><span data-stu-id="d9d54-121">Common properties</span></span>

| <span data-ttu-id="d9d54-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9d54-122">Property</span></span> | <span data-ttu-id="d9d54-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d9d54-123">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="d9d54-124">displayName</span><span class="sxs-lookup"><span data-stu-id="d9d54-124">displayName</span></span> | <span data-ttu-id="d9d54-125">Имя, отображаемое в адресной книге, для пользователя.</span><span class="sxs-lookup"><span data-stu-id="d9d54-125">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="d9d54-126">givenName</span><span class="sxs-lookup"><span data-stu-id="d9d54-126">givenName</span></span>| <span data-ttu-id="d9d54-127">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="d9d54-127">The first name of the user.</span></span> |
|<span data-ttu-id="d9d54-128">surname</span><span class="sxs-lookup"><span data-stu-id="d9d54-128">surname</span></span>| <span data-ttu-id="d9d54-129">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="d9d54-129">The last name of the user.</span></span> |
|<span data-ttu-id="d9d54-130">mail</span><span class="sxs-lookup"><span data-stu-id="d9d54-130">mail</span></span>| <span data-ttu-id="d9d54-131">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="d9d54-131">The user's email address.</span></span> |
|<span data-ttu-id="d9d54-132">photo</span><span class="sxs-lookup"><span data-stu-id="d9d54-132">photo</span></span>| <span data-ttu-id="d9d54-133">Фотография профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="d9d54-133">The user's profile photo.</span></span> |

<span data-ttu-id="d9d54-134">Дополнительные сведения и список всех свойств см. в статье об объекте [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="d9d54-134">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="d9d54-135">Стандартные действия</span><span class="sxs-lookup"><span data-stu-id="d9d54-135">Common operations</span></span>

><span data-ttu-id="d9d54-136">**Примечание.** Для выполнения некоторых из этих операций необходимы дополнительные разрешения.</span><span class="sxs-lookup"><span data-stu-id="d9d54-136">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="d9d54-137">Path</span><span class="sxs-lookup"><span data-stu-id="d9d54-137">Path</span></span>    | <span data-ttu-id="d9d54-138">Описание</span><span class="sxs-lookup"><span data-stu-id="d9d54-138">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="d9d54-139">Вывод списка пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="d9d54-139">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="d9d54-140">Получение определенного пользователя по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="d9d54-140">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="d9d54-141">Получение фотографии профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="d9d54-141">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="d9d54-142">Получение сведений о руководителе пользователя.</span><span class="sxs-lookup"><span data-stu-id="d9d54-142">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="d9d54-143">Вывод списка электронных писем пользователя в его основном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d9d54-143">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="d9d54-144">Вывод списка предстоящих событий пользователя из его календаря.</span><span class="sxs-lookup"><span data-stu-id="d9d54-144">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="d9d54-145">Получение хранилища файлов OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="d9d54-145">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="d9d54-146">Вывод списка групп, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="d9d54-146">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="d9d54-147">Вывод списка команд Microsoft Teams, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="d9d54-147">Lists the Microsoft Teams that the user is a member of.</span></span> |

## <a name="whats-new"></a><span data-ttu-id="d9d54-148">Что нового</span><span class="sxs-lookup"><span data-stu-id="d9d54-148">What's new</span></span>
<span data-ttu-id="d9d54-149">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="d9d54-149">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>