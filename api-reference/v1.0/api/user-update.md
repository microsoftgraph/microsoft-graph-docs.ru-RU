---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 4136e62886c91092c62349f0587d60c53f4d2c83
ms.sourcegitcommit: a1a57e803c334e11316dd571ad1b54c95406740e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2020
ms.locfileid: "44413506"
---
# <a name="update-user"></a><span data-ttu-id="b1d29-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="b1d29-103">Update user</span></span>

<span data-ttu-id="b1d29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1d29-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1d29-105">Обновление свойств объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1d29-105">Update the properties of a user object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1d29-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1d29-106">Permissions</span></span>
<span data-ttu-id="b1d29-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1d29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1d29-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1d29-109">Permission type</span></span>      | <span data-ttu-id="b1d29-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1d29-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1d29-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1d29-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b1d29-112">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b1d29-112">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b1d29-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1d29-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1d29-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1d29-114">User.ReadWrite</span></span>    |
|<span data-ttu-id="b1d29-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1d29-115">Application</span></span> | <span data-ttu-id="b1d29-116">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1d29-116">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="b1d29-117">При обновлении свойства **passwordProfile** необходимо разрешение Directory.AccessAsUser.All.</span><span class="sxs-lookup"><span data-stu-id="b1d29-117">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="b1d29-118">Обновление свойств **businessPhones**, **mobilePhone** или **otherMails** других пользователей разрешается только для пользователей, не являющихся администраторами, или для пользователей, которым назначена одна из следующих ролей: читатель каталога, приглашающий гостей, читатель Центра сообщений или читатель отчетов.</span><span class="sxs-lookup"><span data-stu-id="b1d29-118">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="b1d29-119">Дополнительные сведения см. в разделе "Администратор службы поддержки (паролей)" среди [доступных ролей Azure AD](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="b1d29-119">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="b1d29-120">Это относится к приложениям с предоставленными разрешениями User.ReadWrite.All или Directory.ReadWrite.All (делегированными или для приложений).</span><span class="sxs-lookup"><span data-stu-id="b1d29-120">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

