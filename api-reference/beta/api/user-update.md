---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b7920abc59b3d67da54ff4f880df373afb34e46b
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316662"
---
# <a name="update-user"></a><span data-ttu-id="448c3-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="448c3-103">Update user</span></span>

<span data-ttu-id="448c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="448c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="448c3-105">Обновление свойств объекта [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="448c3-105">Update the properties of a [user](../resources/user.md) object.</span></span> <span data-ttu-id="448c3-106">Не все свойства могут быть обновлены участниками или гостями с разрешениями по умолчанию без ролей администратора.</span><span class="sxs-lookup"><span data-stu-id="448c3-106">Not all properties can be updated by Member or Guest users with their default permissions without Administrator roles.</span></span> <span data-ttu-id="448c3-107">[Сравните разрешения по умолчанию для участника и гостя](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions), чтобы узнать, какими свойствами они могут управлять.</span><span class="sxs-lookup"><span data-stu-id="448c3-107">[Compare member and guest default permissions](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions) to see properties they can manage.</span></span>

## <a name="permissions"></a><span data-ttu-id="448c3-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="448c3-108">Permissions</span></span>
<span data-ttu-id="448c3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="448c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="448c3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="448c3-111">Permission type</span></span>      | <span data-ttu-id="448c3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="448c3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="448c3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="448c3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="448c3-114">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="448c3-114">User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="448c3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="448c3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="448c3-116">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="448c3-116">User.ReadWrite</span></span>    |
|<span data-ttu-id="448c3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="448c3-117">Application</span></span> | <span data-ttu-id="448c3-118">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="448c3-118">User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="448c3-119">При обновлении **свойства passwordProfile** требуется следующее разрешение: *Directory.AccessAsUser.All*.</span><span class="sxs-lookup"><span data-stu-id="448c3-119">When updating the **passwordProfile** property, the following permission is required: *Directory.AccessAsUser.All*.</span></span>
> - <span data-ttu-id="448c3-120">Обновление свойств **businessPhones**, **mobilePhone** или **otherMails** других пользователей разрешается только для пользователей, не являющихся администраторами, или для пользователей, которым назначена одна из следующих ролей: читатель каталога, приглашающий гостей, читатель Центра сообщений или читатель отчетов.</span><span class="sxs-lookup"><span data-stu-id="448c3-120">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="448c3-121">Дополнительные сведения см. в разделе "Администратор службы поддержки (паролей)" среди [встроенных ролей Azure AD](/azure/active-directory/roles/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="448c3-121">For more details, see Helpdesk (Password) Administrator in [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference).</span></span>  <span data-ttu-id="448c3-122">Это относится к приложениям с предоставленными разрешениями User.ReadWrite.All или Directory.ReadWrite.All (делегированными или для приложений).</span><span class="sxs-lookup"><span data-stu-id="448c3-122">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>
> - <span data-ttu-id="448c3-123">Чтобы обновить профиль с делегированным разрешением User.ReadWrite в личной учетной записи Майкрософт, ваша личная учетная запись Майкрософт должна быть привязана к клиенту AAD.</span><span class="sxs-lookup"><span data-stu-id="448c3-123">Your personal Microsoft account must be tied to an AAD tenant to update your profile with the User.ReadWrite delegated permission on a personal Microsoft account.</span></span>
> - <span data-ttu-id="448c3-124">Обновление свойства **личностей** требует разрешения User.ManageIdentities.All.</span><span class="sxs-lookup"><span data-stu-id="448c3-124">Updating the **identities** property requires the User.ManageIdentities.All permission.</span></span> <span data-ttu-id="448c3-125">Кроме того, добавление [локальной учетной записи B2C](../resources/objectidentity.md) к существующему объекту **пользователя** не допускается, если только объект **пользователя** не содержит идентификатор локальной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="448c3-125">Also, adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="http-request"></a><span data-ttu-id="448c3-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="448c3-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="448c3-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="448c3-127">Request headers</span></span>
| <span data-ttu-id="448c3-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="448c3-128">Header</span></span>       | <span data-ttu-id="448c3-129">Значение</span><span class="sxs-lookup"><span data-stu-id="448c3-129">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="448c3-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="448c3-130">Authorization</span></span>  | <span data-ttu-id="448c3-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="448c3-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="448c3-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="448c3-133">Content-Type</span></span>  | <span data-ttu-id="448c3-134">application/json</span><span class="sxs-lookup"><span data-stu-id="448c3-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="448c3-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="448c3-135">Request body</span></span>
<span data-ttu-id="448c3-p106">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="448c3-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="448c3-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="448c3-139">Property</span></span>     | <span data-ttu-id="448c3-140">Тип</span><span class="sxs-lookup"><span data-stu-id="448c3-140">Type</span></span>   |<span data-ttu-id="448c3-141">Описание</span><span class="sxs-lookup"><span data-stu-id="448c3-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="448c3-142">aboutMe</span><span class="sxs-lookup"><span data-stu-id="448c3-142">aboutMe</span></span>|<span data-ttu-id="448c3-143">String</span><span class="sxs-lookup"><span data-stu-id="448c3-143">String</span></span>|<span data-ttu-id="448c3-144">Свободное текстовое поле, где пользователь может рассказать о себе.</span><span class="sxs-lookup"><span data-stu-id="448c3-144">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="448c3-145">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="448c3-145">accountEnabled</span></span>|<span data-ttu-id="448c3-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="448c3-146">Boolean</span></span>| <span data-ttu-id="448c3-147">Значение **true** указывает, что учетная запись включена. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="448c3-147">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="448c3-148">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-148">This property is required when a user is created.</span></span>    |
| <span data-ttu-id="448c3-149">ageGroup</span><span class="sxs-lookup"><span data-stu-id="448c3-149">ageGroup</span></span> | [<span data-ttu-id="448c3-150">ageGroup</span><span class="sxs-lookup"><span data-stu-id="448c3-150">ageGroup</span></span>](../resources/user.md#agegroup-values) | <span data-ttu-id="448c3-151">Устанавливает возрастную группу пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-151">Sets the age group of the user.</span></span> <span data-ttu-id="448c3-152">Допустимые значения: `null`, `minor`, `notAdult` и `adult`.</span><span class="sxs-lookup"><span data-stu-id="448c3-152">Allowed values: `null`, `minor`, `notAdult` and `adult`.</span></span> <span data-ttu-id="448c3-153">Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](../resources/user.md#legal-age-group-property-definitions).</span><span class="sxs-lookup"><span data-stu-id="448c3-153">Refer to the [legal age group property definitions](../resources/user.md#legal-age-group-property-definitions) for further information.</span></span> |
|<span data-ttu-id="448c3-154">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="448c3-154">assignedLicenses</span></span>|<span data-ttu-id="448c3-155">Коллекция [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="448c3-155">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="448c3-p109">Лицензии, назначенные пользователю. Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="448c3-p109">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="448c3-158">birthday</span><span class="sxs-lookup"><span data-stu-id="448c3-158">birthday</span></span>|<span data-ttu-id="448c3-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="448c3-159">DateTimeOffset</span></span>|<span data-ttu-id="448c3-160">День рождения пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-160">The birthday of the user.</span></span> <span data-ttu-id="448c3-161">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="448c3-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="448c3-162">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="448c3-162">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="448c3-163">businessPhones</span><span class="sxs-lookup"><span data-stu-id="448c3-163">businessPhones</span></span>| <span data-ttu-id="448c3-164">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="448c3-164">String collection</span></span> | <span data-ttu-id="448c3-p111">Номера телефонов пользователя. ПРИМЕЧАНИЕ. Несмотря на то что это коллекция строк, в качестве этого свойства можно указать только одно число.</span><span class="sxs-lookup"><span data-stu-id="448c3-p111">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="448c3-167">city</span><span class="sxs-lookup"><span data-stu-id="448c3-167">city</span></span>|<span data-ttu-id="448c3-168">String</span><span class="sxs-lookup"><span data-stu-id="448c3-168">String</span></span>|<span data-ttu-id="448c3-169">Город, в котором находится пользователь.</span><span class="sxs-lookup"><span data-stu-id="448c3-169">The city in which the user is located.</span></span>|
| <span data-ttu-id="448c3-170">companyName</span><span class="sxs-lookup"><span data-stu-id="448c3-170">companyName</span></span> | <span data-ttu-id="448c3-171">String</span><span class="sxs-lookup"><span data-stu-id="448c3-171">String</span></span> | <span data-ttu-id="448c3-172">Название организации, с которой связан пользователь.</span><span class="sxs-lookup"><span data-stu-id="448c3-172">The company name which the user is associated.</span></span> <span data-ttu-id="448c3-173">Это свойство может быть полезно для описания компании внешнего пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-173">This property can be useful for describing the company that an external user comes from.</span></span> <span data-ttu-id="448c3-174">Длина имени компании не должна превышать 64 символов.</span><span class="sxs-lookup"><span data-stu-id="448c3-174">The maximum length of the company name is 64 characters.</span></span> |
| <span data-ttu-id="448c3-175">consentProvidedForMinor</span><span class="sxs-lookup"><span data-stu-id="448c3-175">consentProvidedForMinor</span></span> | [<span data-ttu-id="448c3-176">consentProvidedForMinor</span><span class="sxs-lookup"><span data-stu-id="448c3-176">consentProvidedForMinor</span></span>](../resources/user.md#consentprovidedforminor-values) | <span data-ttu-id="448c3-177">Устанавливает, получено ли согласие для несовершеннолетних.</span><span class="sxs-lookup"><span data-stu-id="448c3-177">Sets whether consent has been obtained for minors.</span></span> <span data-ttu-id="448c3-178">Допустимые значения: `null`, `granted`, `denied` и `notRequired`.</span><span class="sxs-lookup"><span data-stu-id="448c3-178">Allowed values: `null`, `granted`, `denied` and `notRequired`.</span></span> <span data-ttu-id="448c3-179">Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](../resources/user.md#legal-age-group-property-definitions).</span><span class="sxs-lookup"><span data-stu-id="448c3-179">Refer to the [legal age group property definitions](../resources/user.md#legal-age-group-property-definitions) for further information.</span></span> |
|<span data-ttu-id="448c3-180">country</span><span class="sxs-lookup"><span data-stu-id="448c3-180">country</span></span>|<span data-ttu-id="448c3-181">String</span><span class="sxs-lookup"><span data-stu-id="448c3-181">String</span></span>|<span data-ttu-id="448c3-182">Страна или регион, в котором находится пользователь, например "США" или "Соединенное Королевство".</span><span class="sxs-lookup"><span data-stu-id="448c3-182">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="448c3-183">department</span><span class="sxs-lookup"><span data-stu-id="448c3-183">department</span></span>|<span data-ttu-id="448c3-184">String</span><span class="sxs-lookup"><span data-stu-id="448c3-184">String</span></span>|<span data-ttu-id="448c3-185">Название отдела, в котором работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="448c3-185">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="448c3-186">displayName</span><span class="sxs-lookup"><span data-stu-id="448c3-186">displayName</span></span>|<span data-ttu-id="448c3-187">String</span><span class="sxs-lookup"><span data-stu-id="448c3-187">String</span></span>|<span data-ttu-id="448c3-188">Имя пользователя, отображаемое в адресной книге.</span><span class="sxs-lookup"><span data-stu-id="448c3-188">The name displayed in the address book for the user.</span></span> <span data-ttu-id="448c3-189">Обычно это сочетание имени, отчества и фамилии пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-189">This is usually the combination of the user's first name, middle initial and last name.</span></span> <span data-ttu-id="448c3-190">Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении.</span><span class="sxs-lookup"><span data-stu-id="448c3-190">This property is required when a user is created and it cannot be cleared during updates.</span></span> <span data-ttu-id="448c3-191">Поддерживает `$filter` и `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="448c3-191">Supports `$filter` and `$orderby`.</span></span>|
|<span data-ttu-id="448c3-192">employeeId</span><span class="sxs-lookup"><span data-stu-id="448c3-192">employeeId</span></span>|<span data-ttu-id="448c3-193">String</span><span class="sxs-lookup"><span data-stu-id="448c3-193">String</span></span>|<span data-ttu-id="448c3-194">Идентификатор сотрудника, назначенный пользователю организацией.</span><span class="sxs-lookup"><span data-stu-id="448c3-194">The employee identifier assigned to the user by the organization.</span></span>|
| <span data-ttu-id="448c3-195">employeeType</span><span class="sxs-lookup"><span data-stu-id="448c3-195">employeeType</span></span> | <span data-ttu-id="448c3-196">String</span><span class="sxs-lookup"><span data-stu-id="448c3-196">String</span></span> | <span data-ttu-id="448c3-197">Фиксирует тип корпоративного работника.</span><span class="sxs-lookup"><span data-stu-id="448c3-197">Captures enterprise worker type.</span></span> <span data-ttu-id="448c3-198">Например, `Employee`, `Contractor`, `Consultant` или `Vendor`.</span><span class="sxs-lookup"><span data-stu-id="448c3-198">For example, `Employee`, `Contractor`, `Consultant`, or `Vendor`.</span></span> <span data-ttu-id="448c3-199">Возвращается только с помощью оператора `$select`.</span><span class="sxs-lookup"><span data-stu-id="448c3-199">Returned only on `$select`.</span></span> <span data-ttu-id="448c3-200">Поддерживает `$filter` с оператором `eq`.</span><span class="sxs-lookup"><span data-stu-id="448c3-200">Supports `$filter` with the `eq` operator.</span></span>|
|<span data-ttu-id="448c3-201">givenName</span><span class="sxs-lookup"><span data-stu-id="448c3-201">givenName</span></span>|<span data-ttu-id="448c3-202">String</span><span class="sxs-lookup"><span data-stu-id="448c3-202">String</span></span>|<span data-ttu-id="448c3-203">Простое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-203">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="448c3-204">hireDate</span><span class="sxs-lookup"><span data-stu-id="448c3-204">hireDate</span></span>|<span data-ttu-id="448c3-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="448c3-205">DateTimeOffset</span></span>|<span data-ttu-id="448c3-206">Дата найма пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-206">The hire date of the user.</span></span> <span data-ttu-id="448c3-207">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="448c3-207">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="448c3-208">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="448c3-208">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="448c3-209">identities</span><span class="sxs-lookup"><span data-stu-id="448c3-209">identities</span></span>|<span data-ttu-id="448c3-210">Коллекция [objectIdentity](../resources/objectidentity.md)</span><span class="sxs-lookup"><span data-stu-id="448c3-210">[objectIdentity](../resources/objectidentity.md) collection</span></span>| <span data-ttu-id="448c3-211">Представляет удостоверения, которые можно использовать для входа в учетную запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-211">Represents the identities that can be used to sign in to this user account.</span></span> <span data-ttu-id="448c3-212">Удостоверение может предоставляться корпорацией Майкрософт, организациями или поставщиками удостоверений социальных сетей, такими как Facebook, Google и Майкрософт, и привязывается к учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-212">An identity can be provided by Microsoft, by organizations, or by social identity providers such as Facebook, Google, and Microsoft, and tied to a user account.</span></span> <span data-ttu-id="448c3-213">Любое обновление **удостоверений** заменит всю коллекцию, и необходимо предоставить идентификатор userPrincipalName **signInType** в коллекции.</span><span class="sxs-lookup"><span data-stu-id="448c3-213">Any update to **identities** will replace the entire collection and you must supply the userPrincipalName **signInType** identity in the collection.</span></span>|
|<span data-ttu-id="448c3-214">interests;</span><span class="sxs-lookup"><span data-stu-id="448c3-214">interests</span></span>|<span data-ttu-id="448c3-215">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="448c3-215">String collection</span></span>|<span data-ttu-id="448c3-216">Список интересов пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-216">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="448c3-217">jobTitle</span><span class="sxs-lookup"><span data-stu-id="448c3-217">jobTitle</span></span>|<span data-ttu-id="448c3-218">String</span><span class="sxs-lookup"><span data-stu-id="448c3-218">String</span></span>|<span data-ttu-id="448c3-219">Должность пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-219">The user’s job title.</span></span>|
|<span data-ttu-id="448c3-220">почта;</span><span class="sxs-lookup"><span data-stu-id="448c3-220">mail</span></span>|<span data-ttu-id="448c3-221">String</span><span class="sxs-lookup"><span data-stu-id="448c3-221">String</span></span>|<span data-ttu-id="448c3-222">SMTP-адрес пользователя, например `jeff@contoso.onmicrosoft.com`.</span><span class="sxs-lookup"><span data-stu-id="448c3-222">The SMTP address for the user, for example, `jeff@contoso.onmicrosoft.com`.</span></span> <span data-ttu-id="448c3-223">Изменение этого свойства также приведет к обновлению коллекции пользователя **proxyAddresses**, которая будет включать это значение как SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="448c3-223">Changes to this property will also update the user's **proxyAddresses** collection to include the value as a SMTP address.</span></span> <br><br><span data-ttu-id="448c3-224">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="448c3-224">Returned by default.</span></span> <span data-ttu-id="448c3-225">Поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="448c3-225">Supports `$filter`.</span></span>|
|<span data-ttu-id="448c3-226">mailNickname</span><span class="sxs-lookup"><span data-stu-id="448c3-226">mailNickname</span></span>|<span data-ttu-id="448c3-227">String</span><span class="sxs-lookup"><span data-stu-id="448c3-227">String</span></span>|<span data-ttu-id="448c3-p120">Псевдоним электронной почты пользователя. Это свойство должно быть указано при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-p120">The mail alias for the user. This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="448c3-230">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="448c3-230">mobilePhone</span></span>|<span data-ttu-id="448c3-231">String</span><span class="sxs-lookup"><span data-stu-id="448c3-231">String</span></span>|<span data-ttu-id="448c3-232">Основной сотовый телефон пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-232">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="448c3-233">mySite</span><span class="sxs-lookup"><span data-stu-id="448c3-233">mySite</span></span>|<span data-ttu-id="448c3-234">String</span><span class="sxs-lookup"><span data-stu-id="448c3-234">String</span></span>|<span data-ttu-id="448c3-235">URL-адрес личного сайта пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-235">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="448c3-236">officeLocation</span><span class="sxs-lookup"><span data-stu-id="448c3-236">officeLocation</span></span>|<span data-ttu-id="448c3-237">String</span><span class="sxs-lookup"><span data-stu-id="448c3-237">String</span></span>|<span data-ttu-id="448c3-238">Расположение офиса на месте работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-238">The office location in the user's place of business.</span></span>|
| <span data-ttu-id="448c3-239">onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="448c3-239">onPremisesExtensionAttributes</span></span> | [<span data-ttu-id="448c3-240">onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="448c3-240">onPremisesExtensionAttributes</span></span>](../resources/onpremisesextensionattributes.md) | <span data-ttu-id="448c3-241">Содержит свойства extensionAttribute 1–15 для пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-241">Contains extensionAttributes 1-15 for the user.</span></span> <span data-ttu-id="448c3-242">Обратите внимание, что отдельные атрибуты расширения нельзя выбирать и фильтровать.</span><span class="sxs-lookup"><span data-stu-id="448c3-242">Note that the individual extension attributes are neither selectable nor filterable.</span></span> <span data-ttu-id="448c3-243">Для пользователей `onPremisesSyncEnabled` исходным центром управления для этого набора свойств является локальная среда, и он предназначен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="448c3-243">For an `onPremisesSyncEnabled` user, the source of authority for this set of properties is the on-premises and is read-only and is read-only.</span></span> <span data-ttu-id="448c3-244">Эти атрибуты расширения также называются настраиваемыми атрибутами 1–15 Exchange.</span><span class="sxs-lookup"><span data-stu-id="448c3-244">These extension attributes are also known as Exchange custom attributes 1-15.</span></span>|
|<span data-ttu-id="448c3-245">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="448c3-245">onPremisesImmutableId</span></span>|<span data-ttu-id="448c3-246">String</span><span class="sxs-lookup"><span data-stu-id="448c3-246">String</span></span>|<span data-ttu-id="448c3-247">Это свойство используется для сопоставления локальной учетной записи Active Directory с объектом пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="448c3-247">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="448c3-248">Его необходимо указывать при создании учетной записи пользователя в Graph, если в качестве свойства **userPrincipalName** (имени участника-пользователя) используется федеративный домен.</span><span class="sxs-lookup"><span data-stu-id="448c3-248">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="448c3-249">**Важно!** В этом свойстве не допускается использование символов **$** и **_**.</span><span class="sxs-lookup"><span data-stu-id="448c3-249">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="448c3-250">otherMails</span><span class="sxs-lookup"><span data-stu-id="448c3-250">otherMails</span></span>|<span data-ttu-id="448c3-251">String</span><span class="sxs-lookup"><span data-stu-id="448c3-251">String</span></span> |<span data-ttu-id="448c3-252">Список дополнительных адресов электронной почты для пользователя. Например: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span><span class="sxs-lookup"><span data-stu-id="448c3-252">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="448c3-253">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="448c3-253">passwordPolicies</span></span>|<span data-ttu-id="448c3-254">String</span><span class="sxs-lookup"><span data-stu-id="448c3-254">String</span></span>|<span data-ttu-id="448c3-255">Задает политики паролей для пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-255">Specifies password policies for the user.</span></span> <span data-ttu-id="448c3-256">Это свойство представляет собой перечисление с возможным значением `DisableStrongPassword`. Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="448c3-256">This value is an enumeration with one possible value being `DisableStrongPassword`, which allows weaker passwords than the default policy to be specified.</span></span> <span data-ttu-id="448c3-257">Вы также можете указать значение `DisablePasswordExpiration`.</span><span class="sxs-lookup"><span data-stu-id="448c3-257">`DisablePasswordExpiration` can also be specified.</span></span> <span data-ttu-id="448c3-258">Два значения можно указать одновременно. Пример: `DisablePasswordExpiration, DisableStrongPassword`.</span><span class="sxs-lookup"><span data-stu-id="448c3-258">The two may be specified together; for example: `DisablePasswordExpiration, DisableStrongPassword`.</span></span>|
|<span data-ttu-id="448c3-259">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="448c3-259">passwordProfile</span></span>|[<span data-ttu-id="448c3-260">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="448c3-260">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="448c3-261">Задает профиль пароля для пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-261">Specifies the password profile for the user.</span></span> <span data-ttu-id="448c3-262">Профиль содержит пароль пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-262">The profile contains the user’s password.</span></span> <span data-ttu-id="448c3-263">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-263">This property is required when a user is created.</span></span> <span data-ttu-id="448c3-264">Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**.</span><span class="sxs-lookup"><span data-stu-id="448c3-264">The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property.</span></span> <span data-ttu-id="448c3-265">По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="448c3-265">By default, a strong password is required.</span></span> <span data-ttu-id="448c3-266">Чтобы обновить это свойство, требуется разрешение *Directory.AccessAsUser.All*.</span><span class="sxs-lookup"><span data-stu-id="448c3-266">The *Directory.AccessAsUser.All* permission is required to update this property.</span></span>|
|<span data-ttu-id="448c3-267">pastProjects</span><span class="sxs-lookup"><span data-stu-id="448c3-267">pastProjects</span></span>|<span data-ttu-id="448c3-268">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="448c3-268">String collection</span></span>|<span data-ttu-id="448c3-269">Список предыдущих проектов пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-269">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="448c3-270">postalCode</span><span class="sxs-lookup"><span data-stu-id="448c3-270">postalCode</span></span>|<span data-ttu-id="448c3-271">String</span><span class="sxs-lookup"><span data-stu-id="448c3-271">String</span></span>|<span data-ttu-id="448c3-p125">Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код.</span><span class="sxs-lookup"><span data-stu-id="448c3-p125">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="448c3-275">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="448c3-275">preferredLanguage</span></span>|<span data-ttu-id="448c3-276">String</span><span class="sxs-lookup"><span data-stu-id="448c3-276">String</span></span>|<span data-ttu-id="448c3-277">Предпочитаемый язык для пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-277">The preferred language for the user.</span></span> <span data-ttu-id="448c3-278">Он должен быть представлен в формате ISO 639-1, например `en-US`.</span><span class="sxs-lookup"><span data-stu-id="448c3-278">Should follow ISO 639-1 Code; for example `en-US`.</span></span>|
|<span data-ttu-id="448c3-279">responsibilities;</span><span class="sxs-lookup"><span data-stu-id="448c3-279">responsibilities</span></span>|<span data-ttu-id="448c3-280">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="448c3-280">String collection</span></span>|<span data-ttu-id="448c3-281">Список обязанностей пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-281">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="448c3-282">schools</span><span class="sxs-lookup"><span data-stu-id="448c3-282">schools</span></span>|<span data-ttu-id="448c3-283">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="448c3-283">String collection</span></span>|<span data-ttu-id="448c3-284">Список учебных заведений, которые посещал пользователь.</span><span class="sxs-lookup"><span data-stu-id="448c3-284">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="448c3-285">skills</span><span class="sxs-lookup"><span data-stu-id="448c3-285">skills</span></span>|<span data-ttu-id="448c3-286">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="448c3-286">String collection</span></span>|<span data-ttu-id="448c3-287">Список навыков пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-287">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="448c3-288">state</span><span class="sxs-lookup"><span data-stu-id="448c3-288">state</span></span>|<span data-ttu-id="448c3-289">String</span><span class="sxs-lookup"><span data-stu-id="448c3-289">String</span></span>|<span data-ttu-id="448c3-290">Область, республика, край или округ в адресе пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-290">The state or province in the user's address.</span></span>|
|<span data-ttu-id="448c3-291">streetAddress</span><span class="sxs-lookup"><span data-stu-id="448c3-291">streetAddress</span></span>|<span data-ttu-id="448c3-292">String</span><span class="sxs-lookup"><span data-stu-id="448c3-292">String</span></span>|<span data-ttu-id="448c3-293">Почтовый адрес места работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-293">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="448c3-294">surname</span><span class="sxs-lookup"><span data-stu-id="448c3-294">surname</span></span>|<span data-ttu-id="448c3-295">String</span><span class="sxs-lookup"><span data-stu-id="448c3-295">String</span></span>|<span data-ttu-id="448c3-296">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-296">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="448c3-297">usageLocation</span><span class="sxs-lookup"><span data-stu-id="448c3-297">usageLocation</span></span>|<span data-ttu-id="448c3-298">String</span><span class="sxs-lookup"><span data-stu-id="448c3-298">String</span></span>|<span data-ttu-id="448c3-299">Двухбуквенный код страны (по стандарту ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="448c3-299">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="448c3-300">Необходим для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в разных странах.</span><span class="sxs-lookup"><span data-stu-id="448c3-300">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="448c3-301">Примеры: `US`, `JP` и `GB`.</span><span class="sxs-lookup"><span data-stu-id="448c3-301">Examples include: `US`, `JP`, and `GB`.</span></span> <span data-ttu-id="448c3-302">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="448c3-302">Not nullable.</span></span>|
|<span data-ttu-id="448c3-303">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="448c3-303">userPrincipalName</span></span>|<span data-ttu-id="448c3-304">String</span><span class="sxs-lookup"><span data-stu-id="448c3-304">String</span></span>|<span data-ttu-id="448c3-p128">Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](../resources/organization.md). Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="448c3-p128">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="448c3-312">userType</span><span class="sxs-lookup"><span data-stu-id="448c3-312">userType</span></span>|<span data-ttu-id="448c3-313">String</span><span class="sxs-lookup"><span data-stu-id="448c3-313">String</span></span>|<span data-ttu-id="448c3-314">Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например `Member` и `Guest`.</span><span class="sxs-lookup"><span data-stu-id="448c3-314">A string value that can be used to classify user types in your directory, such as `Member` and `Guest`.</span></span>          |

<span data-ttu-id="448c3-315">Поскольку ресурс **пользователя** поддерживает [расширения,](/graph/extensibility-overview)вы можете использовать операцию для добавления, обновления или удаления собственных данных, определенных для приложения, в настраиваемом свойстве расширения в существующем экземпляре `PATCH` пользователя. </span><span class="sxs-lookup"><span data-stu-id="448c3-315">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **user** instance.</span></span>

> [!NOTE] 
> <span data-ttu-id="448c3-316">Следующие свойства не могут быть обновлены с помощью контекста только для приложений: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools** и **skills**.</span><span class="sxs-lookup"><span data-stu-id="448c3-316">The follow properties cannot be updated using an application-only context: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, and **skills**.</span></span>

## <a name="response"></a><span data-ttu-id="448c3-317">Отклик</span><span class="sxs-lookup"><span data-stu-id="448c3-317">Response</span></span>

<span data-ttu-id="448c3-318">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="448c3-318">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="448c3-319">Пример</span><span class="sxs-lookup"><span data-stu-id="448c3-319">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="448c3-320">Пример 1. Обновление свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="448c3-320">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="448c3-321">Запрос</span><span class="sxs-lookup"><span data-stu-id="448c3-321">Request</span></span>

<span data-ttu-id="448c3-322">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="448c3-322">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="448c3-323">HTTP</span><span class="sxs-lookup"><span data-stu-id="448c3-323">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="448c3-324">C#</span><span class="sxs-lookup"><span data-stu-id="448c3-324">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="448c3-325">JavaScript</span><span class="sxs-lookup"><span data-stu-id="448c3-325">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="448c3-326">Objective-C</span><span class="sxs-lookup"><span data-stu-id="448c3-326">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="448c3-327">Java</span><span class="sxs-lookup"><span data-stu-id="448c3-327">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="448c3-328">Отклик</span><span class="sxs-lookup"><span data-stu-id="448c3-328">Response</span></span>

<span data-ttu-id="448c3-329">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="448c3-329">The following example shows the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="448c3-330">Пример 2. Обновление свойств указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="448c3-330">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="448c3-331">Запрос</span><span class="sxs-lookup"><span data-stu-id="448c3-331">Request</span></span>

<span data-ttu-id="448c3-332">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="448c3-332">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="448c3-333">HTTP</span><span class="sxs-lookup"><span data-stu-id="448c3-333">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="448c3-334">C#</span><span class="sxs-lookup"><span data-stu-id="448c3-334">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="448c3-335">JavaScript</span><span class="sxs-lookup"><span data-stu-id="448c3-335">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="448c3-336">Objective-C</span><span class="sxs-lookup"><span data-stu-id="448c3-336">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="448c3-337">Java</span><span class="sxs-lookup"><span data-stu-id="448c3-337">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="448c3-338">Отклик</span><span class="sxs-lookup"><span data-stu-id="448c3-338">Response</span></span>

<span data-ttu-id="448c3-339">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="448c3-339">The following example shows the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-the-passwordprofile-of-a-user-to-reset-their-password"></a><span data-ttu-id="448c3-340">Пример 3. Обновление passwordProfile пользователя для сброса его пароля</span><span class="sxs-lookup"><span data-stu-id="448c3-340">Example 3: Update the passwordProfile of a user to reset their password</span></span>

<span data-ttu-id="448c3-341">В следующем примере показан запрос, который сбрасывает пароль другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="448c3-341">The following example shows a request that resets the password of another user.</span></span>

#### <a name="request"></a><span data-ttu-id="448c3-342">Запрос</span><span class="sxs-lookup"><span data-stu-id="448c3-342">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="448c3-343">HTTP</span><span class="sxs-lookup"><span data-stu-id="448c3-343">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user_passwordProfile"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
  "passwordProfile": {
    "forceChangePasswordNextSignIn": false,
    "password": "xWwvJ]6NMw+bWH-d"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="448c3-344">C#</span><span class="sxs-lookup"><span data-stu-id="448c3-344">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-passwordprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="448c3-345">JavaScript</span><span class="sxs-lookup"><span data-stu-id="448c3-345">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-passwordprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="448c3-346">Objective-C</span><span class="sxs-lookup"><span data-stu-id="448c3-346">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-passwordprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="448c3-347">Java</span><span class="sxs-lookup"><span data-stu-id="448c3-347">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-passwordprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="448c3-348">Отклик</span><span class="sxs-lookup"><span data-stu-id="448c3-348">Response</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="448c3-349">См. также</span><span class="sxs-lookup"><span data-stu-id="448c3-349">See also</span></span>

- [<span data-ttu-id="448c3-350">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="448c3-350">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="448c3-351">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="448c3-351">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="448c3-352">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="448c3-352">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
