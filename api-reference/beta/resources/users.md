---
title: Работа с пользователями в Microsoft Graph
description: Создавайте впечатляющие приложения, учитывающие пользователей, их связи с другими пользователями и группами, а также их почту, календарь и файлы.
localization_priority: Priority
author: krbain
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 7e78476b85ed16550ca1af23c8e3fd611869a127
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402956"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="8b169-103">Работа с пользователями в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8b169-103">Working with users in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b169-104">Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.</span><span class="sxs-lookup"><span data-stu-id="8b169-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="8b169-105">Вы можете получить доступ к пользователям через Microsoft Graph двумя указанными ниже способами.</span><span class="sxs-lookup"><span data-stu-id="8b169-105">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="8b169-106">По идентификатору пользователя (`/users/{id}`).</span><span class="sxs-lookup"><span data-stu-id="8b169-106">By their ID, `/users/{id}`</span></span>
- <span data-ttu-id="8b169-107">С помощью псевдонима `/me` (который совпадает с `/users/{signed-in user's id}`) для пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="8b169-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="8b169-108">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b169-108">Authorization</span></span>

<span data-ttu-id="8b169-p101">Для операций доступа к пользователям необходимо одно из указанных ниже [разрешений](/graph/permissions-reference). Первые три разрешения могут быть предоставлены приложению пользователем. Остальные разрешения могут быть предоставлены приложению администратором.</span><span class="sxs-lookup"><span data-stu-id="8b169-p101">One of the following [permissions](/graph/permissions-reference) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="8b169-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="8b169-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="8b169-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="8b169-113">User.Read</span></span>
- <span data-ttu-id="8b169-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b169-114">User.ReadWrite</span></span>
- <span data-ttu-id="8b169-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b169-115">User.Read.All</span></span>
- <span data-ttu-id="8b169-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b169-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="8b169-117">User.ManageIdentities.All</span><span class="sxs-lookup"><span data-stu-id="8b169-117">User.ManageIdentities.All</span></span>
- <span data-ttu-id="8b169-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b169-118">Directory.Read.All</span></span>
- <span data-ttu-id="8b169-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b169-119">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="8b169-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8b169-120">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="8b169-121">Общие свойства</span><span class="sxs-lookup"><span data-stu-id="8b169-121">Common properties</span></span>

| <span data-ttu-id="8b169-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b169-122">Property</span></span> | <span data-ttu-id="8b169-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8b169-123">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="8b169-124">displayName</span><span class="sxs-lookup"><span data-stu-id="8b169-124">displayName</span></span> | <span data-ttu-id="8b169-125">Имя, отображаемое в адресной книге, для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b169-125">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="8b169-126">givenName</span><span class="sxs-lookup"><span data-stu-id="8b169-126">givenName</span></span>| <span data-ttu-id="8b169-127">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b169-127">The first name of the user.</span></span> |
|<span data-ttu-id="8b169-128">surname</span><span class="sxs-lookup"><span data-stu-id="8b169-128">surname</span></span>| <span data-ttu-id="8b169-129">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b169-129">The last name of the user.</span></span> |
|<span data-ttu-id="8b169-130">mail</span><span class="sxs-lookup"><span data-stu-id="8b169-130">mail</span></span>| <span data-ttu-id="8b169-131">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b169-131">The user's email address.</span></span> |
|<span data-ttu-id="8b169-132">photo</span><span class="sxs-lookup"><span data-stu-id="8b169-132">photo</span></span>| <span data-ttu-id="8b169-133">Фотография профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b169-133">The user's profile photo.</span></span> |

<span data-ttu-id="8b169-134">Дополнительные сведения и список всех свойств см. в статье об объекте [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="8b169-134">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="8b169-135">Стандартные действия</span><span class="sxs-lookup"><span data-stu-id="8b169-135">Common operations</span></span>

><span data-ttu-id="8b169-136">**Примечание.** Для выполнения некоторых из этих операций необходимы дополнительные разрешения.</span><span class="sxs-lookup"><span data-stu-id="8b169-136">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="8b169-137">Path</span><span class="sxs-lookup"><span data-stu-id="8b169-137">Path</span></span>    | <span data-ttu-id="8b169-138">Описание</span><span class="sxs-lookup"><span data-stu-id="8b169-138">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="8b169-139">Вывод списка пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="8b169-139">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="8b169-140">Получение определенного пользователя по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="8b169-140">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="8b169-141">Получение фотографии профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b169-141">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="8b169-142">Получение сведений о руководителе пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b169-142">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="8b169-143">Вывод списка электронных писем пользователя в его основном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="8b169-143">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="8b169-144">Вывод списка предстоящих событий пользователя из его календаря.</span><span class="sxs-lookup"><span data-stu-id="8b169-144">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="8b169-145">Получение хранилища файлов OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b169-145">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="8b169-146">Вывод списка групп, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="8b169-146">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="8b169-147">Вывод списка команд Microsoft Teams, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="8b169-147">Lists the Microsoft Teams that the user is a member of.</span></span> |

## <a name="whats-new"></a><span data-ttu-id="8b169-148">Что нового</span><span class="sxs-lookup"><span data-stu-id="8b169-148">What's new</span></span>
<span data-ttu-id="8b169-149">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="8b169-149">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>