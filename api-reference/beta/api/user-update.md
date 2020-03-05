---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 60be070916577de5b4f285c7711b15f37541f96f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451628"
---
# <a name="update-user"></a><span data-ttu-id="cd547-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="cd547-103">Update user</span></span>

<span data-ttu-id="cd547-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cd547-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd547-105">Обновление свойств объекта [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="cd547-105">Update the properties of a [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd547-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd547-106">Permissions</span></span>
<span data-ttu-id="cd547-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd547-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd547-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd547-109">Permission type</span></span>      | <span data-ttu-id="cd547-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd547-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd547-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd547-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cd547-112">User. ReadWrite, User. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cd547-112">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="cd547-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd547-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd547-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd547-114">User.ReadWrite</span></span>    |
|<span data-ttu-id="cd547-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd547-115">Application</span></span> | <span data-ttu-id="cd547-116">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd547-116">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="cd547-117">При обновлении свойства **passwordProfile** необходимо разрешение Directory.AccessAsUser.All.</span><span class="sxs-lookup"><span data-stu-id="cd547-117">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="cd547-118">Обновление свойств **businessPhones**, **mobilePhone** или **otherMails** других пользователей разрешается только для пользователей, не являющихся администраторами, или для пользователей, которым назначена одна из следующих ролей: читатель каталога, приглашающий гостей, читатель Центра сообщений или читатель отчетов.</span><span class="sxs-lookup"><span data-stu-id="cd547-118">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="cd547-119">Дополнительные сведения см. в разделе "Администратор службы поддержки (паролей)" среди [доступных ролей Azure AD](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="cd547-119">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="cd547-120">Это относится к приложениям с предоставленными разрешениями User.ReadWrite.All или Directory.ReadWrite.All (делегированными или для приложений).</span><span class="sxs-lookup"><span data-stu-id="cd547-120">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

>[!NOTE]
><span data-ttu-id="cd547-121">Для обновления свойства " **удостоверения** " требуется разрешение User. Манажеидентитиес. ALL.</span><span class="sxs-lookup"><span data-stu-id="cd547-121">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="cd547-122">Кроме того, добавление [локальной учетной записи B2C](../resources/objectidentity.md) к существующему объекту **пользователя** запрещено, если объект **пользователя** еще не содержит удостоверение локальной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="cd547-122">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="cd547-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd547-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="cd547-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd547-124">Request headers</span></span>
| <span data-ttu-id="cd547-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd547-125">Header</span></span>       | <span data-ttu-id="cd547-126">Значение</span><span class="sxs-lookup"><span data-stu-id="cd547-126">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="cd547-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd547-127">Authorization</span></span>  | <span data-ttu-id="cd547-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd547-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cd547-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd547-130">Content-Type</span></span>  | <span data-ttu-id="cd547-131">application/json</span><span class="sxs-lookup"><span data-stu-id="cd547-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cd547-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd547-132">Request body</span></span>
<span data-ttu-id="cd547-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="cd547-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cd547-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd547-136">Property</span></span>     | <span data-ttu-id="cd547-137">Тип</span><span class="sxs-lookup"><span data-stu-id="cd547-137">Type</span></span>   |<span data-ttu-id="cd547-138">Описание</span><span class="sxs-lookup"><span data-stu-id="cd547-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd547-139">aboutMe</span><span class="sxs-lookup"><span data-stu-id="cd547-139">aboutMe</span></span>|<span data-ttu-id="cd547-140">String</span><span class="sxs-lookup"><span data-stu-id="cd547-140">String</span></span>|<span data-ttu-id="cd547-141">Свободное текстовое поле, где пользователь может рассказать о себе.</span><span class="sxs-lookup"><span data-stu-id="cd547-141">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="cd547-142">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="cd547-142">accountEnabled</span></span>|<span data-ttu-id="cd547-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd547-143">Boolean</span></span>| <span data-ttu-id="cd547-144">Значение **true** указывает, что учетная запись включена. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="cd547-144">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="cd547-145">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-145">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="cd547-146">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="cd547-146">assignedLicenses</span></span>|<span data-ttu-id="cd547-147">Коллекция [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="cd547-147">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="cd547-p107">Лицензии, назначенные пользователю. Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="cd547-p107">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="cd547-150">birthday</span><span class="sxs-lookup"><span data-stu-id="cd547-150">birthday</span></span>|<span data-ttu-id="cd547-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd547-151">DateTimeOffset</span></span>|<span data-ttu-id="cd547-p108">День рождения пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cd547-p108">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="cd547-155">businessPhones</span><span class="sxs-lookup"><span data-stu-id="cd547-155">businessPhones</span></span>| <span data-ttu-id="cd547-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cd547-156">String collection</span></span> | <span data-ttu-id="cd547-p109">Номера телефонов пользователя. ПРИМЕЧАНИЕ. Несмотря на то что это коллекция строк, в качестве этого свойства можно указать только одно число.</span><span class="sxs-lookup"><span data-stu-id="cd547-p109">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="cd547-159">city</span><span class="sxs-lookup"><span data-stu-id="cd547-159">city</span></span>|<span data-ttu-id="cd547-160">String</span><span class="sxs-lookup"><span data-stu-id="cd547-160">String</span></span>|<span data-ttu-id="cd547-161">Город, в котором находится пользователь.</span><span class="sxs-lookup"><span data-stu-id="cd547-161">The city in which the user is located.</span></span>|
|<span data-ttu-id="cd547-162">country</span><span class="sxs-lookup"><span data-stu-id="cd547-162">country</span></span>|<span data-ttu-id="cd547-163">Строка</span><span class="sxs-lookup"><span data-stu-id="cd547-163">String</span></span>|<span data-ttu-id="cd547-164">Страна или регион, в котором находится пользователь, например "США" или "Соединенное Королевство".</span><span class="sxs-lookup"><span data-stu-id="cd547-164">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="cd547-165">department</span><span class="sxs-lookup"><span data-stu-id="cd547-165">department</span></span>|<span data-ttu-id="cd547-166">String</span><span class="sxs-lookup"><span data-stu-id="cd547-166">String</span></span>|<span data-ttu-id="cd547-167">Название отдела, в котором работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="cd547-167">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="cd547-168">displayName</span><span class="sxs-lookup"><span data-stu-id="cd547-168">displayName</span></span>|<span data-ttu-id="cd547-169">String</span><span class="sxs-lookup"><span data-stu-id="cd547-169">String</span></span>|<span data-ttu-id="cd547-p110">Отображаемое имя пользователя в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="cd547-p110">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="cd547-174">employeeId</span><span class="sxs-lookup"><span data-stu-id="cd547-174">employeeId</span></span>|<span data-ttu-id="cd547-175">String</span><span class="sxs-lookup"><span data-stu-id="cd547-175">String</span></span>|<span data-ttu-id="cd547-176">Идентификатор сотрудника, назначенный пользователю организацией.</span><span class="sxs-lookup"><span data-stu-id="cd547-176">The employee identifier assigned to the user by the organization.</span></span>|
|<span data-ttu-id="cd547-177">givenName</span><span class="sxs-lookup"><span data-stu-id="cd547-177">givenName</span></span>|<span data-ttu-id="cd547-178">String</span><span class="sxs-lookup"><span data-stu-id="cd547-178">String</span></span>|<span data-ttu-id="cd547-179">Простое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-179">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="cd547-180">hireDate</span><span class="sxs-lookup"><span data-stu-id="cd547-180">hireDate</span></span>|<span data-ttu-id="cd547-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd547-181">DateTimeOffset</span></span>|<span data-ttu-id="cd547-p111">Дата найма пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cd547-p111">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="cd547-185">identities</span><span class="sxs-lookup"><span data-stu-id="cd547-185">identities</span></span>|<span data-ttu-id="cd547-186">Коллекция [objectIdentity](../resources/objectidentity.md)</span><span class="sxs-lookup"><span data-stu-id="cd547-186">[objectIdentity](../resources/objectidentity.md) collection</span></span>| <span data-ttu-id="cd547-187">Представляет удостоверения, которые можно использовать для входа в учетную запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-187">Represents the identities that can be used to sign in to this user account.</span></span> <span data-ttu-id="cd547-188">Удостоверение может предоставляться корпорацией Майкрософт, организациями или поставщиками удостоверений социальных сетей, такими как Facebook, Google и Майкрософт, и привязывается к учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-188">An identity can be provided by Microsoft, by organizations, or by social identity providers such as Facebook, Google, and Microsoft, and tied to a user account.</span></span> <span data-ttu-id="cd547-189">Все обновления для **удостоверений** заменят всю коллекцию, и необходимо указать идентификатор userPrincipalName **сигнинтипе** в коллекции.</span><span class="sxs-lookup"><span data-stu-id="cd547-189">Any update to **identities** will replace the entire collection and you must supply the userPrincipalName **signInType** identity in the collection.</span></span>|
|<span data-ttu-id="cd547-190">interests;</span><span class="sxs-lookup"><span data-stu-id="cd547-190">interests</span></span>|<span data-ttu-id="cd547-191">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cd547-191">String collection</span></span>|<span data-ttu-id="cd547-192">Список интересов пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-192">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="cd547-193">jobTitle</span><span class="sxs-lookup"><span data-stu-id="cd547-193">jobTitle</span></span>|<span data-ttu-id="cd547-194">String</span><span class="sxs-lookup"><span data-stu-id="cd547-194">String</span></span>|<span data-ttu-id="cd547-195">Должность пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-195">The user’s job title.</span></span>|
|<span data-ttu-id="cd547-196">mailNickname</span><span class="sxs-lookup"><span data-stu-id="cd547-196">mailNickname</span></span>|<span data-ttu-id="cd547-197">String</span><span class="sxs-lookup"><span data-stu-id="cd547-197">String</span></span>|<span data-ttu-id="cd547-198">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-198">The mail alias for the user.</span></span> <span data-ttu-id="cd547-199">Это свойство должно быть указано при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-199">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="cd547-200">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="cd547-200">mobilePhone</span></span>|<span data-ttu-id="cd547-201">String</span><span class="sxs-lookup"><span data-stu-id="cd547-201">String</span></span>|<span data-ttu-id="cd547-202">Основной сотовый телефон пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-202">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="cd547-203">mySite</span><span class="sxs-lookup"><span data-stu-id="cd547-203">mySite</span></span>|<span data-ttu-id="cd547-204">String</span><span class="sxs-lookup"><span data-stu-id="cd547-204">String</span></span>|<span data-ttu-id="cd547-205">URL-адрес личного сайта пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-205">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="cd547-206">officeLocation</span><span class="sxs-lookup"><span data-stu-id="cd547-206">officeLocation</span></span>|<span data-ttu-id="cd547-207">String</span><span class="sxs-lookup"><span data-stu-id="cd547-207">String</span></span>|<span data-ttu-id="cd547-208">Расположение офиса на месте работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-208">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="cd547-209">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="cd547-209">onPremisesImmutableId</span></span>|<span data-ttu-id="cd547-210">String</span><span class="sxs-lookup"><span data-stu-id="cd547-210">String</span></span>|<span data-ttu-id="cd547-211">Это свойство используется для сопоставления локальной учетной записи Active Directory с объектом пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cd547-211">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="cd547-212">Его необходимо указывать при создании учетной записи пользователя в Graph, если в качестве свойства **userPrincipalName** (имени участника-пользователя) используется федеративный домен.</span><span class="sxs-lookup"><span data-stu-id="cd547-212">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="cd547-213">**Важно!** В этом свойстве не допускается использование символов **$** и **_**.</span><span class="sxs-lookup"><span data-stu-id="cd547-213">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="cd547-214">otherMails</span><span class="sxs-lookup"><span data-stu-id="cd547-214">otherMails</span></span>|<span data-ttu-id="cd547-215">String</span><span class="sxs-lookup"><span data-stu-id="cd547-215">String</span></span> |<span data-ttu-id="cd547-216">Список дополнительных адресов электронной почты для пользователя. Например: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="cd547-216">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="cd547-217">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="cd547-217">passwordPolicies</span></span>|<span data-ttu-id="cd547-218">String</span><span class="sxs-lookup"><span data-stu-id="cd547-218">String</span></span>|<span data-ttu-id="cd547-p115">Задает политики паролей для пользователя. Это свойство представляет собой перечисление с единственным возможным значением — "DisableStrongPassword". Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение "DisablePasswordExpiration". Эти значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="cd547-p115">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="cd547-223">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="cd547-223">passwordProfile</span></span>|[<span data-ttu-id="cd547-224">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="cd547-224">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="cd547-p116">Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="cd547-p116">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="cd547-230">pastProjects</span><span class="sxs-lookup"><span data-stu-id="cd547-230">pastProjects</span></span>|<span data-ttu-id="cd547-231">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cd547-231">String collection</span></span>|<span data-ttu-id="cd547-232">Список предыдущих проектов пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-232">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="cd547-233">postalCode</span><span class="sxs-lookup"><span data-stu-id="cd547-233">postalCode</span></span>|<span data-ttu-id="cd547-234">String</span><span class="sxs-lookup"><span data-stu-id="cd547-234">String</span></span>|<span data-ttu-id="cd547-p117">Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код.</span><span class="sxs-lookup"><span data-stu-id="cd547-p117">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="cd547-238">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="cd547-238">preferredLanguage</span></span>|<span data-ttu-id="cd547-239">String</span><span class="sxs-lookup"><span data-stu-id="cd547-239">String</span></span>|<span data-ttu-id="cd547-p118">Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1, например "ru-RU".</span><span class="sxs-lookup"><span data-stu-id="cd547-p118">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="cd547-242">responsibilities</span><span class="sxs-lookup"><span data-stu-id="cd547-242">responsibilities</span></span>|<span data-ttu-id="cd547-243">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cd547-243">String collection</span></span>|<span data-ttu-id="cd547-244">Список обязанностей пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-244">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="cd547-245">schools</span><span class="sxs-lookup"><span data-stu-id="cd547-245">schools</span></span>|<span data-ttu-id="cd547-246">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cd547-246">String collection</span></span>|<span data-ttu-id="cd547-247">Список учебных заведений, которые посещал пользователь.</span><span class="sxs-lookup"><span data-stu-id="cd547-247">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="cd547-248">skills</span><span class="sxs-lookup"><span data-stu-id="cd547-248">skills</span></span>|<span data-ttu-id="cd547-249">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cd547-249">String collection</span></span>|<span data-ttu-id="cd547-250">Список навыков пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-250">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="cd547-251">state</span><span class="sxs-lookup"><span data-stu-id="cd547-251">state</span></span>|<span data-ttu-id="cd547-252">Строка</span><span class="sxs-lookup"><span data-stu-id="cd547-252">String</span></span>|<span data-ttu-id="cd547-253">Область, республика, край или округ в адресе пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-253">The state or province in the user's address.</span></span>|
|<span data-ttu-id="cd547-254">streetAddress</span><span class="sxs-lookup"><span data-stu-id="cd547-254">streetAddress</span></span>|<span data-ttu-id="cd547-255">String</span><span class="sxs-lookup"><span data-stu-id="cd547-255">String</span></span>|<span data-ttu-id="cd547-256">Почтовый адрес места работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-256">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="cd547-257">surname</span><span class="sxs-lookup"><span data-stu-id="cd547-257">surname</span></span>|<span data-ttu-id="cd547-258">String</span><span class="sxs-lookup"><span data-stu-id="cd547-258">String</span></span>|<span data-ttu-id="cd547-259">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd547-259">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="cd547-260">usageLocation</span><span class="sxs-lookup"><span data-stu-id="cd547-260">usageLocation</span></span>|<span data-ttu-id="cd547-261">String</span><span class="sxs-lookup"><span data-stu-id="cd547-261">String</span></span>|<span data-ttu-id="cd547-262">Двухбуквенный код страны (по стандарту ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="cd547-262">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="cd547-263">Необходим для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в разных странах.</span><span class="sxs-lookup"><span data-stu-id="cd547-263">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="cd547-264">Примеры: "RU", "JP", "GB".</span><span class="sxs-lookup"><span data-stu-id="cd547-264">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="cd547-265">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="cd547-265">Not nullable.</span></span>|
|<span data-ttu-id="cd547-266">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cd547-266">userPrincipalName</span></span>|<span data-ttu-id="cd547-267">String</span><span class="sxs-lookup"><span data-stu-id="cd547-267">String</span></span>|<span data-ttu-id="cd547-p120">Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](../resources/organization.md). Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="cd547-p120">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="cd547-275">userType</span><span class="sxs-lookup"><span data-stu-id="cd547-275">userType</span></span>|<span data-ttu-id="cd547-276">String</span><span class="sxs-lookup"><span data-stu-id="cd547-276">String</span></span>|<span data-ttu-id="cd547-277">Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость".</span><span class="sxs-lookup"><span data-stu-id="cd547-277">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

<span data-ttu-id="cd547-278">Так как ресурс **User** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в пользовательских свойствах расширения в существующем **пользовательском** экземпляре.</span><span class="sxs-lookup"><span data-stu-id="cd547-278">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **user** instance.</span></span>

## <a name="response"></a><span data-ttu-id="cd547-279">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd547-279">Response</span></span>

<span data-ttu-id="cd547-280">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cd547-280">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cd547-281">Пример</span><span class="sxs-lookup"><span data-stu-id="cd547-281">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="cd547-282">Пример 1. Обновление свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="cd547-282">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="cd547-283">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd547-283">Request</span></span>

<span data-ttu-id="cd547-284">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd547-284">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cd547-285">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd547-285">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cd547-286">C#</span><span class="sxs-lookup"><span data-stu-id="cd547-286">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd547-287">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd547-287">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd547-288">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd547-288">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cd547-289">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd547-289">Response</span></span>

<span data-ttu-id="cd547-290">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cd547-290">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="cd547-291">Пример 2. Обновление свойств указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="cd547-291">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="cd547-292">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd547-292">Request</span></span>

<span data-ttu-id="cd547-293">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd547-293">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cd547-294">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd547-294">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cd547-295">C#</span><span class="sxs-lookup"><span data-stu-id="cd547-295">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd547-296">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd547-296">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd547-297">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd547-297">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cd547-298">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd547-298">Response</span></span>

<span data-ttu-id="cd547-299">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cd547-299">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="cd547-300">См. также</span><span class="sxs-lookup"><span data-stu-id="cd547-300">See also</span></span>

- [<span data-ttu-id="cd547-301">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="cd547-301">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="cd547-302">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="cd547-302">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="cd547-303">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="cd547-303">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
