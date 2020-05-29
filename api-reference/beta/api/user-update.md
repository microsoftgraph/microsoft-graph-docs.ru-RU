---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d11283c8f456087d0a4ce816734c9ca05152cbe0
ms.sourcegitcommit: a1a57e803c334e11316dd571ad1b54c95406740e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2020
ms.locfileid: "44413457"
---
# <a name="update-user"></a><span data-ttu-id="446c1-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="446c1-103">Update user</span></span>

<span data-ttu-id="446c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="446c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="446c1-105">Обновление свойств объекта [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="446c1-105">Update the properties of a [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="446c1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="446c1-106">Permissions</span></span>
<span data-ttu-id="446c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="446c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="446c1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="446c1-109">Permission type</span></span>      | <span data-ttu-id="446c1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="446c1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="446c1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="446c1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="446c1-112">User. ReadWrite, User. ReadWrite. ALL, User. Манажеидентитиес. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="446c1-112">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="446c1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="446c1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="446c1-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="446c1-114">User.ReadWrite</span></span>    |
|<span data-ttu-id="446c1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="446c1-115">Application</span></span> | <span data-ttu-id="446c1-116">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="446c1-116">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="446c1-117">При обновлении свойства **passwordProfile** необходимо разрешение Directory.AccessAsUser.All.</span><span class="sxs-lookup"><span data-stu-id="446c1-117">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="446c1-118">Обновление свойств **businessPhones**, **mobilePhone** или **otherMails** других пользователей разрешается только для пользователей, не являющихся администраторами, или для пользователей, которым назначена одна из следующих ролей: читатель каталога, приглашающий гостей, читатель Центра сообщений или читатель отчетов.</span><span class="sxs-lookup"><span data-stu-id="446c1-118">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="446c1-119">Дополнительные сведения см. в разделе "Администратор службы поддержки (паролей)" среди [доступных ролей Azure AD](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="446c1-119">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="446c1-120">Это относится к приложениям с предоставленными разрешениями User.ReadWrite.All или Directory.ReadWrite.All (делегированными или для приложений).</span><span class="sxs-lookup"><span data-stu-id="446c1-120">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

>[!NOTE]
><span data-ttu-id="446c1-121">Обновление свойства **личностей** требует разрешения User.ManageIdentities.All.</span><span class="sxs-lookup"><span data-stu-id="446c1-121">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="446c1-122">Кроме того, добавление [локальной учетной записи B2C](../resources/objectidentity.md) к существующему объекту **пользователя** не допускается, если только объект **пользователя** не содержит идентификатор локальной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="446c1-122">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="446c1-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="446c1-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="446c1-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="446c1-124">Request headers</span></span>
| <span data-ttu-id="446c1-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="446c1-125">Header</span></span>       | <span data-ttu-id="446c1-126">Значение</span><span class="sxs-lookup"><span data-stu-id="446c1-126">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="446c1-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="446c1-127">Authorization</span></span>  | <span data-ttu-id="446c1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="446c1-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="446c1-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="446c1-130">Content-Type</span></span>  | <span data-ttu-id="446c1-131">application/json</span><span class="sxs-lookup"><span data-stu-id="446c1-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="446c1-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="446c1-132">Request body</span></span>
<span data-ttu-id="446c1-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="446c1-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="446c1-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="446c1-136">Property</span></span>     | <span data-ttu-id="446c1-137">Тип</span><span class="sxs-lookup"><span data-stu-id="446c1-137">Type</span></span>   |<span data-ttu-id="446c1-138">Описание</span><span class="sxs-lookup"><span data-stu-id="446c1-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="446c1-139">aboutMe</span><span class="sxs-lookup"><span data-stu-id="446c1-139">aboutMe</span></span>|<span data-ttu-id="446c1-140">String</span><span class="sxs-lookup"><span data-stu-id="446c1-140">String</span></span>|<span data-ttu-id="446c1-141">Свободное текстовое поле, где пользователь может рассказать о себе.</span><span class="sxs-lookup"><span data-stu-id="446c1-141">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="446c1-142">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="446c1-142">accountEnabled</span></span>|<span data-ttu-id="446c1-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="446c1-143">Boolean</span></span>| <span data-ttu-id="446c1-144">Значение **true** указывает, что учетная запись включена. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="446c1-144">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="446c1-145">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-145">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="446c1-146">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="446c1-146">assignedLicenses</span></span>|<span data-ttu-id="446c1-147">Коллекция [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="446c1-147">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="446c1-p107">Лицензии, назначенные пользователю. Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="446c1-p107">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="446c1-150">birthday</span><span class="sxs-lookup"><span data-stu-id="446c1-150">birthday</span></span>|<span data-ttu-id="446c1-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="446c1-151">DateTimeOffset</span></span>|<span data-ttu-id="446c1-p108">День рождения пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="446c1-p108">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="446c1-155">businessPhones</span><span class="sxs-lookup"><span data-stu-id="446c1-155">businessPhones</span></span>| <span data-ttu-id="446c1-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="446c1-156">String collection</span></span> | <span data-ttu-id="446c1-p109">Номера телефонов пользователя. ПРИМЕЧАНИЕ. Несмотря на то что это коллекция строк, в качестве этого свойства можно указать только одно число.</span><span class="sxs-lookup"><span data-stu-id="446c1-p109">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="446c1-159">city</span><span class="sxs-lookup"><span data-stu-id="446c1-159">city</span></span>|<span data-ttu-id="446c1-160">String</span><span class="sxs-lookup"><span data-stu-id="446c1-160">String</span></span>|<span data-ttu-id="446c1-161">Город, в котором находится пользователь.</span><span class="sxs-lookup"><span data-stu-id="446c1-161">The city in which the user is located.</span></span>|
|<span data-ttu-id="446c1-162">country</span><span class="sxs-lookup"><span data-stu-id="446c1-162">country</span></span>|<span data-ttu-id="446c1-163">String</span><span class="sxs-lookup"><span data-stu-id="446c1-163">String</span></span>|<span data-ttu-id="446c1-164">Страна или регион, в котором находится пользователь, например "США" или "Соединенное Королевство".</span><span class="sxs-lookup"><span data-stu-id="446c1-164">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="446c1-165">department</span><span class="sxs-lookup"><span data-stu-id="446c1-165">department</span></span>|<span data-ttu-id="446c1-166">String</span><span class="sxs-lookup"><span data-stu-id="446c1-166">String</span></span>|<span data-ttu-id="446c1-167">Название отдела, в котором работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="446c1-167">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="446c1-168">displayName</span><span class="sxs-lookup"><span data-stu-id="446c1-168">displayName</span></span>|<span data-ttu-id="446c1-169">String</span><span class="sxs-lookup"><span data-stu-id="446c1-169">String</span></span>|<span data-ttu-id="446c1-p110">Отображаемое имя пользователя в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="446c1-p110">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="446c1-174">employeeId</span><span class="sxs-lookup"><span data-stu-id="446c1-174">employeeId</span></span>|<span data-ttu-id="446c1-175">String</span><span class="sxs-lookup"><span data-stu-id="446c1-175">String</span></span>|<span data-ttu-id="446c1-176">Идентификатор сотрудника, назначенный пользователю организацией.</span><span class="sxs-lookup"><span data-stu-id="446c1-176">The employee identifier assigned to the user by the organization.</span></span>|
|<span data-ttu-id="446c1-177">givenName</span><span class="sxs-lookup"><span data-stu-id="446c1-177">givenName</span></span>|<span data-ttu-id="446c1-178">String</span><span class="sxs-lookup"><span data-stu-id="446c1-178">String</span></span>|<span data-ttu-id="446c1-179">Простое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-179">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="446c1-180">hireDate</span><span class="sxs-lookup"><span data-stu-id="446c1-180">hireDate</span></span>|<span data-ttu-id="446c1-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="446c1-181">DateTimeOffset</span></span>|<span data-ttu-id="446c1-p111">Дата найма пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="446c1-p111">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="446c1-185">identities</span><span class="sxs-lookup"><span data-stu-id="446c1-185">identities</span></span>|<span data-ttu-id="446c1-186">Коллекция [objectIdentity](../resources/objectidentity.md)</span><span class="sxs-lookup"><span data-stu-id="446c1-186">[objectIdentity](../resources/objectidentity.md) collection</span></span>| <span data-ttu-id="446c1-187">Представляет удостоверения, которые можно использовать для входа в учетную запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-187">Represents the identities that can be used to sign in to this user account.</span></span> <span data-ttu-id="446c1-188">Удостоверение может предоставляться корпорацией Майкрософт, организациями или поставщиками удостоверений социальных сетей, такими как Facebook, Google и Майкрософт, и привязывается к учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-188">An identity can be provided by Microsoft, by organizations, or by social identity providers such as Facebook, Google, and Microsoft, and tied to a user account.</span></span> <span data-ttu-id="446c1-189">Все обновления для **удостоверений** заменят всю коллекцию, и необходимо указать идентификатор userPrincipalName **сигнинтипе** в коллекции.</span><span class="sxs-lookup"><span data-stu-id="446c1-189">Any update to **identities** will replace the entire collection and you must supply the userPrincipalName **signInType** identity in the collection.</span></span>|
|<span data-ttu-id="446c1-190">interests;</span><span class="sxs-lookup"><span data-stu-id="446c1-190">interests</span></span>|<span data-ttu-id="446c1-191">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="446c1-191">String collection</span></span>|<span data-ttu-id="446c1-192">Список интересов пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-192">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="446c1-193">jobTitle</span><span class="sxs-lookup"><span data-stu-id="446c1-193">jobTitle</span></span>|<span data-ttu-id="446c1-194">String</span><span class="sxs-lookup"><span data-stu-id="446c1-194">String</span></span>|<span data-ttu-id="446c1-195">Должность пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-195">The user’s job title.</span></span>|
|<span data-ttu-id="446c1-196">mailNickname</span><span class="sxs-lookup"><span data-stu-id="446c1-196">mailNickname</span></span>|<span data-ttu-id="446c1-197">String</span><span class="sxs-lookup"><span data-stu-id="446c1-197">String</span></span>|<span data-ttu-id="446c1-198">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-198">The mail alias for the user.</span></span> <span data-ttu-id="446c1-199">Это свойство должно быть указано при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-199">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="446c1-200">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="446c1-200">mobilePhone</span></span>|<span data-ttu-id="446c1-201">String</span><span class="sxs-lookup"><span data-stu-id="446c1-201">String</span></span>|<span data-ttu-id="446c1-202">Основной сотовый телефон пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-202">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="446c1-203">mySite</span><span class="sxs-lookup"><span data-stu-id="446c1-203">mySite</span></span>|<span data-ttu-id="446c1-204">String</span><span class="sxs-lookup"><span data-stu-id="446c1-204">String</span></span>|<span data-ttu-id="446c1-205">URL-адрес личного сайта пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-205">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="446c1-206">officeLocation</span><span class="sxs-lookup"><span data-stu-id="446c1-206">officeLocation</span></span>|<span data-ttu-id="446c1-207">String</span><span class="sxs-lookup"><span data-stu-id="446c1-207">String</span></span>|<span data-ttu-id="446c1-208">Расположение офиса на месте работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-208">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="446c1-209">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="446c1-209">onPremisesImmutableId</span></span>|<span data-ttu-id="446c1-210">String</span><span class="sxs-lookup"><span data-stu-id="446c1-210">String</span></span>|<span data-ttu-id="446c1-211">Это свойство используется для сопоставления локальной учетной записи Active Directory с объектом пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="446c1-211">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="446c1-212">Его необходимо указывать при создании учетной записи пользователя в Graph, если в качестве свойства **userPrincipalName** (имени участника-пользователя) используется федеративный домен.</span><span class="sxs-lookup"><span data-stu-id="446c1-212">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="446c1-213">**Важно!** В этом свойстве не допускается использование символов **$** и **_**.</span><span class="sxs-lookup"><span data-stu-id="446c1-213">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="446c1-214">otherMails</span><span class="sxs-lookup"><span data-stu-id="446c1-214">otherMails</span></span>|<span data-ttu-id="446c1-215">String</span><span class="sxs-lookup"><span data-stu-id="446c1-215">String</span></span> |<span data-ttu-id="446c1-216">Список дополнительных адресов электронной почты для пользователя. Например: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="446c1-216">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="446c1-217">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="446c1-217">passwordPolicies</span></span>|<span data-ttu-id="446c1-218">String</span><span class="sxs-lookup"><span data-stu-id="446c1-218">String</span></span>|<span data-ttu-id="446c1-p115">Задает политики паролей для пользователя. Это свойство представляет собой перечисление с единственным возможным значением — "DisableStrongPassword". Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение "DisablePasswordExpiration". Эти значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="446c1-p115">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="446c1-223">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="446c1-223">passwordProfile</span></span>|[<span data-ttu-id="446c1-224">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="446c1-224">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="446c1-p116">Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="446c1-p116">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="446c1-230">pastProjects</span><span class="sxs-lookup"><span data-stu-id="446c1-230">pastProjects</span></span>|<span data-ttu-id="446c1-231">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="446c1-231">String collection</span></span>|<span data-ttu-id="446c1-232">Список предыдущих проектов пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-232">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="446c1-233">postalCode</span><span class="sxs-lookup"><span data-stu-id="446c1-233">postalCode</span></span>|<span data-ttu-id="446c1-234">String</span><span class="sxs-lookup"><span data-stu-id="446c1-234">String</span></span>|<span data-ttu-id="446c1-p117">Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код.</span><span class="sxs-lookup"><span data-stu-id="446c1-p117">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="446c1-238">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="446c1-238">preferredLanguage</span></span>|<span data-ttu-id="446c1-239">String</span><span class="sxs-lookup"><span data-stu-id="446c1-239">String</span></span>|<span data-ttu-id="446c1-p118">Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1, например "ru-RU".</span><span class="sxs-lookup"><span data-stu-id="446c1-p118">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="446c1-242">responsibilities</span><span class="sxs-lookup"><span data-stu-id="446c1-242">responsibilities</span></span>|<span data-ttu-id="446c1-243">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="446c1-243">String collection</span></span>|<span data-ttu-id="446c1-244">Список обязанностей пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-244">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="446c1-245">schools</span><span class="sxs-lookup"><span data-stu-id="446c1-245">schools</span></span>|<span data-ttu-id="446c1-246">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="446c1-246">String collection</span></span>|<span data-ttu-id="446c1-247">Список учебных заведений, которые посещал пользователь.</span><span class="sxs-lookup"><span data-stu-id="446c1-247">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="446c1-248">skills</span><span class="sxs-lookup"><span data-stu-id="446c1-248">skills</span></span>|<span data-ttu-id="446c1-249">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="446c1-249">String collection</span></span>|<span data-ttu-id="446c1-250">Список навыков пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-250">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="446c1-251">state</span><span class="sxs-lookup"><span data-stu-id="446c1-251">state</span></span>|<span data-ttu-id="446c1-252">Строка</span><span class="sxs-lookup"><span data-stu-id="446c1-252">String</span></span>|<span data-ttu-id="446c1-253">Область, республика, край или округ в адресе пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-253">The state or province in the user's address.</span></span>|
|<span data-ttu-id="446c1-254">streetAddress</span><span class="sxs-lookup"><span data-stu-id="446c1-254">streetAddress</span></span>|<span data-ttu-id="446c1-255">String</span><span class="sxs-lookup"><span data-stu-id="446c1-255">String</span></span>|<span data-ttu-id="446c1-256">Почтовый адрес места работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-256">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="446c1-257">surname</span><span class="sxs-lookup"><span data-stu-id="446c1-257">surname</span></span>|<span data-ttu-id="446c1-258">String</span><span class="sxs-lookup"><span data-stu-id="446c1-258">String</span></span>|<span data-ttu-id="446c1-259">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="446c1-259">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="446c1-260">usageLocation</span><span class="sxs-lookup"><span data-stu-id="446c1-260">usageLocation</span></span>|<span data-ttu-id="446c1-261">String</span><span class="sxs-lookup"><span data-stu-id="446c1-261">String</span></span>|<span data-ttu-id="446c1-262">Двухбуквенный код страны (по стандарту ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="446c1-262">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="446c1-263">Необходим для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в разных странах.</span><span class="sxs-lookup"><span data-stu-id="446c1-263">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="446c1-264">Примеры: "RU", "JP", "GB".</span><span class="sxs-lookup"><span data-stu-id="446c1-264">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="446c1-265">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="446c1-265">Not nullable.</span></span>|
|<span data-ttu-id="446c1-266">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="446c1-266">userPrincipalName</span></span>|<span data-ttu-id="446c1-267">String</span><span class="sxs-lookup"><span data-stu-id="446c1-267">String</span></span>|<span data-ttu-id="446c1-p120">Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](../resources/organization.md). Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="446c1-p120">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="446c1-275">userType</span><span class="sxs-lookup"><span data-stu-id="446c1-275">userType</span></span>|<span data-ttu-id="446c1-276">String</span><span class="sxs-lookup"><span data-stu-id="446c1-276">String</span></span>|<span data-ttu-id="446c1-277">Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость".</span><span class="sxs-lookup"><span data-stu-id="446c1-277">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

<span data-ttu-id="446c1-278">Так как ресурс **User** поддерживает [расширения](/graph/extensibility-overview), с помощью операции можно `PATCH` добавлять, обновлять или удалять собственные данные, зависящие от приложения, в пользовательских свойствах расширения в существующем **пользовательском** экземпляре.</span><span class="sxs-lookup"><span data-stu-id="446c1-278">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **user** instance.</span></span>

> [!NOTE] 
> <span data-ttu-id="446c1-279">Следующие свойства невозможно обновить с использованием контекста, доступного только для приложений: **aboutMe**, **день рождения**, **HireDate**, **интересы**, **личный сайт**, **пастпрожектс**, **преферреднаме**, **обязанности**, **учебные**заведения и **навыки**.</span><span class="sxs-lookup"><span data-stu-id="446c1-279">The follow properties cannot be updated using an application-only context: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, and **skills**.</span></span>

## <a name="response"></a><span data-ttu-id="446c1-280">Отклик</span><span class="sxs-lookup"><span data-stu-id="446c1-280">Response</span></span>

<span data-ttu-id="446c1-281">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="446c1-281">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="446c1-282">Пример</span><span class="sxs-lookup"><span data-stu-id="446c1-282">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="446c1-283">Пример 1. Обновление свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="446c1-283">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="446c1-284">Запрос</span><span class="sxs-lookup"><span data-stu-id="446c1-284">Request</span></span>

<span data-ttu-id="446c1-285">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="446c1-285">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="446c1-286">HTTP</span><span class="sxs-lookup"><span data-stu-id="446c1-286">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/beta/me
Content-type: application/json

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "officeLocation": "city-value"
}
```
# <a name="c"></a>[<span data-ttu-id="446c1-287">C#</span><span class="sxs-lookup"><span data-stu-id="446c1-287">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="446c1-288">JavaScript</span><span class="sxs-lookup"><span data-stu-id="446c1-288">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="446c1-289">Objective-C</span><span class="sxs-lookup"><span data-stu-id="446c1-289">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="446c1-290">Отклик</span><span class="sxs-lookup"><span data-stu-id="446c1-290">Response</span></span>

<span data-ttu-id="446c1-291">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="446c1-291">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="446c1-292">Пример 2. Обновление свойств указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="446c1-292">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="446c1-293">Запрос</span><span class="sxs-lookup"><span data-stu-id="446c1-293">Request</span></span>

<span data-ttu-id="446c1-294">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="446c1-294">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="446c1-295">HTTP</span><span class="sxs-lookup"><span data-stu-id="446c1-295">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_other_user"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "officeLocation": "city-value"
}
```
# <a name="c"></a>[<span data-ttu-id="446c1-296">C#</span><span class="sxs-lookup"><span data-stu-id="446c1-296">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="446c1-297">JavaScript</span><span class="sxs-lookup"><span data-stu-id="446c1-297">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="446c1-298">Objective-C</span><span class="sxs-lookup"><span data-stu-id="446c1-298">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="446c1-299">Отклик</span><span class="sxs-lookup"><span data-stu-id="446c1-299">Response</span></span>

<span data-ttu-id="446c1-300">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="446c1-300">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="446c1-301">См. также</span><span class="sxs-lookup"><span data-stu-id="446c1-301">See also</span></span>

- [<span data-ttu-id="446c1-302">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="446c1-302">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="446c1-303">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="446c1-303">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="446c1-304">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="446c1-304">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
