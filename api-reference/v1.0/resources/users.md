---
title: Работа с пользователями в Microsoft Graph
description: Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bfd7778d3fdc9675880b98a356dd690c4b1eaec8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456887"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="19b7f-103">Работа с пользователями в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="19b7f-103">Working with users in Microsoft Graph</span></span>

<span data-ttu-id="19b7f-104">Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.</span><span class="sxs-lookup"><span data-stu-id="19b7f-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="19b7f-105">Вы можете получить доступ к [пользователям](user.md) через Microsoft Graph двумя указанными ниже способами.</span><span class="sxs-lookup"><span data-stu-id="19b7f-105">You can access [users](user.md) through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="19b7f-106">По идентификатору пользователя (`/users/{id | userPrincipalName}`).</span><span class="sxs-lookup"><span data-stu-id="19b7f-106">By their ID, `/users/{id | userPrincipalName}`</span></span> 
- <span data-ttu-id="19b7f-107">С помощью псевдонима `/me` (который совпадает с `/users/{signed-in user's id}`) для пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="19b7f-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="19b7f-108">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19b7f-108">Authorization</span></span>

<span data-ttu-id="19b7f-p101">Для операций доступа к пользователям необходимо одно из указанных ниже [разрешений](https://developer.microsoft.com/graph/docs/authorization/permission_scopes). Первые три разрешения могут быть предоставлены приложению пользователем. Остальные разрешения могут быть предоставлены приложению администратором.</span><span class="sxs-lookup"><span data-stu-id="19b7f-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="19b7f-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="19b7f-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="19b7f-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="19b7f-113">User.Read</span></span>
- <span data-ttu-id="19b7f-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19b7f-114">User.ReadWrite</span></span>
- <span data-ttu-id="19b7f-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="19b7f-115">User.Read.All</span></span>
- <span data-ttu-id="19b7f-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19b7f-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="19b7f-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="19b7f-117">Directory.Read.All</span></span>
- <span data-ttu-id="19b7f-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19b7f-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="19b7f-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19b7f-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="19b7f-120">Общие свойства</span><span class="sxs-lookup"><span data-stu-id="19b7f-120">Common properties</span></span>

<span data-ttu-id="19b7f-121">Ниже показан набор свойств, используемый по умолчанию и возвращаемый при получении пользователя или выводе списка пользователей.</span><span class="sxs-lookup"><span data-stu-id="19b7f-121">The following represent the default set of properties that are returned when getting a user or listing users.</span></span> <span data-ttu-id="19b7f-122">Это подмножество всех доступных свойств.</span><span class="sxs-lookup"><span data-stu-id="19b7f-122">These are a subset of all available properties.</span></span> <span data-ttu-id="19b7f-123">Чтобы получить дополнительные свойства пользователя, используйте параметр запроса `$select`.</span><span class="sxs-lookup"><span data-stu-id="19b7f-123">To get more user properties, use the `$select` query parameter.</span></span> 

|<span data-ttu-id="19b7f-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="19b7f-124">Property</span></span> |<span data-ttu-id="19b7f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="19b7f-125">Description</span></span> |
|:----------|:-------------|
|<span data-ttu-id="19b7f-126">id</span><span class="sxs-lookup"><span data-stu-id="19b7f-126">id</span></span> | <span data-ttu-id="19b7f-127">Уникальный идентификатор для пользователя.</span><span class="sxs-lookup"><span data-stu-id="19b7f-127">The unique identifier for the user.</span></span>|
|<span data-ttu-id="19b7f-128">businessPhones</span><span class="sxs-lookup"><span data-stu-id="19b7f-128">businessPhones</span></span> | <span data-ttu-id="19b7f-129">Номера телефонов пользователя.</span><span class="sxs-lookup"><span data-stu-id="19b7f-129">The user's phone numbers.</span></span>|
|<span data-ttu-id="19b7f-130">displayName</span><span class="sxs-lookup"><span data-stu-id="19b7f-130">displayName</span></span> | <span data-ttu-id="19b7f-131">Имя, отображаемое в адресной книге, для пользователя.</span><span class="sxs-lookup"><span data-stu-id="19b7f-131">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="19b7f-132">givenName</span><span class="sxs-lookup"><span data-stu-id="19b7f-132">givenName</span></span>| <span data-ttu-id="19b7f-133">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="19b7f-133">The first name of the user.</span></span> |
|<span data-ttu-id="19b7f-134">jobTitle</span><span class="sxs-lookup"><span data-stu-id="19b7f-134">jobTitle</span></span> | <span data-ttu-id="19b7f-135">Должность пользователя.</span><span class="sxs-lookup"><span data-stu-id="19b7f-135">The user's job title.</span></span>|
|<span data-ttu-id="19b7f-136">mail</span><span class="sxs-lookup"><span data-stu-id="19b7f-136">mail</span></span>| <span data-ttu-id="19b7f-137">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="19b7f-137">The user's email address.</span></span> |
|<span data-ttu-id="19b7f-138">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="19b7f-138">mobilePhone</span></span> | <span data-ttu-id="19b7f-139">Номер мобильного телефона пользователя.</span><span class="sxs-lookup"><span data-stu-id="19b7f-139">The user's cellphone number.</span></span>|
|<span data-ttu-id="19b7f-140">officeLocation</span><span class="sxs-lookup"><span data-stu-id="19b7f-140">officeLocation</span></span> | <span data-ttu-id="19b7f-141">Физическое расположение офиса пользователя.</span><span class="sxs-lookup"><span data-stu-id="19b7f-141">The user's physical office location.</span></span>|
|<span data-ttu-id="19b7f-142">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="19b7f-142">preferredLanguage</span></span> | <span data-ttu-id="19b7f-143">Предпочитаемый язык пользователя.</span><span class="sxs-lookup"><span data-stu-id="19b7f-143">The user's language of preference.</span></span>|
|<span data-ttu-id="19b7f-144">surname</span><span class="sxs-lookup"><span data-stu-id="19b7f-144">surname</span></span>| <span data-ttu-id="19b7f-145">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="19b7f-145">The last name of the user.</span></span> |
|<span data-ttu-id="19b7f-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="19b7f-146">userPrincipalName</span></span>| <span data-ttu-id="19b7f-147">Имя участника-пользователя для пользователя.</span><span class="sxs-lookup"><span data-stu-id="19b7f-147">The user's principal name.</span></span> |

<br/>

<span data-ttu-id="19b7f-148">Дополнительные сведения и список всех свойств см. в статье об объекте [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="19b7f-148">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="19b7f-149">Стандартные действия</span><span class="sxs-lookup"><span data-stu-id="19b7f-149">Common operations</span></span>

> <span data-ttu-id="19b7f-150">**Примечание.** Для выполнения некоторых из этих операций необходимы дополнительные разрешения.</span><span class="sxs-lookup"><span data-stu-id="19b7f-150">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="19b7f-151">Path</span><span class="sxs-lookup"><span data-stu-id="19b7f-151">Path</span></span>    | <span data-ttu-id="19b7f-152">Описание</span><span class="sxs-lookup"><span data-stu-id="19b7f-152">Description</span></span> |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="19b7f-153">Вывод списка пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="19b7f-153">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="19b7f-154">Получение определенного пользователя по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="19b7f-154">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="19b7f-155">Получение фотографии профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="19b7f-155">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="19b7f-156">Получение сведений о руководителе пользователя.</span><span class="sxs-lookup"><span data-stu-id="19b7f-156">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="19b7f-157">Вывод списка электронных писем пользователя в его основном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="19b7f-157">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="19b7f-158">Вывод списка предстоящих событий пользователя из его календаря.</span><span class="sxs-lookup"><span data-stu-id="19b7f-158">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="19b7f-159">Получение хранилища файлов OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="19b7f-159">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="19b7f-160">Вывод списка групп, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="19b7f-160">Lists the groups that the user is a member of.</span></span> |
