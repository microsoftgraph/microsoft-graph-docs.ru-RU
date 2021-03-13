---
title: Работа с пользователями в Microsoft Graph
description: Создавайте впечатляющие приложения, учитывающие пользователей, их связи с другими пользователями и группами, а также их почту, календарь и файлы.
localization_priority: Priority
author: jpettere
ms.prod: users
doc_type: conceptualPageType
ms.openlocfilehash: 217e3461c2f14490c0a1ffcf633b513464f1baf1
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759491"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="81f01-103">Работа с пользователями в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="81f01-103">Working with users in Microsoft Graph</span></span>

<span data-ttu-id="81f01-104">Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.</span><span class="sxs-lookup"><span data-stu-id="81f01-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="81f01-105">Вы можете получить доступ к [пользователям](user.md) через Microsoft Graph двумя указанными ниже способами.</span><span class="sxs-lookup"><span data-stu-id="81f01-105">You can access [users](user.md) through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="81f01-106">По идентификатору пользователя (`/users/{id | userPrincipalName}`).</span><span class="sxs-lookup"><span data-stu-id="81f01-106">By their ID, `/users/{id | userPrincipalName}`</span></span>
- <span data-ttu-id="81f01-107">С помощью псевдонима `/me` (который совпадает с `/users/{signed-in user's id}`) для пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="81f01-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="81f01-108">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81f01-108">Authorization</span></span>

<span data-ttu-id="81f01-p101">Для операций доступа к пользователям необходимо одно из указанных ниже [разрешений](/graph/permissions-reference). Первые три разрешения могут быть предоставлены приложению пользователем. Остальные разрешения могут быть предоставлены приложению администратором.</span><span class="sxs-lookup"><span data-stu-id="81f01-p101">One of the following [permissions](/graph/permissions-reference) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="81f01-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="81f01-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="81f01-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="81f01-113">User.Read</span></span>
- <span data-ttu-id="81f01-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81f01-114">User.ReadWrite</span></span>
- <span data-ttu-id="81f01-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="81f01-115">User.Read.All</span></span>
- <span data-ttu-id="81f01-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81f01-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="81f01-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="81f01-117">Directory.Read.All</span></span>
- <span data-ttu-id="81f01-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81f01-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="81f01-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="81f01-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="81f01-120">Общие свойства</span><span class="sxs-lookup"><span data-stu-id="81f01-120">Common properties</span></span>

