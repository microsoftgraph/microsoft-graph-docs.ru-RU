---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: af8d2c99d814c8a7b82e905e3fbbc7d5709bb9d6
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396858"
---
# <a name="update-user"></a><span data-ttu-id="65742-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="65742-103">Update user</span></span>

<span data-ttu-id="65742-104">Обновление свойств объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="65742-104">Update the properties of a user object.</span></span>

## <a name="permissions"></a><span data-ttu-id="65742-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65742-105">Permissions</span></span>
<span data-ttu-id="65742-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65742-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65742-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65742-108">Permission type</span></span>      | <span data-ttu-id="65742-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65742-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65742-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65742-110">Delegated (work or school account)</span></span> | <span data-ttu-id="65742-111">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="65742-111">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="65742-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65742-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65742-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65742-113">User.ReadWrite</span></span>    |
|<span data-ttu-id="65742-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65742-114">Application</span></span> | <span data-ttu-id="65742-115">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65742-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="65742-116">При обновлении свойства **passwordProfile** необходимо разрешение Directory.AccessAsUser.All.</span><span class="sxs-lookup"><span data-stu-id="65742-116">When updating the passwordProfile property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="65742-117">Обновление свойств **businessPhones**, **mobilePhone** или **otherMails** других пользователей разрешается только для пользователей, не являющихся администраторами, или для пользователей, которым назначена одна из следующих ролей: читатель каталога, приглашающий гостей, читатель Центра сообщений или читатель отчетов.</span><span class="sxs-lookup"><span data-stu-id="65742-117">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="65742-118">Дополнительные сведения см. в разделе "Администратор службы поддержки (паролей)" среди [доступных ролей Azure AD](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="65742-118">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="65742-119">Это относится к приложениям с предоставленными разрешениями User.ReadWrite.All или Directory.ReadWrite.All (делегированными или для приложений).</span><span class="sxs-lookup"><span data-stu-id="65742-119">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="65742-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65742-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="65742-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65742-121">Request headers</span></span>
| <span data-ttu-id="65742-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65742-122">Header</span></span>       | <span data-ttu-id="65742-123">Значение</span><span class="sxs-lookup"><span data-stu-id="65742-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="65742-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65742-124">Authorization</span></span>  | <span data-ttu-id="65742-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65742-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="65742-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65742-127">Content-Type</span></span>  | <span data-ttu-id="65742-128">application/json</span><span class="sxs-lookup"><span data-stu-id="65742-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="65742-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="65742-129">Request body</span></span>
<span data-ttu-id="65742-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="65742-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="65742-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="65742-133">Property</span></span>     | <span data-ttu-id="65742-134">Тип</span><span class="sxs-lookup"><span data-stu-id="65742-134">Type</span></span>   |<span data-ttu-id="65742-135">Описание</span><span class="sxs-lookup"><span data-stu-id="65742-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65742-136">aboutMe</span><span class="sxs-lookup"><span data-stu-id="65742-136">aboutMe</span></span>|<span data-ttu-id="65742-137">String</span><span class="sxs-lookup"><span data-stu-id="65742-137">String</span></span>|<span data-ttu-id="65742-138">Свободное текстовое поле, где пользователь может рассказать о себе.</span><span class="sxs-lookup"><span data-stu-id="65742-138">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="65742-139">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="65742-139">accountEnabled</span></span>|<span data-ttu-id="65742-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="65742-140">Boolean</span></span>| <span data-ttu-id="65742-141">Значение **true** указывает, что учетная запись включена. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="65742-141">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="65742-142">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="65742-142">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="65742-143">birthday</span><span class="sxs-lookup"><span data-stu-id="65742-143">birthday</span></span>|<span data-ttu-id="65742-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65742-144">DateTimeOffset</span></span>|<span data-ttu-id="65742-p106">День рождения пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="65742-p106">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="65742-148">businessPhones</span><span class="sxs-lookup"><span data-stu-id="65742-148">businessPhones</span></span>| <span data-ttu-id="65742-149">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="65742-149">String collection</span></span> | <span data-ttu-id="65742-p107">Номера телефонов пользователя. ПРИМЕЧАНИЕ. Несмотря на то что это коллекция строк, в качестве этого свойства можно указать только одно число.</span><span class="sxs-lookup"><span data-stu-id="65742-p107">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="65742-152">city</span><span class="sxs-lookup"><span data-stu-id="65742-152">city</span></span>|<span data-ttu-id="65742-153">String</span><span class="sxs-lookup"><span data-stu-id="65742-153">String</span></span>|<span data-ttu-id="65742-154">Город, в котором находится пользователь.</span><span class="sxs-lookup"><span data-stu-id="65742-154">The city in which the user is located.</span></span>|
|<span data-ttu-id="65742-155">country</span><span class="sxs-lookup"><span data-stu-id="65742-155">country</span></span>|<span data-ttu-id="65742-156">String</span><span class="sxs-lookup"><span data-stu-id="65742-156">String</span></span>|<span data-ttu-id="65742-157">Страна или регион, в котором находится пользователь, например "США" или "Соединенное Королевство".</span><span class="sxs-lookup"><span data-stu-id="65742-157">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="65742-158">department</span><span class="sxs-lookup"><span data-stu-id="65742-158">department</span></span>|<span data-ttu-id="65742-159">String</span><span class="sxs-lookup"><span data-stu-id="65742-159">String</span></span>|<span data-ttu-id="65742-160">Название отдела, в котором работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="65742-160">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="65742-161">displayName</span><span class="sxs-lookup"><span data-stu-id="65742-161">displayName</span></span>|<span data-ttu-id="65742-162">String</span><span class="sxs-lookup"><span data-stu-id="65742-162">String</span></span>|<span data-ttu-id="65742-p108">Отображаемое имя пользователя в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="65742-p108">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="65742-167">givenName</span><span class="sxs-lookup"><span data-stu-id="65742-167">givenName</span></span>|<span data-ttu-id="65742-168">String</span><span class="sxs-lookup"><span data-stu-id="65742-168">String</span></span>|<span data-ttu-id="65742-169">Простое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="65742-169">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="65742-170">hireDate</span><span class="sxs-lookup"><span data-stu-id="65742-170">hireDate</span></span>|<span data-ttu-id="65742-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65742-171">DateTimeOffset</span></span>|<span data-ttu-id="65742-p109">Дата найма пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="65742-p109">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="65742-175">interests</span><span class="sxs-lookup"><span data-stu-id="65742-175">interests</span></span>|<span data-ttu-id="65742-176">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="65742-176">String collection</span></span>|<span data-ttu-id="65742-177">Список интересов пользователя.</span><span class="sxs-lookup"><span data-stu-id="65742-177">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="65742-178">jobTitle</span><span class="sxs-lookup"><span data-stu-id="65742-178">jobTitle</span></span>|<span data-ttu-id="65742-179">String</span><span class="sxs-lookup"><span data-stu-id="65742-179">String</span></span>|<span data-ttu-id="65742-180">Должность пользователя.</span><span class="sxs-lookup"><span data-stu-id="65742-180">The user’s job title.</span></span>|
|<span data-ttu-id="65742-181">mailNickname</span><span class="sxs-lookup"><span data-stu-id="65742-181">mailNickname</span></span>|<span data-ttu-id="65742-182">String</span><span class="sxs-lookup"><span data-stu-id="65742-182">String</span></span>|<span data-ttu-id="65742-183">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="65742-183">The mail alias for the user.</span></span> <span data-ttu-id="65742-184">Это свойство должно быть указано при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="65742-184">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="65742-185">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="65742-185">mobilePhone</span></span>|<span data-ttu-id="65742-186">String</span><span class="sxs-lookup"><span data-stu-id="65742-186">String</span></span>|<span data-ttu-id="65742-187">Основной сотовый телефон пользователя.</span><span class="sxs-lookup"><span data-stu-id="65742-187">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="65742-188">mySite</span><span class="sxs-lookup"><span data-stu-id="65742-188">mySite</span></span>|<span data-ttu-id="65742-189">String</span><span class="sxs-lookup"><span data-stu-id="65742-189">String</span></span>|<span data-ttu-id="65742-190">URL-адрес личного сайта пользователя.</span><span class="sxs-lookup"><span data-stu-id="65742-190">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="65742-191">officeLocation</span><span class="sxs-lookup"><span data-stu-id="65742-191">officeLocation</span></span>|<span data-ttu-id="65742-192">String</span><span class="sxs-lookup"><span data-stu-id="65742-192">String</span></span>|<span data-ttu-id="65742-193">Расположение офиса на месте работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="65742-193">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="65742-194">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="65742-194">onPremisesImmutableId</span></span>|<span data-ttu-id="65742-195">String</span><span class="sxs-lookup"><span data-stu-id="65742-195">String</span></span>|<span data-ttu-id="65742-196">Это свойство используется для сопоставления локальной учетной записи Active Directory с объектом пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="65742-196">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="65742-197">Его необходимо указывать при создании учетной записи пользователя в Graph, если в качестве свойства **userPrincipalName** (имени участника-пользователя) используется федеративный домен.</span><span class="sxs-lookup"><span data-stu-id="65742-197">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="65742-198">**Важно!** В этом свойстве не допускается использование символов **$** и **_**.</span><span class="sxs-lookup"><span data-stu-id="65742-198">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="65742-199">otherMails</span><span class="sxs-lookup"><span data-stu-id="65742-199">otherMails</span></span>|<span data-ttu-id="65742-200">String</span><span class="sxs-lookup"><span data-stu-id="65742-200">String</span></span> |<span data-ttu-id="65742-201">Список дополнительных адресов электронной почты для пользователя. Например: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="65742-201">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="65742-202">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="65742-202">passwordPolicies</span></span>|<span data-ttu-id="65742-203">String</span><span class="sxs-lookup"><span data-stu-id="65742-203">String</span></span>|<span data-ttu-id="65742-p112">Задает политики паролей для пользователя. Это свойство представляет собой перечисление с единственным возможным значением — "DisableStrongPassword". Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение "DisablePasswordExpiration". Эти значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="65742-p112">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="65742-208">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="65742-208">passwordProfile</span></span>|[<span data-ttu-id="65742-209">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="65742-209">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="65742-p113">Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="65742-p113">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="65742-215">pastProjects</span><span class="sxs-lookup"><span data-stu-id="65742-215">pastProjects</span></span>|<span data-ttu-id="65742-216">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="65742-216">String collection</span></span>|<span data-ttu-id="65742-217">Список предыдущих проектов пользователя.</span><span class="sxs-lookup"><span data-stu-id="65742-217">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="65742-218">postalCode</span><span class="sxs-lookup"><span data-stu-id="65742-218">postalCode</span></span>|<span data-ttu-id="65742-219">String</span><span class="sxs-lookup"><span data-stu-id="65742-219">String</span></span>|<span data-ttu-id="65742-p114">Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код.</span><span class="sxs-lookup"><span data-stu-id="65742-p114">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="65742-223">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="65742-223">preferredLanguage</span></span>|<span data-ttu-id="65742-224">String</span><span class="sxs-lookup"><span data-stu-id="65742-224">String</span></span>|<span data-ttu-id="65742-p115">Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1, например "ru-RU".</span><span class="sxs-lookup"><span data-stu-id="65742-p115">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="65742-227">responsibilities</span><span class="sxs-lookup"><span data-stu-id="65742-227">responsibilities</span></span>|<span data-ttu-id="65742-228">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="65742-228">String collection</span></span>|<span data-ttu-id="65742-229">Список обязанностей пользователя.</span><span class="sxs-lookup"><span data-stu-id="65742-229">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="65742-230">schools</span><span class="sxs-lookup"><span data-stu-id="65742-230">schools</span></span>|<span data-ttu-id="65742-231">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="65742-231">String collection</span></span>|<span data-ttu-id="65742-232">Список учебных заведений, которые посещал пользователь.</span><span class="sxs-lookup"><span data-stu-id="65742-232">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="65742-233">skills</span><span class="sxs-lookup"><span data-stu-id="65742-233">skills</span></span>|<span data-ttu-id="65742-234">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="65742-234">String collection</span></span>|<span data-ttu-id="65742-235">Список навыков пользователя.</span><span class="sxs-lookup"><span data-stu-id="65742-235">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="65742-236">state</span><span class="sxs-lookup"><span data-stu-id="65742-236">state</span></span>|<span data-ttu-id="65742-237">String</span><span class="sxs-lookup"><span data-stu-id="65742-237">String</span></span>|<span data-ttu-id="65742-238">Область, республика, край или округ в адресе пользователя.</span><span class="sxs-lookup"><span data-stu-id="65742-238">The state or province in the user's address.</span></span>|
|<span data-ttu-id="65742-239">streetAddress</span><span class="sxs-lookup"><span data-stu-id="65742-239">streetAddress</span></span>|<span data-ttu-id="65742-240">String</span><span class="sxs-lookup"><span data-stu-id="65742-240">String</span></span>|<span data-ttu-id="65742-241">Почтовый адрес места работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="65742-241">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="65742-242">surname</span><span class="sxs-lookup"><span data-stu-id="65742-242">surname</span></span>|<span data-ttu-id="65742-243">String</span><span class="sxs-lookup"><span data-stu-id="65742-243">String</span></span>|<span data-ttu-id="65742-244">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="65742-244">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="65742-245">usageLocation</span><span class="sxs-lookup"><span data-stu-id="65742-245">usageLocation</span></span>|<span data-ttu-id="65742-246">String</span><span class="sxs-lookup"><span data-stu-id="65742-246">String</span></span>|<span data-ttu-id="65742-247">Двухбуквенный код страны (по стандарту ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="65742-247">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="65742-248">Необходим для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в разных странах.</span><span class="sxs-lookup"><span data-stu-id="65742-248">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="65742-249">Примеры: "RU", "JP", "GB".</span><span class="sxs-lookup"><span data-stu-id="65742-249">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="65742-250">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="65742-250">Not nullable.</span></span>|
|<span data-ttu-id="65742-251">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="65742-251">userPrincipalName</span></span>|<span data-ttu-id="65742-252">String</span><span class="sxs-lookup"><span data-stu-id="65742-252">String</span></span>|<span data-ttu-id="65742-p117">Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](../resources/organization.md). Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="65742-p117">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="65742-260">userType</span><span class="sxs-lookup"><span data-stu-id="65742-260">userType</span></span>|<span data-ttu-id="65742-261">String</span><span class="sxs-lookup"><span data-stu-id="65742-261">String</span></span>|<span data-ttu-id="65742-262">Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость".</span><span class="sxs-lookup"><span data-stu-id="65742-262">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

## <a name="response"></a><span data-ttu-id="65742-263">Отклик</span><span class="sxs-lookup"><span data-stu-id="65742-263">Response</span></span>

<span data-ttu-id="65742-264">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="65742-264">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="65742-265">Пример</span><span class="sxs-lookup"><span data-stu-id="65742-265">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="65742-266">Пример 1. Обновление свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="65742-266">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="65742-267">Запрос</span><span class="sxs-lookup"><span data-stu-id="65742-267">Request</span></span>

<span data-ttu-id="65742-268">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65742-268">The following example shows how to create a request context.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="65742-269">HTTP</span><span class="sxs-lookup"><span data-stu-id="65742-269">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="65742-270">C#</span><span class="sxs-lookup"><span data-stu-id="65742-270">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65742-271">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65742-271">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65742-272">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65742-272">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="65742-273">Java</span><span class="sxs-lookup"><span data-stu-id="65742-273">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="65742-274">Отклик</span><span class="sxs-lookup"><span data-stu-id="65742-274">Response</span></span>
<span data-ttu-id="65742-275">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="65742-275">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="65742-276">Пример 2. Обновление свойств указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="65742-276">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="65742-277">Запрос</span><span class="sxs-lookup"><span data-stu-id="65742-277">Request</span></span>

<span data-ttu-id="65742-278">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65742-278">The following example shows how to create a request context.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="65742-279">HTTP</span><span class="sxs-lookup"><span data-stu-id="65742-279">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="65742-280">C#</span><span class="sxs-lookup"><span data-stu-id="65742-280">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65742-281">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65742-281">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65742-282">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65742-282">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="65742-283">Java</span><span class="sxs-lookup"><span data-stu-id="65742-283">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="65742-284">Отклик</span><span class="sxs-lookup"><span data-stu-id="65742-284">Response</span></span>

<span data-ttu-id="65742-285">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="65742-285">The following example shows the response.</span></span>
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
