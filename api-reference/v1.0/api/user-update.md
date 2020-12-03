---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 9996b69908d6d8882cc7b1085af14b5273c7d55f
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523443"
---
# <a name="update-user"></a><span data-ttu-id="22a78-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="22a78-103">Update user</span></span>

<span data-ttu-id="22a78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22a78-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22a78-105">Обновление свойств объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a78-105">Update the properties of a user object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22a78-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22a78-106">Permissions</span></span>
<span data-ttu-id="22a78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22a78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22a78-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22a78-109">Permission type</span></span>      | <span data-ttu-id="22a78-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22a78-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22a78-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22a78-111">Delegated (work or school account)</span></span> | <span data-ttu-id="22a78-112">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="22a78-112">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="22a78-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22a78-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22a78-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22a78-114">User.ReadWrite</span></span>    |
|<span data-ttu-id="22a78-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22a78-115">Application</span></span> | <span data-ttu-id="22a78-116">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22a78-116">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="22a78-117">При обновлении свойства **passwordProfile** необходимо разрешение Directory.AccessAsUser.All.</span><span class="sxs-lookup"><span data-stu-id="22a78-117">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="22a78-118">Обновление свойств **businessPhones**, **mobilePhone** или **otherMails** других пользователей разрешается только для пользователей, не являющихся администраторами, или для пользователей, которым назначена одна из следующих ролей: читатель каталога, приглашающий гостей, читатель Центра сообщений или читатель отчетов.</span><span class="sxs-lookup"><span data-stu-id="22a78-118">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="22a78-119">Дополнительные сведения см. в разделе "Администратор службы поддержки (паролей)" среди [доступных ролей Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="22a78-119">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="22a78-120">Это относится к приложениям с предоставленными разрешениями User.ReadWrite.All или Directory.ReadWrite.All (делегированными или для приложений).</span><span class="sxs-lookup"><span data-stu-id="22a78-120">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

