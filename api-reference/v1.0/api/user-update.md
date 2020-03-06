---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0aef89c30fc67132352d9d70f9b0fc56e3a9063e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508907"
---
# <a name="update-user"></a><span data-ttu-id="d6c66-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="d6c66-103">Update user</span></span>

<span data-ttu-id="d6c66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6c66-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d6c66-105">Обновление свойств объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6c66-105">Update the properties of a user object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6c66-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6c66-106">Permissions</span></span>
<span data-ttu-id="d6c66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6c66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6c66-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6c66-109">Permission type</span></span>      | <span data-ttu-id="d6c66-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6c66-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6c66-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6c66-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d6c66-112">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d6c66-112">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d6c66-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6c66-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6c66-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6c66-114">User.ReadWrite</span></span>    |
|<span data-ttu-id="d6c66-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6c66-115">Application</span></span> | <span data-ttu-id="d6c66-116">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6c66-116">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="d6c66-117">При обновлении свойства **passwordProfile** необходимо разрешение Directory.AccessAsUser.All.</span><span class="sxs-lookup"><span data-stu-id="d6c66-117">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="d6c66-118">Обновление свойств **businessPhones**, **mobilePhone** или **otherMails** других пользователей разрешается только для пользователей, не являющихся администраторами, или для пользователей, которым назначена одна из следующих ролей: читатель каталога, приглашающий гостей, читатель Центра сообщений или читатель отчетов.</span><span class="sxs-lookup"><span data-stu-id="d6c66-118">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="d6c66-119">Дополнительные сведения см. в разделе "Администратор службы поддержки (паролей)" среди [доступных ролей Azure AD](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="d6c66-119">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="d6c66-120">Это относится к приложениям с предоставленными разрешениями User.ReadWrite.All или Directory.ReadWrite.All (делегированными или для приложений).</span><span class="sxs-lookup"><span data-stu-id="d6c66-120">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="d6c66-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6c66-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="d6c66-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6c66-122">Request headers</span></span>
| <span data-ttu-id="d6c66-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6c66-123">Header</span></span>       | <span data-ttu-id="d6c66-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d6c66-124">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="d6c66-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6c66-125">Authorization</span></span>  | <span data-ttu-id="d6c66-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6c66-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d6c66-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6c66-128">Content-Type</span></span>  | <span data-ttu-id="d6c66-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d6c66-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d6c66-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d6c66-130">Request body</span></span>
<span data-ttu-id="d6c66-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d6c66-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d6c66-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6c66-134">Property</span></span>     | <span data-ttu-id="d6c66-135">Тип</span><span class="sxs-lookup"><span data-stu-id="d6c66-135">Type</span></span>   |<span data-ttu-id="d6c66-136">Описание</span><span class="sxs-lookup"><span data-stu-id="d6c66-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6c66-137">aboutMe</span><span class="sxs-lookup"><span data-stu-id="d6c66-137">aboutMe</span></span>|<span data-ttu-id="d6c66-138">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-138">String</span></span>|<span data-ttu-id="d6c66-139">Свободное текстовое поле, где пользователь может рассказать о себе.</span><span class="sxs-lookup"><span data-stu-id="d6c66-139">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="d6c66-140">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="d6c66-140">accountEnabled</span></span>|<span data-ttu-id="d6c66-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6c66-141">Boolean</span></span>| <span data-ttu-id="d6c66-142">Значение **true** указывает, что учетная запись включена. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="d6c66-142">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="d6c66-143">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6c66-143">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="d6c66-144">birthday</span><span class="sxs-lookup"><span data-stu-id="d6c66-144">birthday</span></span>|<span data-ttu-id="d6c66-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6c66-145">DateTimeOffset</span></span>|<span data-ttu-id="d6c66-p106">День рождения пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d6c66-p106">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d6c66-149">businessPhones</span><span class="sxs-lookup"><span data-stu-id="d6c66-149">businessPhones</span></span>| <span data-ttu-id="d6c66-150">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d6c66-150">String collection</span></span> | <span data-ttu-id="d6c66-p107">Номера телефонов пользователя. ПРИМЕЧАНИЕ. Несмотря на то что это коллекция строк, в качестве этого свойства можно указать только одно число.</span><span class="sxs-lookup"><span data-stu-id="d6c66-p107">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="d6c66-153">city</span><span class="sxs-lookup"><span data-stu-id="d6c66-153">city</span></span>|<span data-ttu-id="d6c66-154">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-154">String</span></span>|<span data-ttu-id="d6c66-155">Город, в котором находится пользователь.</span><span class="sxs-lookup"><span data-stu-id="d6c66-155">The city in which the user is located.</span></span>|
|<span data-ttu-id="d6c66-156">country</span><span class="sxs-lookup"><span data-stu-id="d6c66-156">country</span></span>|<span data-ttu-id="d6c66-157">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-157">String</span></span>|<span data-ttu-id="d6c66-158">Страна или регион, в котором находится пользователь, например "США" или "Соединенное Королевство".</span><span class="sxs-lookup"><span data-stu-id="d6c66-158">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="d6c66-159">department</span><span class="sxs-lookup"><span data-stu-id="d6c66-159">department</span></span>|<span data-ttu-id="d6c66-160">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-160">String</span></span>|<span data-ttu-id="d6c66-161">Название отдела, в котором работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="d6c66-161">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="d6c66-162">displayName</span><span class="sxs-lookup"><span data-stu-id="d6c66-162">displayName</span></span>|<span data-ttu-id="d6c66-163">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-163">String</span></span>|<span data-ttu-id="d6c66-p108">Отображаемое имя пользователя в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="d6c66-p108">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="d6c66-168">givenName</span><span class="sxs-lookup"><span data-stu-id="d6c66-168">givenName</span></span>|<span data-ttu-id="d6c66-169">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-169">String</span></span>|<span data-ttu-id="d6c66-170">Простое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6c66-170">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="d6c66-171">hireDate</span><span class="sxs-lookup"><span data-stu-id="d6c66-171">hireDate</span></span>|<span data-ttu-id="d6c66-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6c66-172">DateTimeOffset</span></span>|<span data-ttu-id="d6c66-p109">Дата найма пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d6c66-p109">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d6c66-176">interests</span><span class="sxs-lookup"><span data-stu-id="d6c66-176">interests</span></span>|<span data-ttu-id="d6c66-177">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d6c66-177">String collection</span></span>|<span data-ttu-id="d6c66-178">Список интересов пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6c66-178">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="d6c66-179">jobTitle</span><span class="sxs-lookup"><span data-stu-id="d6c66-179">jobTitle</span></span>|<span data-ttu-id="d6c66-180">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-180">String</span></span>|<span data-ttu-id="d6c66-181">Должность пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6c66-181">The user’s job title.</span></span>|
|<span data-ttu-id="d6c66-182">mailNickname</span><span class="sxs-lookup"><span data-stu-id="d6c66-182">mailNickname</span></span>|<span data-ttu-id="d6c66-183">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-183">String</span></span>|<span data-ttu-id="d6c66-184">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6c66-184">The mail alias for the user.</span></span> <span data-ttu-id="d6c66-185">Это свойство должно быть указано при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6c66-185">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="d6c66-186">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="d6c66-186">mobilePhone</span></span>|<span data-ttu-id="d6c66-187">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-187">String</span></span>|<span data-ttu-id="d6c66-188">Основной сотовый телефон пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6c66-188">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="d6c66-189">mySite</span><span class="sxs-lookup"><span data-stu-id="d6c66-189">mySite</span></span>|<span data-ttu-id="d6c66-190">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-190">String</span></span>|<span data-ttu-id="d6c66-191">URL-адрес личного сайта пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6c66-191">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="d6c66-192">officeLocation</span><span class="sxs-lookup"><span data-stu-id="d6c66-192">officeLocation</span></span>|<span data-ttu-id="d6c66-193">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-193">String</span></span>|<span data-ttu-id="d6c66-194">Расположение офиса на месте работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6c66-194">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="d6c66-195">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="d6c66-195">onPremisesImmutableId</span></span>|<span data-ttu-id="d6c66-196">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-196">String</span></span>|<span data-ttu-id="d6c66-197">Это свойство используется для сопоставления локальной учетной записи Active Directory с объектом пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d6c66-197">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="d6c66-198">Его необходимо указывать при создании учетной записи пользователя в Graph, если в качестве свойства **userPrincipalName** (имени участника-пользователя) используется федеративный домен.</span><span class="sxs-lookup"><span data-stu-id="d6c66-198">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="d6c66-199">**Важно!** В этом свойстве не допускается использование символов **$** и **_**.</span><span class="sxs-lookup"><span data-stu-id="d6c66-199">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="d6c66-200">otherMails</span><span class="sxs-lookup"><span data-stu-id="d6c66-200">otherMails</span></span>|<span data-ttu-id="d6c66-201">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-201">String</span></span> |<span data-ttu-id="d6c66-202">Список дополнительных адресов электронной почты для пользователя. Например: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="d6c66-202">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="d6c66-203">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="d6c66-203">passwordPolicies</span></span>|<span data-ttu-id="d6c66-204">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-204">String</span></span>|<span data-ttu-id="d6c66-p112">Задает политики паролей для пользователя. Это свойство представляет собой перечисление с единственным возможным значением — "DisableStrongPassword". Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение "DisablePasswordExpiration". Эти значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="d6c66-p112">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="d6c66-209">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="d6c66-209">passwordProfile</span></span>|[<span data-ttu-id="d6c66-210">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="d6c66-210">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="d6c66-p113">Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="d6c66-p113">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="d6c66-216">pastProjects</span><span class="sxs-lookup"><span data-stu-id="d6c66-216">pastProjects</span></span>|<span data-ttu-id="d6c66-217">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d6c66-217">String collection</span></span>|<span data-ttu-id="d6c66-218">Список предыдущих проектов пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6c66-218">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="d6c66-219">postalCode</span><span class="sxs-lookup"><span data-stu-id="d6c66-219">postalCode</span></span>|<span data-ttu-id="d6c66-220">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-220">String</span></span>|<span data-ttu-id="d6c66-p114">Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код.</span><span class="sxs-lookup"><span data-stu-id="d6c66-p114">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="d6c66-224">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="d6c66-224">preferredLanguage</span></span>|<span data-ttu-id="d6c66-225">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-225">String</span></span>|<span data-ttu-id="d6c66-p115">Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1, например "ru-RU".</span><span class="sxs-lookup"><span data-stu-id="d6c66-p115">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="d6c66-228">responsibilities</span><span class="sxs-lookup"><span data-stu-id="d6c66-228">responsibilities</span></span>|<span data-ttu-id="d6c66-229">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d6c66-229">String collection</span></span>|<span data-ttu-id="d6c66-230">Список обязанностей пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6c66-230">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="d6c66-231">schools</span><span class="sxs-lookup"><span data-stu-id="d6c66-231">schools</span></span>|<span data-ttu-id="d6c66-232">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d6c66-232">String collection</span></span>|<span data-ttu-id="d6c66-233">Список учебных заведений, которые посещал пользователь.</span><span class="sxs-lookup"><span data-stu-id="d6c66-233">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="d6c66-234">skills</span><span class="sxs-lookup"><span data-stu-id="d6c66-234">skills</span></span>|<span data-ttu-id="d6c66-235">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d6c66-235">String collection</span></span>|<span data-ttu-id="d6c66-236">Список навыков пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6c66-236">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="d6c66-237">state</span><span class="sxs-lookup"><span data-stu-id="d6c66-237">state</span></span>|<span data-ttu-id="d6c66-238">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-238">String</span></span>|<span data-ttu-id="d6c66-239">Область, республика, край или округ в адресе пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6c66-239">The state or province in the user's address.</span></span>|
|<span data-ttu-id="d6c66-240">streetAddress</span><span class="sxs-lookup"><span data-stu-id="d6c66-240">streetAddress</span></span>|<span data-ttu-id="d6c66-241">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-241">String</span></span>|<span data-ttu-id="d6c66-242">Почтовый адрес места работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6c66-242">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="d6c66-243">surname</span><span class="sxs-lookup"><span data-stu-id="d6c66-243">surname</span></span>|<span data-ttu-id="d6c66-244">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-244">String</span></span>|<span data-ttu-id="d6c66-245">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6c66-245">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="d6c66-246">usageLocation</span><span class="sxs-lookup"><span data-stu-id="d6c66-246">usageLocation</span></span>|<span data-ttu-id="d6c66-247">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-247">String</span></span>|<span data-ttu-id="d6c66-248">Двухбуквенный код страны (по стандарту ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="d6c66-248">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="d6c66-249">Необходим для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в разных странах.</span><span class="sxs-lookup"><span data-stu-id="d6c66-249">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="d6c66-250">Примеры: "RU", "JP", "GB".</span><span class="sxs-lookup"><span data-stu-id="d6c66-250">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="d6c66-251">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="d6c66-251">Not nullable.</span></span>|
|<span data-ttu-id="d6c66-252">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d6c66-252">userPrincipalName</span></span>|<span data-ttu-id="d6c66-253">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-253">String</span></span>|<span data-ttu-id="d6c66-p117">Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](../resources/organization.md). Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="d6c66-p117">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="d6c66-261">userType</span><span class="sxs-lookup"><span data-stu-id="d6c66-261">userType</span></span>|<span data-ttu-id="d6c66-262">String</span><span class="sxs-lookup"><span data-stu-id="d6c66-262">String</span></span>|<span data-ttu-id="d6c66-263">Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость".</span><span class="sxs-lookup"><span data-stu-id="d6c66-263">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