>[!NOTE]
><span data-ttu-id="b1d29-121">Обновление свойства **личностей** требует разрешения User.ManageIdentities.All.</span><span class="sxs-lookup"><span data-stu-id="b1d29-121">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="b1d29-122">Кроме того, добавление [локальной учетной записи B2C](../resources/objectidentity.md) к существующему объекту **пользователя** не допускается, если только объект **пользователя** не содержит идентификатор локальной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="b1d29-122">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="b1d29-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1d29-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="b1d29-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1d29-124">Request headers</span></span>
| <span data-ttu-id="b1d29-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1d29-125">Header</span></span>       | <span data-ttu-id="b1d29-126">Значение</span><span class="sxs-lookup"><span data-stu-id="b1d29-126">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="b1d29-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1d29-127">Authorization</span></span>  | <span data-ttu-id="b1d29-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1d29-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b1d29-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1d29-130">Content-Type</span></span>  | <span data-ttu-id="b1d29-131">application/json</span><span class="sxs-lookup"><span data-stu-id="b1d29-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1d29-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b1d29-132">Request body</span></span>
<span data-ttu-id="b1d29-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b1d29-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b1d29-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1d29-136">Property</span></span>     | <span data-ttu-id="b1d29-137">Тип</span><span class="sxs-lookup"><span data-stu-id="b1d29-137">Type</span></span>   |<span data-ttu-id="b1d29-138">Описание</span><span class="sxs-lookup"><span data-stu-id="b1d29-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1d29-139">aboutMe</span><span class="sxs-lookup"><span data-stu-id="b1d29-139">aboutMe</span></span>|<span data-ttu-id="b1d29-140">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-140">String</span></span>|<span data-ttu-id="b1d29-141">Свободное текстовое поле, где пользователь может рассказать о себе.</span><span class="sxs-lookup"><span data-stu-id="b1d29-141">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="b1d29-142">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="b1d29-142">accountEnabled</span></span>|<span data-ttu-id="b1d29-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1d29-143">Boolean</span></span>| <span data-ttu-id="b1d29-144">Значение **true** указывает, что учетная запись включена. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="b1d29-144">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="b1d29-145">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1d29-145">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="b1d29-146">birthday</span><span class="sxs-lookup"><span data-stu-id="b1d29-146">birthday</span></span>|<span data-ttu-id="b1d29-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1d29-147">DateTimeOffset</span></span>|<span data-ttu-id="b1d29-p107">День рождения пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b1d29-p107">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b1d29-151">businessPhones</span><span class="sxs-lookup"><span data-stu-id="b1d29-151">businessPhones</span></span>| <span data-ttu-id="b1d29-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b1d29-152">String collection</span></span> | <span data-ttu-id="b1d29-p108">Номера телефонов пользователя. ПРИМЕЧАНИЕ. Несмотря на то что это коллекция строк, в качестве этого свойства можно указать только одно число.</span><span class="sxs-lookup"><span data-stu-id="b1d29-p108">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="b1d29-155">city</span><span class="sxs-lookup"><span data-stu-id="b1d29-155">city</span></span>|<span data-ttu-id="b1d29-156">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-156">String</span></span>|<span data-ttu-id="b1d29-157">Город, в котором находится пользователь.</span><span class="sxs-lookup"><span data-stu-id="b1d29-157">The city in which the user is located.</span></span>|
|<span data-ttu-id="b1d29-158">country</span><span class="sxs-lookup"><span data-stu-id="b1d29-158">country</span></span>|<span data-ttu-id="b1d29-159">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-159">String</span></span>|<span data-ttu-id="b1d29-160">Страна или регион, в котором находится пользователь, например "США" или "Соединенное Королевство".</span><span class="sxs-lookup"><span data-stu-id="b1d29-160">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="b1d29-161">department</span><span class="sxs-lookup"><span data-stu-id="b1d29-161">department</span></span>|<span data-ttu-id="b1d29-162">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-162">String</span></span>|<span data-ttu-id="b1d29-163">Название отдела, в котором работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="b1d29-163">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="b1d29-164">displayName</span><span class="sxs-lookup"><span data-stu-id="b1d29-164">displayName</span></span>|<span data-ttu-id="b1d29-165">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-165">String</span></span>|<span data-ttu-id="b1d29-p109">Отображаемое имя пользователя в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="b1d29-p109">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="b1d29-170">givenName</span><span class="sxs-lookup"><span data-stu-id="b1d29-170">givenName</span></span>|<span data-ttu-id="b1d29-171">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-171">String</span></span>|<span data-ttu-id="b1d29-172">Простое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1d29-172">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="b1d29-173">hireDate</span><span class="sxs-lookup"><span data-stu-id="b1d29-173">hireDate</span></span>|<span data-ttu-id="b1d29-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1d29-174">DateTimeOffset</span></span>|<span data-ttu-id="b1d29-p110">Дата найма пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b1d29-p110">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b1d29-178">interests</span><span class="sxs-lookup"><span data-stu-id="b1d29-178">interests</span></span>|<span data-ttu-id="b1d29-179">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b1d29-179">String collection</span></span>|<span data-ttu-id="b1d29-180">Список интересов пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1d29-180">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="b1d29-181">jobTitle</span><span class="sxs-lookup"><span data-stu-id="b1d29-181">jobTitle</span></span>|<span data-ttu-id="b1d29-182">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-182">String</span></span>|<span data-ttu-id="b1d29-183">Должность пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1d29-183">The user’s job title.</span></span>|
|<span data-ttu-id="b1d29-184">mailNickname</span><span class="sxs-lookup"><span data-stu-id="b1d29-184">mailNickname</span></span>|<span data-ttu-id="b1d29-185">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-185">String</span></span>|<span data-ttu-id="b1d29-186">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1d29-186">The mail alias for the user.</span></span> <span data-ttu-id="b1d29-187">Это свойство должно быть указано при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1d29-187">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="b1d29-188">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="b1d29-188">mobilePhone</span></span>|<span data-ttu-id="b1d29-189">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-189">String</span></span>|<span data-ttu-id="b1d29-190">Основной сотовый телефон пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1d29-190">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="b1d29-191">mySite</span><span class="sxs-lookup"><span data-stu-id="b1d29-191">mySite</span></span>|<span data-ttu-id="b1d29-192">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-192">String</span></span>|<span data-ttu-id="b1d29-193">URL-адрес личного сайта пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1d29-193">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="b1d29-194">officeLocation</span><span class="sxs-lookup"><span data-stu-id="b1d29-194">officeLocation</span></span>|<span data-ttu-id="b1d29-195">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-195">String</span></span>|<span data-ttu-id="b1d29-196">Расположение офиса на месте работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1d29-196">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="b1d29-197">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="b1d29-197">onPremisesImmutableId</span></span>|<span data-ttu-id="b1d29-198">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-198">String</span></span>|<span data-ttu-id="b1d29-199">Это свойство используется для сопоставления локальной учетной записи Active Directory с объектом пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1d29-199">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="b1d29-200">Его необходимо указывать при создании учетной записи пользователя в Graph, если в качестве свойства **userPrincipalName** (имени участника-пользователя) используется федеративный домен.</span><span class="sxs-lookup"><span data-stu-id="b1d29-200">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="b1d29-201">**Важно!** В этом свойстве не допускается использование символов **$** и **_**.</span><span class="sxs-lookup"><span data-stu-id="b1d29-201">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="b1d29-202">otherMails</span><span class="sxs-lookup"><span data-stu-id="b1d29-202">otherMails</span></span>|<span data-ttu-id="b1d29-203">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-203">String</span></span> |<span data-ttu-id="b1d29-204">Список дополнительных адресов электронной почты для пользователя. Например: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="b1d29-204">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="b1d29-205">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="b1d29-205">passwordPolicies</span></span>|<span data-ttu-id="b1d29-206">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-206">String</span></span>|<span data-ttu-id="b1d29-p113">Задает политики паролей для пользователя. Это свойство представляет собой перечисление с единственным возможным значением — "DisableStrongPassword". Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение "DisablePasswordExpiration". Эти значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="b1d29-p113">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="b1d29-211">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="b1d29-211">passwordProfile</span></span>|[<span data-ttu-id="b1d29-212">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="b1d29-212">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="b1d29-p114">Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="b1d29-p114">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="b1d29-218">pastProjects</span><span class="sxs-lookup"><span data-stu-id="b1d29-218">pastProjects</span></span>|<span data-ttu-id="b1d29-219">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b1d29-219">String collection</span></span>|<span data-ttu-id="b1d29-220">Список предыдущих проектов пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1d29-220">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="b1d29-221">postalCode</span><span class="sxs-lookup"><span data-stu-id="b1d29-221">postalCode</span></span>|<span data-ttu-id="b1d29-222">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-222">String</span></span>|<span data-ttu-id="b1d29-p115">Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код.</span><span class="sxs-lookup"><span data-stu-id="b1d29-p115">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="b1d29-226">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="b1d29-226">preferredLanguage</span></span>|<span data-ttu-id="b1d29-227">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-227">String</span></span>|<span data-ttu-id="b1d29-p116">Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1, например "ru-RU".</span><span class="sxs-lookup"><span data-stu-id="b1d29-p116">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="b1d29-230">responsibilities</span><span class="sxs-lookup"><span data-stu-id="b1d29-230">responsibilities</span></span>|<span data-ttu-id="b1d29-231">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b1d29-231">String collection</span></span>|<span data-ttu-id="b1d29-232">Список обязанностей пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1d29-232">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="b1d29-233">schools</span><span class="sxs-lookup"><span data-stu-id="b1d29-233">schools</span></span>|<span data-ttu-id="b1d29-234">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b1d29-234">String collection</span></span>|<span data-ttu-id="b1d29-235">Список учебных заведений, которые посещал пользователь.</span><span class="sxs-lookup"><span data-stu-id="b1d29-235">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="b1d29-236">skills</span><span class="sxs-lookup"><span data-stu-id="b1d29-236">skills</span></span>|<span data-ttu-id="b1d29-237">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b1d29-237">String collection</span></span>|<span data-ttu-id="b1d29-238">Список навыков пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1d29-238">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="b1d29-239">state</span><span class="sxs-lookup"><span data-stu-id="b1d29-239">state</span></span>|<span data-ttu-id="b1d29-240">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-240">String</span></span>|<span data-ttu-id="b1d29-241">Область, республика, край или округ в адресе пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1d29-241">The state or province in the user's address.</span></span>|
|<span data-ttu-id="b1d29-242">streetAddress</span><span class="sxs-lookup"><span data-stu-id="b1d29-242">streetAddress</span></span>|<span data-ttu-id="b1d29-243">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-243">String</span></span>|<span data-ttu-id="b1d29-244">Почтовый адрес места работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1d29-244">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="b1d29-245">surname</span><span class="sxs-lookup"><span data-stu-id="b1d29-245">surname</span></span>|<span data-ttu-id="b1d29-246">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-246">String</span></span>|<span data-ttu-id="b1d29-247">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1d29-247">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="b1d29-248">usageLocation</span><span class="sxs-lookup"><span data-stu-id="b1d29-248">usageLocation</span></span>|<span data-ttu-id="b1d29-249">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-249">String</span></span>|<span data-ttu-id="b1d29-250">Двухбуквенный код страны (по стандарту ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="b1d29-250">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="b1d29-251">Необходим для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в разных странах.</span><span class="sxs-lookup"><span data-stu-id="b1d29-251">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="b1d29-252">Примеры: "RU", "JP", "GB".</span><span class="sxs-lookup"><span data-stu-id="b1d29-252">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="b1d29-253">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="b1d29-253">Not nullable.</span></span>|
|<span data-ttu-id="b1d29-254">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1d29-254">userPrincipalName</span></span>|<span data-ttu-id="b1d29-255">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-255">String</span></span>|<span data-ttu-id="b1d29-p118">Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](../resources/organization.md). Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="b1d29-p118">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="b1d29-263">userType</span><span class="sxs-lookup"><span data-stu-id="b1d29-263">userType</span></span>|<span data-ttu-id="b1d29-264">String</span><span class="sxs-lookup"><span data-stu-id="b1d29-264">String</span></span>|<span data-ttu-id="b1d29-265">Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость".</span><span class="sxs-lookup"><span data-stu-id="b1d29-265">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