>[!NOTE]
><span data-ttu-id="22a78-121">Обновление свойства **личностей** требует разрешения User.ManageIdentities.All.</span><span class="sxs-lookup"><span data-stu-id="22a78-121">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="22a78-122">Кроме того, добавление [локальной учетной записи B2C](../resources/objectidentity.md) к существующему объекту **пользователя** не допускается, если только объект **пользователя** не содержит идентификатор локальной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="22a78-122">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="22a78-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22a78-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="22a78-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22a78-124">Request headers</span></span>
| <span data-ttu-id="22a78-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22a78-125">Header</span></span>       | <span data-ttu-id="22a78-126">Значение</span><span class="sxs-lookup"><span data-stu-id="22a78-126">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="22a78-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22a78-127">Authorization</span></span>  | <span data-ttu-id="22a78-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22a78-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="22a78-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="22a78-130">Content-Type</span></span>  | <span data-ttu-id="22a78-131">application/json</span><span class="sxs-lookup"><span data-stu-id="22a78-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="22a78-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="22a78-132">Request body</span></span>
<span data-ttu-id="22a78-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="22a78-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="22a78-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="22a78-136">Property</span></span>     | <span data-ttu-id="22a78-137">Тип</span><span class="sxs-lookup"><span data-stu-id="22a78-137">Type</span></span>   |<span data-ttu-id="22a78-138">Описание</span><span class="sxs-lookup"><span data-stu-id="22a78-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22a78-139">aboutMe</span><span class="sxs-lookup"><span data-stu-id="22a78-139">aboutMe</span></span>|<span data-ttu-id="22a78-140">String</span><span class="sxs-lookup"><span data-stu-id="22a78-140">String</span></span>|<span data-ttu-id="22a78-141">Свободное текстовое поле, где пользователь может рассказать о себе.</span><span class="sxs-lookup"><span data-stu-id="22a78-141">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="22a78-142">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="22a78-142">accountEnabled</span></span>|<span data-ttu-id="22a78-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="22a78-143">Boolean</span></span>| <span data-ttu-id="22a78-144">Значение **true** указывает, что учетная запись включена. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="22a78-144">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="22a78-145">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a78-145">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="22a78-146">birthday</span><span class="sxs-lookup"><span data-stu-id="22a78-146">birthday</span></span>|<span data-ttu-id="22a78-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22a78-147">DateTimeOffset</span></span>|<span data-ttu-id="22a78-p107">День рождения пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="22a78-p107">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="22a78-151">businessPhones</span><span class="sxs-lookup"><span data-stu-id="22a78-151">businessPhones</span></span>| <span data-ttu-id="22a78-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="22a78-152">String collection</span></span> | <span data-ttu-id="22a78-p108">Номера телефонов пользователя. ПРИМЕЧАНИЕ. Несмотря на то что это коллекция строк, в качестве этого свойства можно указать только одно число.</span><span class="sxs-lookup"><span data-stu-id="22a78-p108">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="22a78-155">city</span><span class="sxs-lookup"><span data-stu-id="22a78-155">city</span></span>|<span data-ttu-id="22a78-156">String</span><span class="sxs-lookup"><span data-stu-id="22a78-156">String</span></span>|<span data-ttu-id="22a78-157">Город, в котором находится пользователь.</span><span class="sxs-lookup"><span data-stu-id="22a78-157">The city in which the user is located.</span></span>|
|<span data-ttu-id="22a78-158">country</span><span class="sxs-lookup"><span data-stu-id="22a78-158">country</span></span>|<span data-ttu-id="22a78-159">String</span><span class="sxs-lookup"><span data-stu-id="22a78-159">String</span></span>|<span data-ttu-id="22a78-160">Страна или регион, в котором находится пользователь, например "США" или "Соединенное Королевство".</span><span class="sxs-lookup"><span data-stu-id="22a78-160">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="22a78-161">department</span><span class="sxs-lookup"><span data-stu-id="22a78-161">department</span></span>|<span data-ttu-id="22a78-162">String</span><span class="sxs-lookup"><span data-stu-id="22a78-162">String</span></span>|<span data-ttu-id="22a78-163">Название отдела, в котором работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="22a78-163">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="22a78-164">displayName</span><span class="sxs-lookup"><span data-stu-id="22a78-164">displayName</span></span>|<span data-ttu-id="22a78-165">String</span><span class="sxs-lookup"><span data-stu-id="22a78-165">String</span></span>|<span data-ttu-id="22a78-p109">Отображаемое имя пользователя в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="22a78-p109">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="22a78-170">givenName</span><span class="sxs-lookup"><span data-stu-id="22a78-170">givenName</span></span>|<span data-ttu-id="22a78-171">String</span><span class="sxs-lookup"><span data-stu-id="22a78-171">String</span></span>|<span data-ttu-id="22a78-172">Простое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a78-172">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="22a78-173">hireDate</span><span class="sxs-lookup"><span data-stu-id="22a78-173">hireDate</span></span>|<span data-ttu-id="22a78-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22a78-174">DateTimeOffset</span></span>|<span data-ttu-id="22a78-p110">Дата найма пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="22a78-p110">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="22a78-178">interests</span><span class="sxs-lookup"><span data-stu-id="22a78-178">interests</span></span>|<span data-ttu-id="22a78-179">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="22a78-179">String collection</span></span>|<span data-ttu-id="22a78-180">Список интересов пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a78-180">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="22a78-181">jobTitle</span><span class="sxs-lookup"><span data-stu-id="22a78-181">jobTitle</span></span>|<span data-ttu-id="22a78-182">String</span><span class="sxs-lookup"><span data-stu-id="22a78-182">String</span></span>|<span data-ttu-id="22a78-183">Должность пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a78-183">The user’s job title.</span></span>|
|<span data-ttu-id="22a78-184">почта;</span><span class="sxs-lookup"><span data-stu-id="22a78-184">mail</span></span>|<span data-ttu-id="22a78-185">String</span><span class="sxs-lookup"><span data-stu-id="22a78-185">String</span></span>|<span data-ttu-id="22a78-186">SMTP-адрес пользователя, например "gregory@contoso.onmicrosoft.com".</span><span class="sxs-lookup"><span data-stu-id="22a78-186">The SMTP address for the user, for example, "jeff@contoso.onmicrosoft.com".</span></span> <span data-ttu-id="22a78-187">Изменение этого свойства также приведет к обновлению коллекции пользователя **proxyAddresses**, которая будет включать это значение как SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="22a78-187">Changes to this property will also update the user's **proxyAddresses** collection to include the value as a SMTP address.</span></span> <br><br><span data-ttu-id="22a78-188">Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="22a78-188">Supports $filter.</span></span>|
|<span data-ttu-id="22a78-189">mailNickname</span><span class="sxs-lookup"><span data-stu-id="22a78-189">mailNickname</span></span>|<span data-ttu-id="22a78-190">String</span><span class="sxs-lookup"><span data-stu-id="22a78-190">String</span></span>|<span data-ttu-id="22a78-191">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a78-191">The mail alias for the user.</span></span> <span data-ttu-id="22a78-192">Это свойство должно быть указано при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a78-192">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="22a78-193">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="22a78-193">mobilePhone</span></span>|<span data-ttu-id="22a78-194">String</span><span class="sxs-lookup"><span data-stu-id="22a78-194">String</span></span>|<span data-ttu-id="22a78-195">Основной сотовый телефон пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a78-195">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="22a78-196">mySite</span><span class="sxs-lookup"><span data-stu-id="22a78-196">mySite</span></span>|<span data-ttu-id="22a78-197">String</span><span class="sxs-lookup"><span data-stu-id="22a78-197">String</span></span>|<span data-ttu-id="22a78-198">URL-адрес личного сайта пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a78-198">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="22a78-199">officeLocation</span><span class="sxs-lookup"><span data-stu-id="22a78-199">officeLocation</span></span>|<span data-ttu-id="22a78-200">String</span><span class="sxs-lookup"><span data-stu-id="22a78-200">String</span></span>|<span data-ttu-id="22a78-201">Расположение офиса на месте работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a78-201">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="22a78-202">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="22a78-202">onPremisesImmutableId</span></span>|<span data-ttu-id="22a78-203">String</span><span class="sxs-lookup"><span data-stu-id="22a78-203">String</span></span>|<span data-ttu-id="22a78-204">Это свойство используется для сопоставления локальной учетной записи Active Directory с объектом пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="22a78-204">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="22a78-205">Его необходимо указывать при создании учетной записи пользователя в Graph, если в качестве свойства **userPrincipalName** (имени участника-пользователя) используется федеративный домен.</span><span class="sxs-lookup"><span data-stu-id="22a78-205">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="22a78-206">**Важно!** В этом свойстве не допускается использование символов **$** и **_**.</span><span class="sxs-lookup"><span data-stu-id="22a78-206">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="22a78-207">otherMails</span><span class="sxs-lookup"><span data-stu-id="22a78-207">otherMails</span></span>|<span data-ttu-id="22a78-208">String</span><span class="sxs-lookup"><span data-stu-id="22a78-208">String</span></span> |<span data-ttu-id="22a78-209">Список дополнительных адресов электронной почты для пользователя. Например: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="22a78-209">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="22a78-210">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="22a78-210">passwordPolicies</span></span>|<span data-ttu-id="22a78-211">String</span><span class="sxs-lookup"><span data-stu-id="22a78-211">String</span></span>|<span data-ttu-id="22a78-p114">Задает политики паролей для пользователя. Это свойство представляет собой перечисление с единственным возможным значением — "DisableStrongPassword". Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение "DisablePasswordExpiration". Эти значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="22a78-p114">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="22a78-216">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="22a78-216">passwordProfile</span></span>|[<span data-ttu-id="22a78-217">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="22a78-217">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="22a78-p115">Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="22a78-p115">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="22a78-223">pastProjects</span><span class="sxs-lookup"><span data-stu-id="22a78-223">pastProjects</span></span>|<span data-ttu-id="22a78-224">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="22a78-224">String collection</span></span>|<span data-ttu-id="22a78-225">Список предыдущих проектов пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a78-225">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="22a78-226">postalCode</span><span class="sxs-lookup"><span data-stu-id="22a78-226">postalCode</span></span>|<span data-ttu-id="22a78-227">String</span><span class="sxs-lookup"><span data-stu-id="22a78-227">String</span></span>|<span data-ttu-id="22a78-p116">Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код.</span><span class="sxs-lookup"><span data-stu-id="22a78-p116">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="22a78-231">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="22a78-231">preferredLanguage</span></span>|<span data-ttu-id="22a78-232">String</span><span class="sxs-lookup"><span data-stu-id="22a78-232">String</span></span>|<span data-ttu-id="22a78-p117">Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1, например "ru-RU".</span><span class="sxs-lookup"><span data-stu-id="22a78-p117">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="22a78-235">responsibilities</span><span class="sxs-lookup"><span data-stu-id="22a78-235">responsibilities</span></span>|<span data-ttu-id="22a78-236">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="22a78-236">String collection</span></span>|<span data-ttu-id="22a78-237">Список обязанностей пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a78-237">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="22a78-238">schools</span><span class="sxs-lookup"><span data-stu-id="22a78-238">schools</span></span>|<span data-ttu-id="22a78-239">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="22a78-239">String collection</span></span>|<span data-ttu-id="22a78-240">Список учебных заведений, которые посещал пользователь.</span><span class="sxs-lookup"><span data-stu-id="22a78-240">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="22a78-241">skills</span><span class="sxs-lookup"><span data-stu-id="22a78-241">skills</span></span>|<span data-ttu-id="22a78-242">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="22a78-242">String collection</span></span>|<span data-ttu-id="22a78-243">Список навыков пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a78-243">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="22a78-244">state</span><span class="sxs-lookup"><span data-stu-id="22a78-244">state</span></span>|<span data-ttu-id="22a78-245">String</span><span class="sxs-lookup"><span data-stu-id="22a78-245">String</span></span>|<span data-ttu-id="22a78-246">Область, республика, край или округ в адресе пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a78-246">The state or province in the user's address.</span></span>|
|<span data-ttu-id="22a78-247">streetAddress</span><span class="sxs-lookup"><span data-stu-id="22a78-247">streetAddress</span></span>|<span data-ttu-id="22a78-248">String</span><span class="sxs-lookup"><span data-stu-id="22a78-248">String</span></span>|<span data-ttu-id="22a78-249">Почтовый адрес места работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a78-249">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="22a78-250">surname</span><span class="sxs-lookup"><span data-stu-id="22a78-250">surname</span></span>|<span data-ttu-id="22a78-251">String</span><span class="sxs-lookup"><span data-stu-id="22a78-251">String</span></span>|<span data-ttu-id="22a78-252">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="22a78-252">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="22a78-253">usageLocation</span><span class="sxs-lookup"><span data-stu-id="22a78-253">usageLocation</span></span>|<span data-ttu-id="22a78-254">String</span><span class="sxs-lookup"><span data-stu-id="22a78-254">String</span></span>|<span data-ttu-id="22a78-255">Двухбуквенный код страны (по стандарту ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="22a78-255">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="22a78-256">Необходим для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в разных странах.</span><span class="sxs-lookup"><span data-stu-id="22a78-256">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="22a78-257">Примеры: "RU", "JP", "GB".</span><span class="sxs-lookup"><span data-stu-id="22a78-257">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="22a78-258">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="22a78-258">Not nullable.</span></span>|
|<span data-ttu-id="22a78-259">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="22a78-259">userPrincipalName</span></span>|<span data-ttu-id="22a78-260">String</span><span class="sxs-lookup"><span data-stu-id="22a78-260">String</span></span>|<span data-ttu-id="22a78-p119">Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](../resources/organization.md). Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="22a78-p119">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="22a78-268">userType</span><span class="sxs-lookup"><span data-stu-id="22a78-268">userType</span></span>|<span data-ttu-id="22a78-269">String</span><span class="sxs-lookup"><span data-stu-id="22a78-269">String</span></span>|<span data-ttu-id="22a78-270">Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость".</span><span class="sxs-lookup"><span data-stu-id="22a78-270">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