## <a name="response"></a><span data-ttu-id="d6c66-264">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6c66-264">Response</span></span>

<span data-ttu-id="d6c66-265">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d6c66-265">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d6c66-266">Пример</span><span class="sxs-lookup"><span data-stu-id="d6c66-266">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="d6c66-267">Пример 1. Обновление свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="d6c66-267">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="d6c66-268">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6c66-268">Request</span></span>

<span data-ttu-id="d6c66-269">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6c66-269">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d6c66-270">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6c66-270">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "officeLocation": "city-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d6c66-271">C#</span><span class="sxs-lookup"><span data-stu-id="d6c66-271">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6c66-272">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6c66-272">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6c66-273">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6c66-273">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6c66-274">Java</span><span class="sxs-lookup"><span data-stu-id="d6c66-274">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="d6c66-275">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6c66-275">Response</span></span>
<span data-ttu-id="d6c66-276">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d6c66-276">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="d6c66-277">Пример 2. Обновление свойств указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="d6c66-277">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="d6c66-278">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6c66-278">Request</span></span>

<span data-ttu-id="d6c66-279">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6c66-279">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d6c66-280">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6c66-280">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_other_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id}
Content-type: application/json

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "officeLocation": "city-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d6c66-281">C#</span><span class="sxs-lookup"><span data-stu-id="d6c66-281">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6c66-282">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6c66-282">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6c66-283">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6c66-283">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6c66-284">Java</span><span class="sxs-lookup"><span data-stu-id="d6c66-284">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d6c66-285">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6c66-285">Response</span></span>

<span data-ttu-id="d6c66-286">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d6c66-286">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
