---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 8be20928a35865202c98a3df9c3b75360a32d530
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720020"
---
# <a name="update-user"></a><span data-ttu-id="23f66-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="23f66-103">Update user</span></span>

<span data-ttu-id="23f66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23f66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23f66-105">Обновление свойств объекта [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="23f66-105">Update the properties of a [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="23f66-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23f66-106">Permissions</span></span>
<span data-ttu-id="23f66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23f66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23f66-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23f66-109">Permission type</span></span>      | <span data-ttu-id="23f66-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23f66-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23f66-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23f66-111">Delegated (work or school account)</span></span> | <span data-ttu-id="23f66-112">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23f66-112">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="23f66-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23f66-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23f66-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23f66-114">User.ReadWrite</span></span>    |
|<span data-ttu-id="23f66-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23f66-115">Application</span></span> | <span data-ttu-id="23f66-116">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23f66-116">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="23f66-117">При обновлении свойства **passwordProfile** необходимо разрешение Directory.AccessAsUser.All.</span><span class="sxs-lookup"><span data-stu-id="23f66-117">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="23f66-118">Обновление свойств **businessPhones**, **mobilePhone** или **otherMails** других пользователей разрешается только для пользователей, не являющихся администраторами, или для пользователей, которым назначена одна из следующих ролей: читатель каталога, приглашающий гостей, читатель Центра сообщений или читатель отчетов.</span><span class="sxs-lookup"><span data-stu-id="23f66-118">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="23f66-119">Дополнительные сведения см. в разделе "Администратор службы поддержки (паролей)" среди [доступных ролей Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="23f66-119">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="23f66-120">Это относится к приложениям с предоставленными разрешениями User.ReadWrite.All или Directory.ReadWrite.All (делегированными или для приложений).</span><span class="sxs-lookup"><span data-stu-id="23f66-120">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

>[!NOTE]
><span data-ttu-id="23f66-121">Обновление свойства **личностей** требует разрешения User.ManageIdentities.All.</span><span class="sxs-lookup"><span data-stu-id="23f66-121">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="23f66-122">Кроме того, добавление [локальной учетной записи B2C](../resources/objectidentity.md) к существующему объекту **пользователя** не допускается, если только объект **пользователя** не содержит идентификатор локальной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="23f66-122">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="23f66-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23f66-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="23f66-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23f66-124">Request headers</span></span>
| <span data-ttu-id="23f66-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23f66-125">Header</span></span>       | <span data-ttu-id="23f66-126">Значение</span><span class="sxs-lookup"><span data-stu-id="23f66-126">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="23f66-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23f66-127">Authorization</span></span>  | <span data-ttu-id="23f66-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23f66-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="23f66-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="23f66-130">Content-Type</span></span>  | <span data-ttu-id="23f66-131">application/json</span><span class="sxs-lookup"><span data-stu-id="23f66-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="23f66-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23f66-132">Request body</span></span>
<span data-ttu-id="23f66-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="23f66-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="23f66-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="23f66-136">Property</span></span>     | <span data-ttu-id="23f66-137">Тип</span><span class="sxs-lookup"><span data-stu-id="23f66-137">Type</span></span>   |<span data-ttu-id="23f66-138">Описание</span><span class="sxs-lookup"><span data-stu-id="23f66-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23f66-139">aboutMe</span><span class="sxs-lookup"><span data-stu-id="23f66-139">aboutMe</span></span>|<span data-ttu-id="23f66-140">String</span><span class="sxs-lookup"><span data-stu-id="23f66-140">String</span></span>|<span data-ttu-id="23f66-141">Свободное текстовое поле, где пользователь может рассказать о себе.</span><span class="sxs-lookup"><span data-stu-id="23f66-141">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="23f66-142">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="23f66-142">accountEnabled</span></span>|<span data-ttu-id="23f66-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="23f66-143">Boolean</span></span>| <span data-ttu-id="23f66-144">Значение **true** указывает, что учетная запись включена. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="23f66-144">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="23f66-145">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-145">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="23f66-146">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="23f66-146">assignedLicenses</span></span>|<span data-ttu-id="23f66-147">Коллекция [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="23f66-147">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="23f66-p107">Лицензии, назначенные пользователю. Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="23f66-p107">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="23f66-150">birthday</span><span class="sxs-lookup"><span data-stu-id="23f66-150">birthday</span></span>|<span data-ttu-id="23f66-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23f66-151">DateTimeOffset</span></span>|<span data-ttu-id="23f66-152">День рождения пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-152">The birthday of the user.</span></span> <span data-ttu-id="23f66-153">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="23f66-153">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="23f66-154">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="23f66-154">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="23f66-155">businessPhones</span><span class="sxs-lookup"><span data-stu-id="23f66-155">businessPhones</span></span>| <span data-ttu-id="23f66-156">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="23f66-156">String collection</span></span> | <span data-ttu-id="23f66-p109">Номера телефонов пользователя. ПРИМЕЧАНИЕ. Несмотря на то что это коллекция строк, в качестве этого свойства можно указать только одно число.</span><span class="sxs-lookup"><span data-stu-id="23f66-p109">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="23f66-159">city</span><span class="sxs-lookup"><span data-stu-id="23f66-159">city</span></span>|<span data-ttu-id="23f66-160">String</span><span class="sxs-lookup"><span data-stu-id="23f66-160">String</span></span>|<span data-ttu-id="23f66-161">Город, в котором находится пользователь.</span><span class="sxs-lookup"><span data-stu-id="23f66-161">The city in which the user is located.</span></span>|
|<span data-ttu-id="23f66-162">country</span><span class="sxs-lookup"><span data-stu-id="23f66-162">country</span></span>|<span data-ttu-id="23f66-163">String</span><span class="sxs-lookup"><span data-stu-id="23f66-163">String</span></span>|<span data-ttu-id="23f66-164">Страна или регион, в котором находится пользователь, например "США" или "Соединенное Королевство".</span><span class="sxs-lookup"><span data-stu-id="23f66-164">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="23f66-165">department</span><span class="sxs-lookup"><span data-stu-id="23f66-165">department</span></span>|<span data-ttu-id="23f66-166">String</span><span class="sxs-lookup"><span data-stu-id="23f66-166">String</span></span>|<span data-ttu-id="23f66-167">Название отдела, в котором работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="23f66-167">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="23f66-168">displayName</span><span class="sxs-lookup"><span data-stu-id="23f66-168">displayName</span></span>|<span data-ttu-id="23f66-169">String</span><span class="sxs-lookup"><span data-stu-id="23f66-169">String</span></span>|<span data-ttu-id="23f66-p110">Отображаемое имя пользователя в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="23f66-p110">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="23f66-174">employeeId</span><span class="sxs-lookup"><span data-stu-id="23f66-174">employeeId</span></span>|<span data-ttu-id="23f66-175">String</span><span class="sxs-lookup"><span data-stu-id="23f66-175">String</span></span>|<span data-ttu-id="23f66-176">Идентификатор сотрудника, назначенный пользователю организацией.</span><span class="sxs-lookup"><span data-stu-id="23f66-176">The employee identifier assigned to the user by the organization.</span></span>|
|<span data-ttu-id="23f66-177">givenName;</span><span class="sxs-lookup"><span data-stu-id="23f66-177">givenName</span></span>|<span data-ttu-id="23f66-178">String</span><span class="sxs-lookup"><span data-stu-id="23f66-178">String</span></span>|<span data-ttu-id="23f66-179">Простое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-179">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="23f66-180">hireDate</span><span class="sxs-lookup"><span data-stu-id="23f66-180">hireDate</span></span>|<span data-ttu-id="23f66-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23f66-181">DateTimeOffset</span></span>|<span data-ttu-id="23f66-182">Дата найма пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-182">The hire date of the user.</span></span> <span data-ttu-id="23f66-183">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="23f66-183">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="23f66-184">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="23f66-184">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="23f66-185">identities</span><span class="sxs-lookup"><span data-stu-id="23f66-185">identities</span></span>|<span data-ttu-id="23f66-186">Коллекция [objectIdentity](../resources/objectidentity.md)</span><span class="sxs-lookup"><span data-stu-id="23f66-186">[objectIdentity](../resources/objectidentity.md) collection</span></span>| <span data-ttu-id="23f66-187">Представляет удостоверения, которые можно использовать для входа в учетную запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-187">Represents the identities that can be used to sign in to this user account.</span></span> <span data-ttu-id="23f66-188">Удостоверение может предоставляться корпорацией Майкрософт, организациями или поставщиками удостоверений социальных сетей, такими как Facebook, Google и Майкрософт, и привязывается к учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-188">An identity can be provided by Microsoft, by organizations, or by social identity providers such as Facebook, Google, and Microsoft, and tied to a user account.</span></span> <span data-ttu-id="23f66-189">Любое обновление **удостоверений** заменит всю коллекцию, и необходимо предоставить идентификатор userPrincipalName **signInType** в коллекции.</span><span class="sxs-lookup"><span data-stu-id="23f66-189">Any update to **identities** will replace the entire collection and you must supply the userPrincipalName **signInType** identity in the collection.</span></span>|
|<span data-ttu-id="23f66-190">interests;</span><span class="sxs-lookup"><span data-stu-id="23f66-190">interests</span></span>|<span data-ttu-id="23f66-191">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="23f66-191">String collection</span></span>|<span data-ttu-id="23f66-192">Список интересов пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-192">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="23f66-193">jobTitle</span><span class="sxs-lookup"><span data-stu-id="23f66-193">jobTitle</span></span>|<span data-ttu-id="23f66-194">String</span><span class="sxs-lookup"><span data-stu-id="23f66-194">String</span></span>|<span data-ttu-id="23f66-195">Должность пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-195">The user’s job title.</span></span>|
|<span data-ttu-id="23f66-196">почта;</span><span class="sxs-lookup"><span data-stu-id="23f66-196">mail</span></span>|<span data-ttu-id="23f66-197">String</span><span class="sxs-lookup"><span data-stu-id="23f66-197">String</span></span>|<span data-ttu-id="23f66-198">SMTP-адрес пользователя, например "gregory@contoso.onmicrosoft.com".</span><span class="sxs-lookup"><span data-stu-id="23f66-198">The SMTP address for the user, for example, "jeff@contoso.onmicrosoft.com".</span></span> <span data-ttu-id="23f66-199">Изменение этого свойства также приведет к обновлению коллекции пользователя **proxyAddresses**, которая будет включать это значение как SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="23f66-199">Changes to this property will also update the user's **proxyAddresses** collection to include the value as a SMTP address.</span></span> <br><br><span data-ttu-id="23f66-200">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="23f66-200">Returned by default.</span></span> <span data-ttu-id="23f66-201">Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="23f66-201">Supports $filter.</span></span>|
|<span data-ttu-id="23f66-202">mailNickname</span><span class="sxs-lookup"><span data-stu-id="23f66-202">mailNickname</span></span>|<span data-ttu-id="23f66-203">String</span><span class="sxs-lookup"><span data-stu-id="23f66-203">String</span></span>|<span data-ttu-id="23f66-204">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-204">The mail alias for the user.</span></span> <span data-ttu-id="23f66-205">Это свойство должно быть указано при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-205">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="23f66-206">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="23f66-206">mobilePhone</span></span>|<span data-ttu-id="23f66-207">String</span><span class="sxs-lookup"><span data-stu-id="23f66-207">String</span></span>|<span data-ttu-id="23f66-208">Основной сотовый телефон пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-208">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="23f66-209">mySite</span><span class="sxs-lookup"><span data-stu-id="23f66-209">mySite</span></span>|<span data-ttu-id="23f66-210">String</span><span class="sxs-lookup"><span data-stu-id="23f66-210">String</span></span>|<span data-ttu-id="23f66-211">URL-адрес личного сайта пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-211">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="23f66-212">officeLocation</span><span class="sxs-lookup"><span data-stu-id="23f66-212">officeLocation</span></span>|<span data-ttu-id="23f66-213">String</span><span class="sxs-lookup"><span data-stu-id="23f66-213">String</span></span>|<span data-ttu-id="23f66-214">Расположение офиса на месте работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-214">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="23f66-215">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="23f66-215">onPremisesImmutableId</span></span>|<span data-ttu-id="23f66-216">String</span><span class="sxs-lookup"><span data-stu-id="23f66-216">String</span></span>|<span data-ttu-id="23f66-217">Это свойство используется для сопоставления локальной учетной записи Active Directory с объектом пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="23f66-217">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="23f66-218">Его необходимо указывать при создании учетной записи пользователя в Graph, если в качестве свойства **userPrincipalName** (имени участника-пользователя) используется федеративный домен.</span><span class="sxs-lookup"><span data-stu-id="23f66-218">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="23f66-219">**Важно!** В этом свойстве не допускается использование символов **$** и **_**.</span><span class="sxs-lookup"><span data-stu-id="23f66-219">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="23f66-220">otherMails</span><span class="sxs-lookup"><span data-stu-id="23f66-220">otherMails</span></span>|<span data-ttu-id="23f66-221">String</span><span class="sxs-lookup"><span data-stu-id="23f66-221">String</span></span> |<span data-ttu-id="23f66-222">Список дополнительных адресов электронной почты для пользователя. Например: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="23f66-222">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="23f66-223">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="23f66-223">passwordPolicies</span></span>|<span data-ttu-id="23f66-224">String</span><span class="sxs-lookup"><span data-stu-id="23f66-224">String</span></span>|<span data-ttu-id="23f66-p117">Задает политики паролей для пользователя. Это свойство представляет собой перечисление с единственным возможным значением — "DisableStrongPassword". Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение "DisablePasswordExpiration". Эти значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="23f66-p117">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="23f66-229">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="23f66-229">passwordProfile</span></span>|[<span data-ttu-id="23f66-230">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="23f66-230">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="23f66-p118">Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="23f66-p118">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="23f66-236">pastProjects</span><span class="sxs-lookup"><span data-stu-id="23f66-236">pastProjects</span></span>|<span data-ttu-id="23f66-237">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="23f66-237">String collection</span></span>|<span data-ttu-id="23f66-238">Список предыдущих проектов пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-238">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="23f66-239">postalCode</span><span class="sxs-lookup"><span data-stu-id="23f66-239">postalCode</span></span>|<span data-ttu-id="23f66-240">String</span><span class="sxs-lookup"><span data-stu-id="23f66-240">String</span></span>|<span data-ttu-id="23f66-p119">Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код.</span><span class="sxs-lookup"><span data-stu-id="23f66-p119">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="23f66-244">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="23f66-244">preferredLanguage</span></span>|<span data-ttu-id="23f66-245">String</span><span class="sxs-lookup"><span data-stu-id="23f66-245">String</span></span>|<span data-ttu-id="23f66-p120">Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1, например "ru-RU".</span><span class="sxs-lookup"><span data-stu-id="23f66-p120">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="23f66-248">responsibilities</span><span class="sxs-lookup"><span data-stu-id="23f66-248">responsibilities</span></span>|<span data-ttu-id="23f66-249">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="23f66-249">String collection</span></span>|<span data-ttu-id="23f66-250">Список обязанностей пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-250">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="23f66-251">schools</span><span class="sxs-lookup"><span data-stu-id="23f66-251">schools</span></span>|<span data-ttu-id="23f66-252">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="23f66-252">String collection</span></span>|<span data-ttu-id="23f66-253">Список учебных заведений, которые посещал пользователь.</span><span class="sxs-lookup"><span data-stu-id="23f66-253">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="23f66-254">skills</span><span class="sxs-lookup"><span data-stu-id="23f66-254">skills</span></span>|<span data-ttu-id="23f66-255">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="23f66-255">String collection</span></span>|<span data-ttu-id="23f66-256">Список навыков пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-256">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="23f66-257">state</span><span class="sxs-lookup"><span data-stu-id="23f66-257">state</span></span>|<span data-ttu-id="23f66-258">String</span><span class="sxs-lookup"><span data-stu-id="23f66-258">String</span></span>|<span data-ttu-id="23f66-259">Область, республика, край или округ в адресе пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-259">The state or province in the user's address.</span></span>|
|<span data-ttu-id="23f66-260">streetAddress</span><span class="sxs-lookup"><span data-stu-id="23f66-260">streetAddress</span></span>|<span data-ttu-id="23f66-261">String</span><span class="sxs-lookup"><span data-stu-id="23f66-261">String</span></span>|<span data-ttu-id="23f66-262">Почтовый адрес места работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-262">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="23f66-263">surname</span><span class="sxs-lookup"><span data-stu-id="23f66-263">surname</span></span>|<span data-ttu-id="23f66-264">String</span><span class="sxs-lookup"><span data-stu-id="23f66-264">String</span></span>|<span data-ttu-id="23f66-265">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="23f66-265">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="23f66-266">usageLocation</span><span class="sxs-lookup"><span data-stu-id="23f66-266">usageLocation</span></span>|<span data-ttu-id="23f66-267">String</span><span class="sxs-lookup"><span data-stu-id="23f66-267">String</span></span>|<span data-ttu-id="23f66-268">Двухбуквенный код страны (по стандарту ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="23f66-268">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="23f66-269">Необходим для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в разных странах.</span><span class="sxs-lookup"><span data-stu-id="23f66-269">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="23f66-270">Примеры: "RU", "JP", "GB".</span><span class="sxs-lookup"><span data-stu-id="23f66-270">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="23f66-271">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="23f66-271">Not nullable.</span></span>|
|<span data-ttu-id="23f66-272">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="23f66-272">userPrincipalName</span></span>|<span data-ttu-id="23f66-273">String</span><span class="sxs-lookup"><span data-stu-id="23f66-273">String</span></span>|<span data-ttu-id="23f66-p122">Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](../resources/organization.md). Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="23f66-p122">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="23f66-281">userType</span><span class="sxs-lookup"><span data-stu-id="23f66-281">userType</span></span>|<span data-ttu-id="23f66-282">String</span><span class="sxs-lookup"><span data-stu-id="23f66-282">String</span></span>|<span data-ttu-id="23f66-283">Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость".</span><span class="sxs-lookup"><span data-stu-id="23f66-283">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

<span data-ttu-id="23f66-284">Поскольку ресурс **пользователя** поддерживает [расширения,](/graph/extensibility-overview)вы можете использовать операцию для добавления, обновления или удаления собственных данных, определенных для приложения, в настраиваемом свойстве расширения в существующем экземпляре `PATCH` пользователя. </span><span class="sxs-lookup"><span data-stu-id="23f66-284">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **user** instance.</span></span>

> [!NOTE] 
> <span data-ttu-id="23f66-285">Следующие свойства не могут быть обновлены с помощью контекста только для приложений: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools** и **skills**.</span><span class="sxs-lookup"><span data-stu-id="23f66-285">The follow properties cannot be updated using an application-only context: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, and **skills**.</span></span>

## <a name="response"></a><span data-ttu-id="23f66-286">Отклик</span><span class="sxs-lookup"><span data-stu-id="23f66-286">Response</span></span>

<span data-ttu-id="23f66-287">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="23f66-287">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="23f66-288">Пример</span><span class="sxs-lookup"><span data-stu-id="23f66-288">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="23f66-289">Пример 1. Обновление свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="23f66-289">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="23f66-290">Запрос</span><span class="sxs-lookup"><span data-stu-id="23f66-290">Request</span></span>

<span data-ttu-id="23f66-291">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23f66-291">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="23f66-292">HTTP</span><span class="sxs-lookup"><span data-stu-id="23f66-292">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/beta/me
Content-type: application/json

{
  "businessPhones": [
    "+1 425 555 0109"
  ],
  "officeLocation": "18/2111"
}
```
# <a name="c"></a>[<span data-ttu-id="23f66-293">C#</span><span class="sxs-lookup"><span data-stu-id="23f66-293">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23f66-294">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23f66-294">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23f66-295">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23f66-295">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23f66-296">Java</span><span class="sxs-lookup"><span data-stu-id="23f66-296">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="23f66-297">Отклик</span><span class="sxs-lookup"><span data-stu-id="23f66-297">Response</span></span>

<span data-ttu-id="23f66-298">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23f66-298">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="23f66-299">Пример 2. Обновление свойств указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="23f66-299">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="23f66-300">Запрос</span><span class="sxs-lookup"><span data-stu-id="23f66-300">Request</span></span>

<span data-ttu-id="23f66-301">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23f66-301">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="23f66-302">HTTP</span><span class="sxs-lookup"><span data-stu-id="23f66-302">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_other_user"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
  "businessPhones": [
    "+1 425 555 0109"
  ],
  "officeLocation": "18/2111"
}
```
# <a name="c"></a>[<span data-ttu-id="23f66-303">C#</span><span class="sxs-lookup"><span data-stu-id="23f66-303">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23f66-304">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23f66-304">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23f66-305">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23f66-305">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23f66-306">Java</span><span class="sxs-lookup"><span data-stu-id="23f66-306">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23f66-307">Отклик</span><span class="sxs-lookup"><span data-stu-id="23f66-307">Response</span></span>

<span data-ttu-id="23f66-308">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23f66-308">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="23f66-309">См. также</span><span class="sxs-lookup"><span data-stu-id="23f66-309">See also</span></span>

- [<span data-ttu-id="23f66-310">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="23f66-310">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="23f66-311">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="23f66-311">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="23f66-312">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="23f66-312">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
