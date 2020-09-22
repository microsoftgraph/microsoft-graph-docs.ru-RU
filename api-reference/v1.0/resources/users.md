---
title: Работа с пользователями в Microsoft Graph
description: Создавайте впечатляющие приложения, учитывающие пользователей, их связи с другими пользователями и группами, а также их почту, календарь и файлы.
localization_priority: Priority
author: krbain
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: c20d008cb2ee37a2ac4b49a3a857fdfabd0688ed
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015381"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="69d73-103">Работа с пользователями в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="69d73-103">Working with users in Microsoft Graph</span></span>

<span data-ttu-id="69d73-104">Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.</span><span class="sxs-lookup"><span data-stu-id="69d73-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="69d73-105">Вы можете получить доступ к [пользователям](user.md) через Microsoft Graph двумя указанными ниже способами.</span><span class="sxs-lookup"><span data-stu-id="69d73-105">You can access [users](user.md) through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="69d73-106">По идентификатору пользователя (`/users/{id | userPrincipalName}`).</span><span class="sxs-lookup"><span data-stu-id="69d73-106">By their ID, `/users/{id | userPrincipalName}`</span></span>
- <span data-ttu-id="69d73-107">С помощью псевдонима `/me` (который совпадает с `/users/{signed-in user's id}`) для пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="69d73-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="69d73-108">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69d73-108">Authorization</span></span>