> [!NOTE] 
> <span data-ttu-id="22a78-271">Следующие свойства не могут быть обновлены с помощью контекста только для приложений: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools** и **skills**.</span><span class="sxs-lookup"><span data-stu-id="22a78-271">The follow properties cannot be updated using an application-only context: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, and **skills**.</span></span>

## <a name="response"></a><span data-ttu-id="22a78-272">Отклик</span><span class="sxs-lookup"><span data-stu-id="22a78-272">Response</span></span>

<span data-ttu-id="22a78-273">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="22a78-273">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="22a78-274">Пример</span><span class="sxs-lookup"><span data-stu-id="22a78-274">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="22a78-275">Пример 1. Обновление свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="22a78-275">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="22a78-276">Запрос</span><span class="sxs-lookup"><span data-stu-id="22a78-276">Request</span></span>

<span data-ttu-id="22a78-277">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22a78-277">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22a78-278">HTTP</span><span class="sxs-lookup"><span data-stu-id="22a78-278">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json

{
  "businessPhones": [
    "+1 425 555 0109"
  ],
  "officeLocation": "18/2111"
}
```
# <a name="c"></a>[<span data-ttu-id="22a78-279">C#</span><span class="sxs-lookup"><span data-stu-id="22a78-279">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22a78-280">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22a78-280">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22a78-281">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22a78-281">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22a78-282">Java</span><span class="sxs-lookup"><span data-stu-id="22a78-282">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="22a78-283">Отклик</span><span class="sxs-lookup"><span data-stu-id="22a78-283">Response</span></span>
<span data-ttu-id="22a78-284">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22a78-284">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="22a78-285">Пример 2. Обновление свойств указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="22a78-285">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="22a78-286">Запрос</span><span class="sxs-lookup"><span data-stu-id="22a78-286">Request</span></span>

<span data-ttu-id="22a78-287">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22a78-287">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="22a78-288">HTTP</span><span class="sxs-lookup"><span data-stu-id="22a78-288">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_other_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id}
Content-type: application/json

{
  "businessPhones": [
    "+1 425 555 0109"
  ],
  "officeLocation": "18/2111"
}
```
# <a name="c"></a>[<span data-ttu-id="22a78-289">C#</span><span class="sxs-lookup"><span data-stu-id="22a78-289">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22a78-290">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22a78-290">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22a78-291">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22a78-291">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22a78-292">Java</span><span class="sxs-lookup"><span data-stu-id="22a78-292">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="22a78-293">Отклик</span><span class="sxs-lookup"><span data-stu-id="22a78-293">Response</span></span>

<span data-ttu-id="22a78-294">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22a78-294">The following example shows the response.</span></span>
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
