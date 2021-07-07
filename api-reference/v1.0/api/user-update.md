---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e0dc12ea65ade7ed838a16645b414752ac0b1971
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208955"
---
# <a name="update-user"></a><span data-ttu-id="6ffe8-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="6ffe8-103">Update user</span></span>

<span data-ttu-id="6ffe8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ffe8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6ffe8-105">Обновление свойств объекта [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="6ffe8-105">Update the properties of a [user](../resources/user.md) object.</span></span> <span data-ttu-id="6ffe8-106">Не все свойства могут быть обновлены участниками или гостями с разрешениями по умолчанию без ролей администратора.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-106">Not all properties can be updated by Member or Guest users with their default permissions without Administrator roles.</span></span> <span data-ttu-id="6ffe8-107">[Сравните разрешения по умолчанию для участника и гостя](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions), чтобы узнать, какими свойствами они могут управлять.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-107">[Compare member and guest default permissions](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions) to see properties they can manage.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ffe8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ffe8-108">Permissions</span></span>
<span data-ttu-id="6ffe8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ffe8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ffe8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ffe8-111">Permission type</span></span>      | <span data-ttu-id="6ffe8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ffe8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ffe8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ffe8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6ffe8-114">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6ffe8-114">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ffe8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ffe8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ffe8-116">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ffe8-116">User.ReadWrite</span></span>    |
|<span data-ttu-id="6ffe8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ffe8-117">Application</span></span> | <span data-ttu-id="6ffe8-118">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ffe8-118">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="6ffe8-119">При обновлении свойства **passwordProfile** необходимо разрешение Directory.AccessAsUser.All.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-119">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="6ffe8-120">Обновление свойств **businessPhones**, **mobilePhone** или **otherMails** других пользователей разрешается только для пользователей, не являющихся администраторами, или для пользователей, которым назначена одна из следующих ролей: читатель каталога, приглашающий гостей, читатель Центра сообщений или читатель отчетов.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-120">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="6ffe8-121">Дополнительные сведения см. в разделе "Администратор службы поддержки (паролей)" среди [встроенных ролей Azure AD](/azure/active-directory/roles/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ffe8-121">For more details, see Helpdesk (Password) Administrator in [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference).</span></span>  <span data-ttu-id="6ffe8-122">Это относится к приложениям с предоставленными разрешениями User.ReadWrite.All или Directory.ReadWrite.All (делегированными или для приложений).</span><span class="sxs-lookup"><span data-stu-id="6ffe8-122">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>
> - <span data-ttu-id="6ffe8-123">Чтобы обновить профиль с делегированным разрешением User.ReadWrite в личной учетной записи Майкрософт, ваша личная учетная запись Майкрософт должна быть привязана к клиенту AAD.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-123">Your personal Microsoft account must be tied to an AAD tenant to update your profile with the User.ReadWrite delegated permission on a personal Microsoft account.</span></span>
> - <span data-ttu-id="6ffe8-124">Обновление свойства **личностей** требует разрешения User.ManageIdentities.All.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-124">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="6ffe8-125">Кроме того, добавление [локальной учетной записи B2C](../resources/objectidentity.md) к существующему объекту **пользователя** не допускается, если только объект **пользователя** не содержит идентификатор локальной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-125">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="6ffe8-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ffe8-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="6ffe8-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ffe8-127">Request headers</span></span>
| <span data-ttu-id="6ffe8-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ffe8-128">Header</span></span>       | <span data-ttu-id="6ffe8-129">Значение</span><span class="sxs-lookup"><span data-stu-id="6ffe8-129">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="6ffe8-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ffe8-130">Authorization</span></span>  | <span data-ttu-id="6ffe8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6ffe8-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6ffe8-133">Content-Type</span></span>  | <span data-ttu-id="6ffe8-134">application/json</span><span class="sxs-lookup"><span data-stu-id="6ffe8-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6ffe8-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ffe8-135">Request body</span></span>
<span data-ttu-id="6ffe8-p106">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6ffe8-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ffe8-139">Property</span></span>     | <span data-ttu-id="6ffe8-140">Тип</span><span class="sxs-lookup"><span data-stu-id="6ffe8-140">Type</span></span>   |<span data-ttu-id="6ffe8-141">Описание</span><span class="sxs-lookup"><span data-stu-id="6ffe8-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ffe8-142">aboutMe</span><span class="sxs-lookup"><span data-stu-id="6ffe8-142">aboutMe</span></span>|<span data-ttu-id="6ffe8-143">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-143">String</span></span>|<span data-ttu-id="6ffe8-144">Свободное текстовое поле, где пользователь может рассказать о себе.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-144">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="6ffe8-145">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="6ffe8-145">accountEnabled</span></span>|<span data-ttu-id="6ffe8-146">Логический</span><span class="sxs-lookup"><span data-stu-id="6ffe8-146">Boolean</span></span>| <span data-ttu-id="6ffe8-147">Если учетная запись обеспечена — `true`, в противном случае — `false`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-147">`true` if the account is enabled; otherwise, `false`.</span></span> <span data-ttu-id="6ffe8-148">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-148">This property is required when a user is created.</span></span>    |
| <span data-ttu-id="6ffe8-149">ageGroup</span><span class="sxs-lookup"><span data-stu-id="6ffe8-149">ageGroup</span></span> | [<span data-ttu-id="6ffe8-150">ageGroup</span><span class="sxs-lookup"><span data-stu-id="6ffe8-150">ageGroup</span></span>](../resources/user.md#agegroup-values) | <span data-ttu-id="6ffe8-151">Устанавливает возрастную группу пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-151">Sets the age group of the user.</span></span> <span data-ttu-id="6ffe8-152">Допустимые значения: `null`, `minor`, `notAdult` и `adult`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-152">Allowed values: `null`, `minor`, `notAdult` and `adult`.</span></span> <span data-ttu-id="6ffe8-153">Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](../resources/user.md#legal-age-group-property-definitions).</span><span class="sxs-lookup"><span data-stu-id="6ffe8-153">Refer to the [legal age group property definitions](../resources/user.md#legal-age-group-property-definitions) for further information.</span></span> |
|<span data-ttu-id="6ffe8-154">birthday</span><span class="sxs-lookup"><span data-stu-id="6ffe8-154">birthday</span></span>|<span data-ttu-id="6ffe8-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ffe8-155">DateTimeOffset</span></span>|<span data-ttu-id="6ffe8-156">День рождения пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-156">The birthday of the user.</span></span> <span data-ttu-id="6ffe8-157">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6ffe8-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6ffe8-158">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-158">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="6ffe8-159">businessPhones</span><span class="sxs-lookup"><span data-stu-id="6ffe8-159">businessPhones</span></span>| <span data-ttu-id="6ffe8-160">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6ffe8-160">String collection</span></span> | <span data-ttu-id="6ffe8-p110">Номера телефонов пользователя. ПРИМЕЧАНИЕ. Несмотря на то что это коллекция строк, в качестве этого свойства можно указать только одно число.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-p110">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="6ffe8-163">city</span><span class="sxs-lookup"><span data-stu-id="6ffe8-163">city</span></span>|<span data-ttu-id="6ffe8-164">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-164">String</span></span>|<span data-ttu-id="6ffe8-165">Город, в котором находится пользователь.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-165">The city in which the user is located.</span></span>|
| <span data-ttu-id="6ffe8-166">companyName</span><span class="sxs-lookup"><span data-stu-id="6ffe8-166">companyName</span></span> | <span data-ttu-id="6ffe8-167">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-167">String</span></span> | <span data-ttu-id="6ffe8-168">Название организации, с которой связан пользователь.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-168">The company name which the user is associated.</span></span> <span data-ttu-id="6ffe8-169">Это свойство может быть полезно для описания компании внешнего пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-169">This property can be useful for describing the company that an external user comes from.</span></span> <span data-ttu-id="6ffe8-170">Длина имени компании не должна превышать 64 символов.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-170">The maximum length of the company name is 64 characters.</span></span> |
| <span data-ttu-id="6ffe8-171">consentProvidedForMinor</span><span class="sxs-lookup"><span data-stu-id="6ffe8-171">consentProvidedForMinor</span></span> | [<span data-ttu-id="6ffe8-172">consentProvidedForMinor</span><span class="sxs-lookup"><span data-stu-id="6ffe8-172">consentProvidedForMinor</span></span>](../resources/user.md#consentprovidedforminor-values) | <span data-ttu-id="6ffe8-173">Устанавливает, получено ли согласие для несовершеннолетних.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-173">Sets whether consent has been obtained for minors.</span></span> <span data-ttu-id="6ffe8-174">Допустимые значения: `null`, `granted`, `denied` и `notRequired`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-174">Allowed values: `null`, `granted`, `denied` and `notRequired`.</span></span> <span data-ttu-id="6ffe8-175">Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](../resources/user.md#legal-age-group-property-definitions).</span><span class="sxs-lookup"><span data-stu-id="6ffe8-175">Refer to the [legal age group property definitions](../resources/user.md#legal-age-group-property-definitions) for further information.</span></span> |
|<span data-ttu-id="6ffe8-176">country</span><span class="sxs-lookup"><span data-stu-id="6ffe8-176">country</span></span>|<span data-ttu-id="6ffe8-177">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-177">String</span></span>|<span data-ttu-id="6ffe8-178">Страна или регион, в котором находится пользователь, например `US` или `UK`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-178">The country/region in which the user is located; for example, `US` or `UK`.</span></span>|
|<span data-ttu-id="6ffe8-179">department</span><span class="sxs-lookup"><span data-stu-id="6ffe8-179">department</span></span>|<span data-ttu-id="6ffe8-180">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-180">String</span></span>|<span data-ttu-id="6ffe8-181">Название отдела, в котором работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-181">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="6ffe8-182">displayName</span><span class="sxs-lookup"><span data-stu-id="6ffe8-182">displayName</span></span>|<span data-ttu-id="6ffe8-183">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-183">String</span></span>|<span data-ttu-id="6ffe8-184">Имя пользователя, отображаемое в адресной книге.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-184">The name displayed in the address book for the user.</span></span> <span data-ttu-id="6ffe8-185">Обычно это сочетание имени, отчества и фамилии пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-185">This is usually the combination of the user's first name, middle initial and last name.</span></span> <span data-ttu-id="6ffe8-186">Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-186">This property is required when a user is created and it cannot be cleared during updates.</span></span> <span data-ttu-id="6ffe8-187">Поддерживает `$filter` и `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-187">Supports `$filter` and `$orderby`.</span></span>|
| <span data-ttu-id="6ffe8-188">employeeId</span><span class="sxs-lookup"><span data-stu-id="6ffe8-188">employeeId</span></span> | <span data-ttu-id="6ffe8-189">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-189">String</span></span> | <span data-ttu-id="6ffe8-190">Идентификатор сотрудника, назначенный пользователю организацией.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-190">The employee identifier assigned to the user by the organization.</span></span> |
| <span data-ttu-id="6ffe8-191">employeeType</span><span class="sxs-lookup"><span data-stu-id="6ffe8-191">employeeType</span></span> | <span data-ttu-id="6ffe8-192">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-192">String</span></span> | <span data-ttu-id="6ffe8-193">Фиксирует тип корпоративного работника.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-193">Captures enterprise worker type.</span></span> <span data-ttu-id="6ffe8-194">Например, `Employee`, `Contractor`, `Consultant` или `Vendor`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-194">For example, `Employee`, `Contractor`, `Consultant`, or `Vendor`.</span></span> <span data-ttu-id="6ffe8-195">Возвращается только с помощью оператора `$select`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-195">Returned only on `$select`.</span></span>|
|<span data-ttu-id="6ffe8-196">givenName;</span><span class="sxs-lookup"><span data-stu-id="6ffe8-196">givenName</span></span>|<span data-ttu-id="6ffe8-197">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-197">String</span></span>|<span data-ttu-id="6ffe8-198">Простое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-198">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="6ffe8-199">hireDate</span><span class="sxs-lookup"><span data-stu-id="6ffe8-199">hireDate</span></span>|<span data-ttu-id="6ffe8-200">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ffe8-200">DateTimeOffset</span></span>|<span data-ttu-id="6ffe8-201">Дата найма пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-201">The hire date of the user.</span></span> <span data-ttu-id="6ffe8-202">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6ffe8-202">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6ffe8-203">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-203">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="6ffe8-204">interests;</span><span class="sxs-lookup"><span data-stu-id="6ffe8-204">interests</span></span>|<span data-ttu-id="6ffe8-205">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6ffe8-205">String collection</span></span>|<span data-ttu-id="6ffe8-206">Список интересов пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-206">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="6ffe8-207">jobTitle</span><span class="sxs-lookup"><span data-stu-id="6ffe8-207">jobTitle</span></span>|<span data-ttu-id="6ffe8-208">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-208">String</span></span>|<span data-ttu-id="6ffe8-209">Должность пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-209">The user’s job title.</span></span>|
|<span data-ttu-id="6ffe8-210">почта;</span><span class="sxs-lookup"><span data-stu-id="6ffe8-210">mail</span></span>|<span data-ttu-id="6ffe8-211">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-211">String</span></span>|<span data-ttu-id="6ffe8-212">SMTP-адрес пользователя, например `jeff@contoso.onmicrosoft.com`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-212">The SMTP address for the user, for example, `jeff@contoso.onmicrosoft.com`.</span></span> <span data-ttu-id="6ffe8-213">Изменение этого свойства также приведет к обновлению коллекции пользователя **proxyAddresses**, которая будет включать это значение как SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-213">Changes to this property will also update the user's **proxyAddresses** collection to include the value as a SMTP address.</span></span>|
|<span data-ttu-id="6ffe8-214">mailNickname</span><span class="sxs-lookup"><span data-stu-id="6ffe8-214">mailNickname</span></span>|<span data-ttu-id="6ffe8-215">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-215">String</span></span>|<span data-ttu-id="6ffe8-p117">Псевдоним электронной почты пользователя. Это свойство должно быть указано при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-p117">The mail alias for the user. This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="6ffe8-218">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="6ffe8-218">mobilePhone</span></span>|<span data-ttu-id="6ffe8-219">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-219">String</span></span>|<span data-ttu-id="6ffe8-220">Основной сотовый телефон пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-220">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="6ffe8-221">mySite</span><span class="sxs-lookup"><span data-stu-id="6ffe8-221">mySite</span></span>|<span data-ttu-id="6ffe8-222">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-222">String</span></span>|<span data-ttu-id="6ffe8-223">URL-адрес личного сайта пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-223">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="6ffe8-224">officeLocation</span><span class="sxs-lookup"><span data-stu-id="6ffe8-224">officeLocation</span></span>|<span data-ttu-id="6ffe8-225">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-225">String</span></span>|<span data-ttu-id="6ffe8-226">Расположение офиса на месте работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-226">The office location in the user's place of business.</span></span>|
| <span data-ttu-id="6ffe8-227">onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="6ffe8-227">onPremisesExtensionAttributes</span></span> | [<span data-ttu-id="6ffe8-228">onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="6ffe8-228">onPremisesExtensionAttributes</span></span>](../resources/onpremisesextensionattributes.md) | <span data-ttu-id="6ffe8-229">Содержит свойства extensionAttribute 1–15 для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-229">Contains extensionAttributes 1-15 for the user.</span></span> <span data-ttu-id="6ffe8-230">Обратите внимание, что отдельные атрибуты расширения нельзя выбирать и фильтровать.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-230">Note that the individual extension attributes are neither selectable nor filterable.</span></span> <span data-ttu-id="6ffe8-231">Для пользователей `onPremisesSyncEnabled` исходным центром управления для этого набора свойств является локальная среда, и он предназначен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-231">For an `onPremisesSyncEnabled` user, the source of authority for this set of properties is the on-premises and is read-only and is read-only.</span></span> <span data-ttu-id="6ffe8-232">Эти атрибуты расширения также называются настраиваемыми атрибутами 1–15 Exchange.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-232">These extension attributes are also known as Exchange custom attributes 1-15.</span></span>|
|<span data-ttu-id="6ffe8-233">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="6ffe8-233">onPremisesImmutableId</span></span>|<span data-ttu-id="6ffe8-234">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-234">String</span></span>|<span data-ttu-id="6ffe8-235">Это свойство используется для сопоставления локальной учетной записи Active Directory с объектом пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-235">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="6ffe8-236">Его необходимо указывать при создании учетной записи пользователя в Graph, если в качестве свойства **userPrincipalName** (имени участника-пользователя) используется федеративный домен.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-236">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="6ffe8-237">**Важно!** В этом свойстве не допускается использование символов **$** и **_**.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-237">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="6ffe8-238">otherMails</span><span class="sxs-lookup"><span data-stu-id="6ffe8-238">otherMails</span></span>|<span data-ttu-id="6ffe8-239">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-239">String</span></span> |<span data-ttu-id="6ffe8-240">Список дополнительных адресов электронной почты для пользователя. Например: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-240">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="6ffe8-241">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="6ffe8-241">passwordPolicies</span></span>|<span data-ttu-id="6ffe8-242">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-242">String</span></span>|<span data-ttu-id="6ffe8-243">Задает политики паролей для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-243">Specifies password policies for the user.</span></span> <span data-ttu-id="6ffe8-244">Это свойство представляет собой перечисление с возможным значением `DisableStrongPassword`. Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-244">This value is an enumeration with one possible value being `DisableStrongPassword`, which allows weaker passwords than the default policy to be specified.</span></span> <span data-ttu-id="6ffe8-245">Вы также можете указать значение `DisablePasswordExpiration`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-245">`DisablePasswordExpiration` can also be specified.</span></span> <span data-ttu-id="6ffe8-246">Два значения можно указать одновременно. Пример: `DisablePasswordExpiration, DisableStrongPassword`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-246">The two may be specified together; for example: `DisablePasswordExpiration, DisableStrongPassword`.</span></span>|
|<span data-ttu-id="6ffe8-247">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="6ffe8-247">passwordProfile</span></span>|[<span data-ttu-id="6ffe8-248">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="6ffe8-248">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="6ffe8-249">Задает профиль пароля для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-249">Specifies the password profile for the user.</span></span> <span data-ttu-id="6ffe8-250">Профиль содержит пароль пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-250">The profile contains the user’s password.</span></span> <span data-ttu-id="6ffe8-251">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-251">This property is required when a user is created.</span></span> <span data-ttu-id="6ffe8-252">Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-252">The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property.</span></span> <span data-ttu-id="6ffe8-253">По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-253">By default, a strong password is required.</span></span> <span data-ttu-id="6ffe8-254">Это невозможно использовать для федеративных пользователей.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-254">This cannot be used for federated users.</span></span> <span data-ttu-id="6ffe8-255">Чтобы обновить это свойство, требуется разрешение *Directory.AccessAsUser.All*.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-255">The *Directory.AccessAsUser.All* permission is required to update this property.</span></span>|
|<span data-ttu-id="6ffe8-256">pastProjects</span><span class="sxs-lookup"><span data-stu-id="6ffe8-256">pastProjects</span></span>|<span data-ttu-id="6ffe8-257">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6ffe8-257">String collection</span></span>|<span data-ttu-id="6ffe8-258">Список предыдущих проектов пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-258">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="6ffe8-259">postalCode</span><span class="sxs-lookup"><span data-stu-id="6ffe8-259">postalCode</span></span>|<span data-ttu-id="6ffe8-260">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-260">String</span></span>|<span data-ttu-id="6ffe8-p122">Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-p122">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="6ffe8-264">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="6ffe8-264">preferredLanguage</span></span>|<span data-ttu-id="6ffe8-265">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-265">String</span></span>|<span data-ttu-id="6ffe8-266">Предпочитаемый язык для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-266">The preferred language for the user.</span></span> <span data-ttu-id="6ffe8-267">Он должен быть представлен в формате ISO 639-1, например `en-US`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-267">Should follow ISO 639-1 Code; for example `en-US`.</span></span>|
|<span data-ttu-id="6ffe8-268">responsibilities;</span><span class="sxs-lookup"><span data-stu-id="6ffe8-268">responsibilities</span></span>|<span data-ttu-id="6ffe8-269">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6ffe8-269">String collection</span></span>|<span data-ttu-id="6ffe8-270">Список обязанностей пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-270">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="6ffe8-271">schools</span><span class="sxs-lookup"><span data-stu-id="6ffe8-271">schools</span></span>|<span data-ttu-id="6ffe8-272">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6ffe8-272">String collection</span></span>|<span data-ttu-id="6ffe8-273">Список учебных заведений, которые посещал пользователь.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-273">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="6ffe8-274">skills</span><span class="sxs-lookup"><span data-stu-id="6ffe8-274">skills</span></span>|<span data-ttu-id="6ffe8-275">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6ffe8-275">String collection</span></span>|<span data-ttu-id="6ffe8-276">Список навыков пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-276">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="6ffe8-277">state</span><span class="sxs-lookup"><span data-stu-id="6ffe8-277">state</span></span>|<span data-ttu-id="6ffe8-278">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-278">String</span></span>|<span data-ttu-id="6ffe8-279">Область, республика, край или округ в адресе пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-279">The state or province in the user's address.</span></span>|
|<span data-ttu-id="6ffe8-280">streetAddress</span><span class="sxs-lookup"><span data-stu-id="6ffe8-280">streetAddress</span></span>|<span data-ttu-id="6ffe8-281">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-281">String</span></span>|<span data-ttu-id="6ffe8-282">Почтовый адрес места работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-282">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="6ffe8-283">surname</span><span class="sxs-lookup"><span data-stu-id="6ffe8-283">surname</span></span>|<span data-ttu-id="6ffe8-284">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-284">String</span></span>|<span data-ttu-id="6ffe8-285">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-285">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="6ffe8-286">usageLocation</span><span class="sxs-lookup"><span data-stu-id="6ffe8-286">usageLocation</span></span>|<span data-ttu-id="6ffe8-287">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-287">String</span></span>|<span data-ttu-id="6ffe8-288">Двухбуквенный код страны (по стандарту ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="6ffe8-288">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="6ffe8-289">Необходим для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в разных странах.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-289">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="6ffe8-290">Примеры: `US`, `JP` и `GB`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-290">Examples include: `US`, `JP`, and `GB`.</span></span> <span data-ttu-id="6ffe8-291">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-291">Not nullable.</span></span>|
|<span data-ttu-id="6ffe8-292">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6ffe8-292">userPrincipalName</span></span>|<span data-ttu-id="6ffe8-293">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-293">String</span></span>|<span data-ttu-id="6ffe8-294">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-294">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="6ffe8-295">Это имя для входа через Интернет по стандарту RFC 822.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-295">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="6ffe8-296">В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-296">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="6ffe8-297">Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-297">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="6ffe8-298">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-298">This property is required when a user is created.</span></span> <span data-ttu-id="6ffe8-299">Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](../resources/organization.md).</span><span class="sxs-lookup"><span data-stu-id="6ffe8-299">The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md).</span></span> <span data-ttu-id="6ffe8-300">Поддерживает `$filter` и `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-300">Supports `$filter` and `$orderby`.</span></span>
|<span data-ttu-id="6ffe8-301">userType</span><span class="sxs-lookup"><span data-stu-id="6ffe8-301">userType</span></span>|<span data-ttu-id="6ffe8-302">String</span><span class="sxs-lookup"><span data-stu-id="6ffe8-302">String</span></span>|<span data-ttu-id="6ffe8-303">Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например `Member` и `Guest`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-303">A string value that can be used to classify user types in your directory, such as `Member` and `Guest`.</span></span>          |

> [!NOTE] 
> <span data-ttu-id="6ffe8-304">Следующие свойства не могут быть обновлены с помощью контекста только для приложений: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools** и **skills**.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-304">The follow properties cannot be updated using an application-only context: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, and **skills**.</span></span>

## <a name="response"></a><span data-ttu-id="6ffe8-305">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ffe8-305">Response</span></span>

<span data-ttu-id="6ffe8-306">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-306">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6ffe8-307">Пример</span><span class="sxs-lookup"><span data-stu-id="6ffe8-307">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="6ffe8-308">Пример 1. Обновление свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="6ffe8-308">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="6ffe8-309">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ffe8-309">Request</span></span>

<span data-ttu-id="6ffe8-310">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-310">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6ffe8-311">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ffe8-311">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6ffe8-312">C#</span><span class="sxs-lookup"><span data-stu-id="6ffe8-312">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ffe8-313">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ffe8-313">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ffe8-314">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ffe8-314">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6ffe8-315">Java</span><span class="sxs-lookup"><span data-stu-id="6ffe8-315">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6ffe8-316">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ffe8-316">Response</span></span>
<span data-ttu-id="6ffe8-317">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-317">The following example shows the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="6ffe8-318">Пример 2. Обновление свойств указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="6ffe8-318">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="6ffe8-319">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ffe8-319">Request</span></span>

<span data-ttu-id="6ffe8-320">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-320">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6ffe8-321">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ffe8-321">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6ffe8-322">C#</span><span class="sxs-lookup"><span data-stu-id="6ffe8-322">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ffe8-323">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ffe8-323">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ffe8-324">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ffe8-324">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6ffe8-325">Java</span><span class="sxs-lookup"><span data-stu-id="6ffe8-325">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6ffe8-326">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ffe8-326">Response</span></span>

<span data-ttu-id="6ffe8-327">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-327">The following example shows the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```


### <a name="example-3-update-the-passwordprofile-of-a-user-to-reset-their-password"></a><span data-ttu-id="6ffe8-328">Пример 3. Обновление passwordProfile пользователя для сброса его пароля</span><span class="sxs-lookup"><span data-stu-id="6ffe8-328">Example 3: Update the passwordProfile of a user to reset their password</span></span>

<span data-ttu-id="6ffe8-329">В приведенном ниже примере показан запрос на сброс пароля другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ffe8-329">The following example shows a request to reset the password of another user.</span></span>

#### <a name="request"></a><span data-ttu-id="6ffe8-330">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ffe8-330">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_user_passwordProfile"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id}
Content-type: application/json

{
  "passwordProfile": {
    "forceChangePasswordNextSignIn": false,
    "password": "xWwvJ]6NMw+bWH-d"
  }
}
```


#### <a name="response"></a><span data-ttu-id="6ffe8-331">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ffe8-331">Response</span></span>
<!-- {
  "blockType": "response"
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