<span data-ttu-id="69d73-p101">Для операций доступа к пользователям необходимо одно из указанных ниже [разрешений](https://developer.microsoft.com/graph/docs/authorization/permission_scopes). Первые три разрешения могут быть предоставлены приложению пользователем. Остальные разрешения могут быть предоставлены приложению администратором.</span><span class="sxs-lookup"><span data-stu-id="69d73-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="69d73-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="69d73-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="69d73-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="69d73-113">User.Read</span></span>
- <span data-ttu-id="69d73-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69d73-114">User.ReadWrite</span></span>
- <span data-ttu-id="69d73-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="69d73-115">User.Read.All</span></span>
- <span data-ttu-id="69d73-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69d73-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="69d73-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="69d73-117">Directory.Read.All</span></span>
- <span data-ttu-id="69d73-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69d73-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="69d73-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="69d73-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="69d73-120">Общие свойства</span><span class="sxs-lookup"><span data-stu-id="69d73-120">Common properties</span></span>

<span data-ttu-id="69d73-121">Ниже показан набор свойств, используемый по умолчанию и возвращаемый при получении пользователя или выводе списка пользователей.</span><span class="sxs-lookup"><span data-stu-id="69d73-121">The following represent the default set of properties that are returned when getting a user or listing users.</span></span> <span data-ttu-id="69d73-122">Это подмножество всех доступных свойств.</span><span class="sxs-lookup"><span data-stu-id="69d73-122">These are a subset of all available properties.</span></span> <span data-ttu-id="69d73-123">Чтобы получить дополнительные свойства пользователя, используйте параметр запроса `$select`.</span><span class="sxs-lookup"><span data-stu-id="69d73-123">To get more user properties, use the `$select` query parameter.</span></span>

|<span data-ttu-id="69d73-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="69d73-124">Property</span></span> |<span data-ttu-id="69d73-125">Описание</span><span class="sxs-lookup"><span data-stu-id="69d73-125">Description</span></span> |
|:----------|:-------------|
|<span data-ttu-id="69d73-126">id</span><span class="sxs-lookup"><span data-stu-id="69d73-126">id</span></span> | <span data-ttu-id="69d73-127">Уникальный идентификатор для пользователя.</span><span class="sxs-lookup"><span data-stu-id="69d73-127">The unique identifier for the user.</span></span>|
|<span data-ttu-id="69d73-128">businessPhones</span><span class="sxs-lookup"><span data-stu-id="69d73-128">businessPhones</span></span> | <span data-ttu-id="69d73-129">Номера телефонов пользователя.</span><span class="sxs-lookup"><span data-stu-id="69d73-129">The user's phone numbers.</span></span>|
|<span data-ttu-id="69d73-130">displayName</span><span class="sxs-lookup"><span data-stu-id="69d73-130">displayName</span></span> | <span data-ttu-id="69d73-131">Имя, отображаемое в адресной книге, для пользователя.</span><span class="sxs-lookup"><span data-stu-id="69d73-131">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="69d73-132">givenName</span><span class="sxs-lookup"><span data-stu-id="69d73-132">givenName</span></span>| <span data-ttu-id="69d73-133">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="69d73-133">The first name of the user.</span></span> |
|<span data-ttu-id="69d73-134">jobTitle</span><span class="sxs-lookup"><span data-stu-id="69d73-134">jobTitle</span></span> | <span data-ttu-id="69d73-135">Должность пользователя.</span><span class="sxs-lookup"><span data-stu-id="69d73-135">The user's job title.</span></span>|
|<span data-ttu-id="69d73-136">mail</span><span class="sxs-lookup"><span data-stu-id="69d73-136">mail</span></span>| <span data-ttu-id="69d73-137">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="69d73-137">The user's email address.</span></span> |
|<span data-ttu-id="69d73-138">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="69d73-138">mobilePhone</span></span> | <span data-ttu-id="69d73-139">Номер мобильного телефона пользователя.</span><span class="sxs-lookup"><span data-stu-id="69d73-139">The user's cellphone number.</span></span>|
|<span data-ttu-id="69d73-140">officeLocation</span><span class="sxs-lookup"><span data-stu-id="69d73-140">officeLocation</span></span> | <span data-ttu-id="69d73-141">Физическое расположение офиса пользователя.</span><span class="sxs-lookup"><span data-stu-id="69d73-141">The user's physical office location.</span></span>|
|<span data-ttu-id="69d73-142">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="69d73-142">preferredLanguage</span></span> | <span data-ttu-id="69d73-143">Предпочитаемый язык пользователя.</span><span class="sxs-lookup"><span data-stu-id="69d73-143">The user's language of preference.</span></span>|
|<span data-ttu-id="69d73-144">surname</span><span class="sxs-lookup"><span data-stu-id="69d73-144">surname</span></span>| <span data-ttu-id="69d73-145">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="69d73-145">The last name of the user.</span></span> |
|<span data-ttu-id="69d73-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="69d73-146">userPrincipalName</span></span>| <span data-ttu-id="69d73-147">Имя участника-пользователя для пользователя.</span><span class="sxs-lookup"><span data-stu-id="69d73-147">The user's principal name.</span></span> |

<span data-ttu-id="69d73-148">Дополнительные сведения и список всех свойств см. в статье об объекте [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="69d73-148">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="69d73-149">Стандартные действия</span><span class="sxs-lookup"><span data-stu-id="69d73-149">Common operations</span></span>

> <span data-ttu-id="69d73-150">**Примечание.** Для выполнения некоторых из этих операций необходимы дополнительные разрешения.</span><span class="sxs-lookup"><span data-stu-id="69d73-150">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="69d73-151">Path</span><span class="sxs-lookup"><span data-stu-id="69d73-151">Path</span></span>    | <span data-ttu-id="69d73-152">Описание</span><span class="sxs-lookup"><span data-stu-id="69d73-152">Description</span></span> |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="69d73-153">Вывод списка пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="69d73-153">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="69d73-154">Получение определенного пользователя по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="69d73-154">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="69d73-155">Получение фотографии профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="69d73-155">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="69d73-156">Получение сведений о руководителе пользователя.</span><span class="sxs-lookup"><span data-stu-id="69d73-156">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="69d73-157">Вывод списка электронных писем пользователя в его основном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="69d73-157">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="69d73-158">Вывод списка предстоящих событий пользователя из его календаря.</span><span class="sxs-lookup"><span data-stu-id="69d73-158">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="69d73-159">Получение хранилища файлов OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="69d73-159">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="69d73-160">Вывод списка групп, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="69d73-160">Lists the groups that the user is a member of.</span></span> |

## <a name="whats-new"></a><span data-ttu-id="69d73-161">Что нового</span><span class="sxs-lookup"><span data-stu-id="69d73-161">What's new</span></span>
<span data-ttu-id="69d73-162">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="69d73-162">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>
