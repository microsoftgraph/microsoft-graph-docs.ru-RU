---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 79f6ec2c72271319548750a4637aff28dfbd7f02
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421780"
---
# <a name="update-user"></a><span data-ttu-id="e64ff-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="e64ff-103">Update user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e64ff-104">Обновление свойств объекта [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="e64ff-104">Update the properties of a [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e64ff-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e64ff-105">Permissions</span></span>
<span data-ttu-id="e64ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e64ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e64ff-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e64ff-108">Permission type</span></span>      | <span data-ttu-id="e64ff-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e64ff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e64ff-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e64ff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e64ff-111">User. ReadWrite, User. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e64ff-111">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="e64ff-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e64ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e64ff-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e64ff-113">User.ReadWrite</span></span>    |
|<span data-ttu-id="e64ff-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e64ff-114">Application</span></span> | <span data-ttu-id="e64ff-115">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e64ff-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="e64ff-116">При обновлении свойства **passwordprofile необходима** необходимо следующее разрешение: Directory. AccessAsUser. ALL.</span><span class="sxs-lookup"><span data-stu-id="e64ff-116">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="e64ff-117">Обновление свойства **businessPhones**, **mobilePhone**или **осермаилс** другого пользователя разрешено только для пользователей, не являющихся администраторами или назначенных одной из следующих ролей: читатели каталогов, гость приглашений, средство чтения центра сообщений и Средство чтения отчетов.</span><span class="sxs-lookup"><span data-stu-id="e64ff-117">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="e64ff-118">Для получения дополнительных сведений обратитесь к администратору службы поддержки (пароль) в [доступных ролях Azure AD](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="e64ff-118">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="e64ff-119">В этом случае приложениям, которым предоставлены разрешения User. ReadWrite. ALL или Directory. ReadWrite. ALL, или Applications. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="e64ff-119">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>


## <a name="http-request"></a><span data-ttu-id="e64ff-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e64ff-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="e64ff-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e64ff-121">Request headers</span></span>
| <span data-ttu-id="e64ff-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e64ff-122">Header</span></span>       | <span data-ttu-id="e64ff-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e64ff-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="e64ff-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e64ff-124">Authorization</span></span>  | <span data-ttu-id="e64ff-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e64ff-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e64ff-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e64ff-127">Content-Type</span></span>  | <span data-ttu-id="e64ff-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e64ff-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e64ff-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e64ff-129">Request body</span></span>
<span data-ttu-id="e64ff-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e64ff-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e64ff-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="e64ff-133">Property</span></span>     | <span data-ttu-id="e64ff-134">Тип</span><span class="sxs-lookup"><span data-stu-id="e64ff-134">Type</span></span>   |<span data-ttu-id="e64ff-135">Описание</span><span class="sxs-lookup"><span data-stu-id="e64ff-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e64ff-136">aboutMe</span><span class="sxs-lookup"><span data-stu-id="e64ff-136">aboutMe</span></span>|<span data-ttu-id="e64ff-137">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-137">String</span></span>|<span data-ttu-id="e64ff-138">Свободное текстовое поле, где пользователь может рассказать о себе.</span><span class="sxs-lookup"><span data-stu-id="e64ff-138">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="e64ff-139">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="e64ff-139">accountEnabled</span></span>|<span data-ttu-id="e64ff-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="e64ff-140">Boolean</span></span>| <span data-ttu-id="e64ff-141">Если учетная запись обеспечена — значение **true**, в противном случае — **false**.</span><span class="sxs-lookup"><span data-stu-id="e64ff-141">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="e64ff-142">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="e64ff-142">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="e64ff-143">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="e64ff-143">assignedLicenses</span></span>|<span data-ttu-id="e64ff-144">Коллекция [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e64ff-144">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="e64ff-p106">Лицензии, назначенные пользователю. Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="e64ff-p106">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="e64ff-147">birthday</span><span class="sxs-lookup"><span data-stu-id="e64ff-147">birthday</span></span>|<span data-ttu-id="e64ff-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e64ff-148">DateTimeOffset</span></span>|<span data-ttu-id="e64ff-p107">День рождения пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e64ff-p107">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e64ff-152">businessPhones</span><span class="sxs-lookup"><span data-stu-id="e64ff-152">businessPhones</span></span>| <span data-ttu-id="e64ff-153">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e64ff-153">String collection</span></span> | <span data-ttu-id="e64ff-p108">Номера телефонов пользователя. ПРИМЕЧАНИЕ. Несмотря на то что это коллекция строк, в качестве этого свойства можно указать только одно число.</span><span class="sxs-lookup"><span data-stu-id="e64ff-p108">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="e64ff-156">city</span><span class="sxs-lookup"><span data-stu-id="e64ff-156">city</span></span>|<span data-ttu-id="e64ff-157">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-157">String</span></span>|<span data-ttu-id="e64ff-158">Город, в котором находится пользователь.</span><span class="sxs-lookup"><span data-stu-id="e64ff-158">The city in which the user is located.</span></span>|
|<span data-ttu-id="e64ff-159">country</span><span class="sxs-lookup"><span data-stu-id="e64ff-159">country</span></span>|<span data-ttu-id="e64ff-160">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-160">String</span></span>|<span data-ttu-id="e64ff-161">Страна или регион, в котором находится пользователь, например "США" или "Соединенное Королевство".</span><span class="sxs-lookup"><span data-stu-id="e64ff-161">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="e64ff-162">department</span><span class="sxs-lookup"><span data-stu-id="e64ff-162">department</span></span>|<span data-ttu-id="e64ff-163">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-163">String</span></span>|<span data-ttu-id="e64ff-164">Название отдела, в котором работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="e64ff-164">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="e64ff-165">displayName</span><span class="sxs-lookup"><span data-stu-id="e64ff-165">displayName</span></span>|<span data-ttu-id="e64ff-166">Строка</span><span class="sxs-lookup"><span data-stu-id="e64ff-166">String</span></span>|<span data-ttu-id="e64ff-p109">Отображаемое имя пользователя в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="e64ff-p109">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="e64ff-171">employeeId</span><span class="sxs-lookup"><span data-stu-id="e64ff-171">employeeId</span></span>|<span data-ttu-id="e64ff-172">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-172">String</span></span>|<span data-ttu-id="e64ff-173">Идентификатор сотрудника, назначенный пользователю организацией.</span><span class="sxs-lookup"><span data-stu-id="e64ff-173">The employee identifier assigned to the user by the organization.</span></span>|
|<span data-ttu-id="e64ff-174">givenName</span><span class="sxs-lookup"><span data-stu-id="e64ff-174">givenName</span></span>|<span data-ttu-id="e64ff-175">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-175">String</span></span>|<span data-ttu-id="e64ff-176">Простое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="e64ff-176">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="e64ff-177">hireDate</span><span class="sxs-lookup"><span data-stu-id="e64ff-177">hireDate</span></span>|<span data-ttu-id="e64ff-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e64ff-178">DateTimeOffset</span></span>|<span data-ttu-id="e64ff-p110">Дата найма пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e64ff-p110">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e64ff-182">interests</span><span class="sxs-lookup"><span data-stu-id="e64ff-182">interests</span></span>|<span data-ttu-id="e64ff-183">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e64ff-183">String collection</span></span>|<span data-ttu-id="e64ff-184">Список интересов пользователя.</span><span class="sxs-lookup"><span data-stu-id="e64ff-184">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="e64ff-185">jobTitle</span><span class="sxs-lookup"><span data-stu-id="e64ff-185">jobTitle</span></span>|<span data-ttu-id="e64ff-186">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-186">String</span></span>|<span data-ttu-id="e64ff-187">Должность пользователя.</span><span class="sxs-lookup"><span data-stu-id="e64ff-187">The user’s job title.</span></span>|
|<span data-ttu-id="e64ff-188">mailNickname</span><span class="sxs-lookup"><span data-stu-id="e64ff-188">mailNickname</span></span>|<span data-ttu-id="e64ff-189">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-189">String</span></span>|<span data-ttu-id="e64ff-190">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e64ff-190">The mail alias for the user.</span></span> <span data-ttu-id="e64ff-191">Это свойство должно быть указано при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="e64ff-191">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="e64ff-192">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="e64ff-192">mobilePhone</span></span>|<span data-ttu-id="e64ff-193">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-193">String</span></span>|<span data-ttu-id="e64ff-194">Основной сотовый телефон пользователя.</span><span class="sxs-lookup"><span data-stu-id="e64ff-194">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="e64ff-195">mySite</span><span class="sxs-lookup"><span data-stu-id="e64ff-195">mySite</span></span>|<span data-ttu-id="e64ff-196">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-196">String</span></span>|<span data-ttu-id="e64ff-197">URL-адрес личного сайта пользователя.</span><span class="sxs-lookup"><span data-stu-id="e64ff-197">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="e64ff-198">officeLocation</span><span class="sxs-lookup"><span data-stu-id="e64ff-198">officeLocation</span></span>|<span data-ttu-id="e64ff-199">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-199">String</span></span>|<span data-ttu-id="e64ff-200">Расположение офиса на месте работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="e64ff-200">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="e64ff-201">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="e64ff-201">onPremisesImmutableId</span></span>|<span data-ttu-id="e64ff-202">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-202">String</span></span>|<span data-ttu-id="e64ff-203">Это свойство используется для сопоставления локальной учетной записи Active Directory с объектом пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e64ff-203">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="e64ff-204">Его необходимо указывать при создании учетной записи пользователя в Graph, если в качестве свойства **userPrincipalName** (имени участника-пользователя) используется федеративный домен.</span><span class="sxs-lookup"><span data-stu-id="e64ff-204">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="e64ff-205">**Важно!** В этом свойстве не допускается использование символов **$** и **_**.</span><span class="sxs-lookup"><span data-stu-id="e64ff-205">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="e64ff-206">otherMails</span><span class="sxs-lookup"><span data-stu-id="e64ff-206">otherMails</span></span>|<span data-ttu-id="e64ff-207">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-207">String</span></span> |<span data-ttu-id="e64ff-208">Список дополнительных адресов электронной почты для пользователя. Например: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="e64ff-208">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="e64ff-209">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="e64ff-209">passwordPolicies</span></span>|<span data-ttu-id="e64ff-210">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-210">String</span></span>|<span data-ttu-id="e64ff-p113">Задает политики паролей для пользователя. Это свойство представляет собой перечисление с единственным возможным значением — "DisableStrongPassword". Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение "DisablePasswordExpiration". Эти значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="e64ff-p113">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="e64ff-215">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="e64ff-215">passwordProfile</span></span>|[<span data-ttu-id="e64ff-216">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="e64ff-216">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="e64ff-p114">Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="e64ff-p114">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="e64ff-222">pastProjects</span><span class="sxs-lookup"><span data-stu-id="e64ff-222">pastProjects</span></span>|<span data-ttu-id="e64ff-223">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e64ff-223">String collection</span></span>|<span data-ttu-id="e64ff-224">Список предыдущих проектов пользователя.</span><span class="sxs-lookup"><span data-stu-id="e64ff-224">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="e64ff-225">postalCode</span><span class="sxs-lookup"><span data-stu-id="e64ff-225">postalCode</span></span>|<span data-ttu-id="e64ff-226">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-226">String</span></span>|<span data-ttu-id="e64ff-p115">Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код.</span><span class="sxs-lookup"><span data-stu-id="e64ff-p115">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="e64ff-230">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="e64ff-230">preferredLanguage</span></span>|<span data-ttu-id="e64ff-231">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-231">String</span></span>|<span data-ttu-id="e64ff-p116">Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1, например "ru-RU".</span><span class="sxs-lookup"><span data-stu-id="e64ff-p116">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="e64ff-234">responsibilities</span><span class="sxs-lookup"><span data-stu-id="e64ff-234">responsibilities</span></span>|<span data-ttu-id="e64ff-235">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e64ff-235">String collection</span></span>|<span data-ttu-id="e64ff-236">Список обязанностей пользователя.</span><span class="sxs-lookup"><span data-stu-id="e64ff-236">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="e64ff-237">schools</span><span class="sxs-lookup"><span data-stu-id="e64ff-237">schools</span></span>|<span data-ttu-id="e64ff-238">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e64ff-238">String collection</span></span>|<span data-ttu-id="e64ff-239">Список учебных заведений, которые посещал пользователь.</span><span class="sxs-lookup"><span data-stu-id="e64ff-239">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="e64ff-240">skills</span><span class="sxs-lookup"><span data-stu-id="e64ff-240">skills</span></span>|<span data-ttu-id="e64ff-241">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e64ff-241">String collection</span></span>|<span data-ttu-id="e64ff-242">Список навыков пользователя.</span><span class="sxs-lookup"><span data-stu-id="e64ff-242">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="e64ff-243">state</span><span class="sxs-lookup"><span data-stu-id="e64ff-243">state</span></span>|<span data-ttu-id="e64ff-244">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-244">String</span></span>|<span data-ttu-id="e64ff-245">Область, республика, край или округ в адресе пользователя.</span><span class="sxs-lookup"><span data-stu-id="e64ff-245">The state or province in the user's address.</span></span>|
|<span data-ttu-id="e64ff-246">streetAddress</span><span class="sxs-lookup"><span data-stu-id="e64ff-246">streetAddress</span></span>|<span data-ttu-id="e64ff-247">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-247">String</span></span>|<span data-ttu-id="e64ff-248">Почтовый адрес места работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="e64ff-248">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="e64ff-249">surname</span><span class="sxs-lookup"><span data-stu-id="e64ff-249">surname</span></span>|<span data-ttu-id="e64ff-250">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-250">String</span></span>|<span data-ttu-id="e64ff-251">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="e64ff-251">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="e64ff-252">usageLocation</span><span class="sxs-lookup"><span data-stu-id="e64ff-252">usageLocation</span></span>|<span data-ttu-id="e64ff-253">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-253">String</span></span>|<span data-ttu-id="e64ff-254">Двухбуквенный код страны (по стандарту ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="e64ff-254">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="e64ff-255">Необходим для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в разных странах.</span><span class="sxs-lookup"><span data-stu-id="e64ff-255">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="e64ff-256">Примеры: "RU", "JP" и "GB".</span><span class="sxs-lookup"><span data-stu-id="e64ff-256">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="e64ff-257">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="e64ff-257">Not nullable.</span></span>|
|<span data-ttu-id="e64ff-258">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e64ff-258">userPrincipalName</span></span>|<span data-ttu-id="e64ff-259">Строка</span><span class="sxs-lookup"><span data-stu-id="e64ff-259">String</span></span>|<span data-ttu-id="e64ff-p118">Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](../resources/organization.md). Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="e64ff-p118">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="e64ff-267">userType</span><span class="sxs-lookup"><span data-stu-id="e64ff-267">userType</span></span>|<span data-ttu-id="e64ff-268">String</span><span class="sxs-lookup"><span data-stu-id="e64ff-268">String</span></span>|<span data-ttu-id="e64ff-269">Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость".</span><span class="sxs-lookup"><span data-stu-id="e64ff-269">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

<span data-ttu-id="e64ff-270">Так как ресурс **User** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в пользовательских свойствах расширения в существующем **пользовательском** экземпляре.</span><span class="sxs-lookup"><span data-stu-id="e64ff-270">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **user** instance.</span></span>

## <a name="response"></a><span data-ttu-id="e64ff-271">Отклик</span><span class="sxs-lookup"><span data-stu-id="e64ff-271">Response</span></span>

<span data-ttu-id="e64ff-272">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e64ff-272">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e64ff-273">Пример</span><span class="sxs-lookup"><span data-stu-id="e64ff-273">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="e64ff-274">Пример 1: обновление свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="e64ff-274">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="e64ff-275">Запрос</span><span class="sxs-lookup"><span data-stu-id="e64ff-275">Request</span></span>

<span data-ttu-id="e64ff-276">В приведенном ниже примере показан запрос.</span><span class="sxs-lookup"><span data-stu-id="e64ff-276">The following example shows a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e64ff-277">HTTP</span><span class="sxs-lookup"><span data-stu-id="e64ff-277">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e64ff-278">C#</span><span class="sxs-lookup"><span data-stu-id="e64ff-278">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e64ff-279">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e64ff-279">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e64ff-280">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e64ff-280">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e64ff-281">Ответ</span><span class="sxs-lookup"><span data-stu-id="e64ff-281">Response</span></span>

<span data-ttu-id="e64ff-282">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e64ff-282">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="e64ff-283">Пример 2: обновление свойств указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="e64ff-283">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="e64ff-284">Запрос</span><span class="sxs-lookup"><span data-stu-id="e64ff-284">Request</span></span>

<span data-ttu-id="e64ff-285">В приведенном ниже примере показан запрос.</span><span class="sxs-lookup"><span data-stu-id="e64ff-285">The following example shows a request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e64ff-286">HTTP</span><span class="sxs-lookup"><span data-stu-id="e64ff-286">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e64ff-287">C#</span><span class="sxs-lookup"><span data-stu-id="e64ff-287">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e64ff-288">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e64ff-288">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e64ff-289">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e64ff-289">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e64ff-290">Ответ</span><span class="sxs-lookup"><span data-stu-id="e64ff-290">Response</span></span>

<span data-ttu-id="e64ff-291">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e64ff-291">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="e64ff-292">См. также</span><span class="sxs-lookup"><span data-stu-id="e64ff-292">See also</span></span>

- [<span data-ttu-id="e64ff-293">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="e64ff-293">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e64ff-294">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e64ff-294">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="e64ff-295">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e64ff-295">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