> [!NOTE] 
> <span data-ttu-id="b1d29-266">Следующие свойства невозможно обновить с использованием контекста, доступного только для приложений: **aboutMe**, **день рождения**, **HireDate**, **интересы**, **личный сайт**, **пастпрожектс**, **преферреднаме**, **обязанности**, **учебные**заведения и **навыки**.</span><span class="sxs-lookup"><span data-stu-id="b1d29-266">The follow properties cannot be updated using an application-only context: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, and **skills**.</span></span>

## <a name="response"></a><span data-ttu-id="b1d29-267">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1d29-267">Response</span></span>

<span data-ttu-id="b1d29-268">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b1d29-268">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b1d29-269">Пример</span><span class="sxs-lookup"><span data-stu-id="b1d29-269">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="b1d29-270">Пример 1. Обновление свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="b1d29-270">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="b1d29-271">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1d29-271">Request</span></span>

<span data-ttu-id="b1d29-272">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1d29-272">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b1d29-273">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1d29-273">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b1d29-274">C#</span><span class="sxs-lookup"><span data-stu-id="b1d29-274">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1d29-275">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1d29-275">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1d29-276">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1d29-276">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b1d29-277">Java</span><span class="sxs-lookup"><span data-stu-id="b1d29-277">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b1d29-278">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1d29-278">Response</span></span>
<span data-ttu-id="b1d29-279">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1d29-279">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="b1d29-280">Пример 2. Обновление свойств указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="b1d29-280">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="b1d29-281">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1d29-281">Request</span></span>

<span data-ttu-id="b1d29-282">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1d29-282">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b1d29-283">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1d29-283">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b1d29-284">C#</span><span class="sxs-lookup"><span data-stu-id="b1d29-284">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1d29-285">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1d29-285">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1d29-286">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1d29-286">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b1d29-287">Java</span><span class="sxs-lookup"><span data-stu-id="b1d29-287">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b1d29-288">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1d29-288">Response</span></span>

<span data-ttu-id="b1d29-289">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1d29-289">The following example shows the response.</span></span>
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