<span data-ttu-id="81f01-121">Ниже показан набор свойств, используемый по умолчанию и возвращаемый при получении пользователя или выводе списка пользователей.</span><span class="sxs-lookup"><span data-stu-id="81f01-121">The following represent the default set of properties that are returned when getting a user or listing users.</span></span> <span data-ttu-id="81f01-122">Это подмножество всех доступных свойств.</span><span class="sxs-lookup"><span data-stu-id="81f01-122">These are a subset of all available properties.</span></span> <span data-ttu-id="81f01-123">Чтобы получить дополнительные свойства пользователя, используйте параметр запроса `$select`.</span><span class="sxs-lookup"><span data-stu-id="81f01-123">To get more user properties, use the `$select` query parameter.</span></span> <span data-ttu-id="81f01-124">Узнайте, [Как использовать параметр поискового запроса $select ](/graph/query-parameters#select-parameter) и каковы [Свойства, поддерживающие параметр $select поискового запроса](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="81f01-124">Learn [how to use the $select query parameter](/graph/query-parameters#select-parameter) and see [properties that support the $select query parameter](../resources/user.md#properties).</span></span>

|<span data-ttu-id="81f01-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="81f01-125">Property</span></span> |<span data-ttu-id="81f01-126">Описание</span><span class="sxs-lookup"><span data-stu-id="81f01-126">Description</span></span> |
|:----------|:-------------|
|<span data-ttu-id="81f01-127">id</span><span class="sxs-lookup"><span data-stu-id="81f01-127">id</span></span> | <span data-ttu-id="81f01-128">Уникальный идентификатор для пользователя.</span><span class="sxs-lookup"><span data-stu-id="81f01-128">The unique identifier for the user.</span></span>|
|<span data-ttu-id="81f01-129">businessPhones</span><span class="sxs-lookup"><span data-stu-id="81f01-129">businessPhones</span></span> | <span data-ttu-id="81f01-130">Номера телефонов пользователя.</span><span class="sxs-lookup"><span data-stu-id="81f01-130">The user's phone numbers.</span></span>|
|<span data-ttu-id="81f01-131">displayName</span><span class="sxs-lookup"><span data-stu-id="81f01-131">displayName</span></span> | <span data-ttu-id="81f01-132">Имя, отображаемое в адресной книге, для пользователя.</span><span class="sxs-lookup"><span data-stu-id="81f01-132">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="81f01-133">givenName</span><span class="sxs-lookup"><span data-stu-id="81f01-133">givenName</span></span>| <span data-ttu-id="81f01-134">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="81f01-134">The first name of the user.</span></span> |
|<span data-ttu-id="81f01-135">jobTitle</span><span class="sxs-lookup"><span data-stu-id="81f01-135">jobTitle</span></span> | <span data-ttu-id="81f01-136">Должность пользователя.</span><span class="sxs-lookup"><span data-stu-id="81f01-136">The user's job title.</span></span>|
|<span data-ttu-id="81f01-137">mail</span><span class="sxs-lookup"><span data-stu-id="81f01-137">mail</span></span>| <span data-ttu-id="81f01-138">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="81f01-138">The user's email address.</span></span> |
|<span data-ttu-id="81f01-139">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="81f01-139">mobilePhone</span></span> | <span data-ttu-id="81f01-140">Номер мобильного телефона пользователя.</span><span class="sxs-lookup"><span data-stu-id="81f01-140">The user's cellphone number.</span></span>|
|<span data-ttu-id="81f01-141">officeLocation</span><span class="sxs-lookup"><span data-stu-id="81f01-141">officeLocation</span></span> | <span data-ttu-id="81f01-142">Физическое расположение офиса пользователя.</span><span class="sxs-lookup"><span data-stu-id="81f01-142">The user's physical office location.</span></span>|
|<span data-ttu-id="81f01-143">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="81f01-143">preferredLanguage</span></span> | <span data-ttu-id="81f01-144">Предпочитаемый язык пользователя.</span><span class="sxs-lookup"><span data-stu-id="81f01-144">The user's language of preference.</span></span>|
|<span data-ttu-id="81f01-145">surname</span><span class="sxs-lookup"><span data-stu-id="81f01-145">surname</span></span>| <span data-ttu-id="81f01-146">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="81f01-146">The last name of the user.</span></span> |
|<span data-ttu-id="81f01-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="81f01-147">userPrincipalName</span></span>| <span data-ttu-id="81f01-148">Имя участника-пользователя для пользователя.</span><span class="sxs-lookup"><span data-stu-id="81f01-148">The user's principal name.</span></span> |

<span data-ttu-id="81f01-149">Дополнительные сведения и список всех свойств см. в статье об объекте [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="81f01-149">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="81f01-150">Стандартные действия</span><span class="sxs-lookup"><span data-stu-id="81f01-150">Common operations</span></span>

> <span data-ttu-id="81f01-151">**Примечание.** Для выполнения некоторых из этих операций необходимы дополнительные разрешения.</span><span class="sxs-lookup"><span data-stu-id="81f01-151">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="81f01-152">Path</span><span class="sxs-lookup"><span data-stu-id="81f01-152">Path</span></span>    | <span data-ttu-id="81f01-153">Описание</span><span class="sxs-lookup"><span data-stu-id="81f01-153">Description</span></span> |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="81f01-154">Вывод списка пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="81f01-154">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="81f01-155">Получение определенного пользователя по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="81f01-155">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="81f01-156">Получение фотографии профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="81f01-156">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="81f01-157">Получение сведений о руководителе пользователя.</span><span class="sxs-lookup"><span data-stu-id="81f01-157">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="81f01-158">Вывод списка электронных писем пользователя в его основном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="81f01-158">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="81f01-159">Вывод списка предстоящих событий пользователя из его календаря.</span><span class="sxs-lookup"><span data-stu-id="81f01-159">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="81f01-160">Получение хранилища файлов OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="81f01-160">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="81f01-161">Вывод списка групп, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="81f01-161">Lists the groups that the user is a member of.</span></span> |

## <a name="whats-new"></a><span data-ttu-id="81f01-162">Что нового</span><span class="sxs-lookup"><span data-stu-id="81f01-162">What's new</span></span>
<span data-ttu-id="81f01-163">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="81f01-163">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>