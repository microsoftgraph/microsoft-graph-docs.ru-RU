---
title: Работа с пользователями в Microsoft Graph
description: Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b98bdd3f84171823942b3a48dd49a8993597a5ee
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572180"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="458e9-103">Работа с пользователями в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="458e9-103">Working with users in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="458e9-104">Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.</span><span class="sxs-lookup"><span data-stu-id="458e9-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="458e9-105">Вы можете получить доступ к пользователям через Microsoft Graph двумя указанными ниже способами.</span><span class="sxs-lookup"><span data-stu-id="458e9-105">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="458e9-106">По идентификатору пользователя (`/users/{id}`).</span><span class="sxs-lookup"><span data-stu-id="458e9-106">By their ID, `/users/{id}`</span></span> 
- <span data-ttu-id="458e9-107">С помощью псевдонима `/me` (который совпадает с `/users/{signed-in user's id}`) для пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="458e9-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="458e9-108">Авторизация</span><span class="sxs-lookup"><span data-stu-id="458e9-108">Authorization</span></span>
<span data-ttu-id="458e9-p101">Для операций доступа к пользователям необходимо одно из указанных ниже [разрешений](https://developer.microsoft.com/graph/docs/authorization/permission_scopes). Первые три разрешения могут быть предоставлены приложению пользователем. Остальные разрешения могут быть предоставлены приложению администратором.</span><span class="sxs-lookup"><span data-stu-id="458e9-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="458e9-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="458e9-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="458e9-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="458e9-113">User.Read</span></span>
- <span data-ttu-id="458e9-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="458e9-114">User.ReadWrite</span></span>
- <span data-ttu-id="458e9-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="458e9-115">User.Read.All</span></span>
- <span data-ttu-id="458e9-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="458e9-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="458e9-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="458e9-117">Directory.Read.All</span></span>
- <span data-ttu-id="458e9-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="458e9-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="458e9-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="458e9-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="458e9-120">Общие свойства</span><span class="sxs-lookup"><span data-stu-id="458e9-120">Common properties</span></span>

<span data-ttu-id="458e9-121">Ниже показан набор свойств, используемый по умолчанию и возвращаемый при получении пользователя или выводе списка пользователей.</span><span class="sxs-lookup"><span data-stu-id="458e9-121">The following represent the default set of properties that are returned when getting a user or listing users.</span></span> <span data-ttu-id="458e9-122">Это подмножество всех доступных свойств.</span><span class="sxs-lookup"><span data-stu-id="458e9-122">These are a subset of all available properties.</span></span> <span data-ttu-id="458e9-123">Чтобы получить дополнительные свойства пользователя, используйте параметр запроса `$select`.</span><span class="sxs-lookup"><span data-stu-id="458e9-123">To get more user properties, use the `$select` query parameter.</span></span> 

|<span data-ttu-id="458e9-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="458e9-124">Property</span></span> |<span data-ttu-id="458e9-125">Описание</span><span class="sxs-lookup"><span data-stu-id="458e9-125">Description</span></span> |
|:----------|:-------------|
|<span data-ttu-id="458e9-126">id</span><span class="sxs-lookup"><span data-stu-id="458e9-126">id</span></span> | <span data-ttu-id="458e9-127">Уникальный идентификатор для пользователя.</span><span class="sxs-lookup"><span data-stu-id="458e9-127">The unique identifier for the user.</span></span>|
|<span data-ttu-id="458e9-128">businessPhones</span><span class="sxs-lookup"><span data-stu-id="458e9-128">businessPhones</span></span> | <span data-ttu-id="458e9-129">Номера телефонов пользователя.</span><span class="sxs-lookup"><span data-stu-id="458e9-129">The user's phone numbers.</span></span>|
|<span data-ttu-id="458e9-130">displayName</span><span class="sxs-lookup"><span data-stu-id="458e9-130">displayName</span></span> | <span data-ttu-id="458e9-131">Имя, отображаемое в адресной книге, для пользователя.</span><span class="sxs-lookup"><span data-stu-id="458e9-131">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="458e9-132">givenName</span><span class="sxs-lookup"><span data-stu-id="458e9-132">givenName</span></span>| <span data-ttu-id="458e9-133">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="458e9-133">The first name of the user.</span></span> |
|<span data-ttu-id="458e9-134">jobTitle</span><span class="sxs-lookup"><span data-stu-id="458e9-134">jobTitle</span></span> | <span data-ttu-id="458e9-135">Должность пользователя.</span><span class="sxs-lookup"><span data-stu-id="458e9-135">The user's job title.</span></span>|
|<span data-ttu-id="458e9-136">mail</span><span class="sxs-lookup"><span data-stu-id="458e9-136">mail</span></span>| <span data-ttu-id="458e9-137">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="458e9-137">The user's email address.</span></span> |
|<span data-ttu-id="458e9-138">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="458e9-138">mobilePhone</span></span> | <span data-ttu-id="458e9-139">Номер мобильного телефона пользователя.</span><span class="sxs-lookup"><span data-stu-id="458e9-139">The user's cellphone number.</span></span>|
|<span data-ttu-id="458e9-140">officeLocation</span><span class="sxs-lookup"><span data-stu-id="458e9-140">officeLocation</span></span> | <span data-ttu-id="458e9-141">Физическое расположение офиса пользователя.</span><span class="sxs-lookup"><span data-stu-id="458e9-141">The user's physical office location.</span></span>|
|<span data-ttu-id="458e9-142">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="458e9-142">preferredLanguage</span></span> | <span data-ttu-id="458e9-143">Предпочитаемый язык пользователя.</span><span class="sxs-lookup"><span data-stu-id="458e9-143">The user's language of preference.</span></span>|
|<span data-ttu-id="458e9-144">surname</span><span class="sxs-lookup"><span data-stu-id="458e9-144">surname</span></span>| <span data-ttu-id="458e9-145">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="458e9-145">The last name of the user.</span></span> |
|<span data-ttu-id="458e9-146">mail</span><span class="sxs-lookup"><span data-stu-id="458e9-146">mail</span></span>| <span data-ttu-id="458e9-147">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="458e9-147">The user's email address.</span></span> |
|<span data-ttu-id="458e9-148">photo</span><span class="sxs-lookup"><span data-stu-id="458e9-148">photo</span></span>| <span data-ttu-id="458e9-149">Фотография профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="458e9-149">The user's profile photo. Read-only.</span></span> |
|<span data-ttu-id="458e9-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="458e9-150">userPrincipalName</span></span>| <span data-ttu-id="458e9-151">Имя участника-пользователя для пользователя.</span><span class="sxs-lookup"><span data-stu-id="458e9-151">The user's principal name.</span></span> |

<span data-ttu-id="458e9-152">Дополнительные сведения и список всех свойств см. в статье об объекте [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="458e9-152">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="458e9-153">Стандартные действия</span><span class="sxs-lookup"><span data-stu-id="458e9-153">Common operations</span></span>
><span data-ttu-id="458e9-154">**Примечание.** Для выполнения некоторых из этих операций необходимы дополнительные разрешения.</span><span class="sxs-lookup"><span data-stu-id="458e9-154">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="458e9-155">Path</span><span class="sxs-lookup"><span data-stu-id="458e9-155">Path</span></span>    | <span data-ttu-id="458e9-156">Описание</span><span class="sxs-lookup"><span data-stu-id="458e9-156">Description</span></span> |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="458e9-157">Вывод списка пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="458e9-157">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="458e9-158">Получение определенного пользователя по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="458e9-158">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="458e9-159">Получение фотографии профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="458e9-159">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="458e9-160">Получение сведений о руководителе пользователя.</span><span class="sxs-lookup"><span data-stu-id="458e9-160">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="458e9-161">Вывод списка электронных писем пользователя в его основном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="458e9-161">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="458e9-162">Вывод списка предстоящих событий пользователя из его календаря.</span><span class="sxs-lookup"><span data-stu-id="458e9-162">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="458e9-163">Получение хранилища файлов OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="458e9-163">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="458e9-164">Вывод списка групп, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="458e9-164">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="458e9-165">Вывод списка команд Microsoft Teams, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="458e9-165">Get the Microsoft Teams that the user is a direct member of.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/users.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
