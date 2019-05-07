---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: adc4bf3854f11141bb29c91035fde92bdf9c5c82
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637068"
---
# <a name="update-user"></a><span data-ttu-id="74d75-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="74d75-103">Update user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74d75-104">Обновление свойств объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="74d75-104">Update the properties of a user object.</span></span>
## <a name="permissions"></a><span data-ttu-id="74d75-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74d75-105">Permissions</span></span>
<span data-ttu-id="74d75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74d75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74d75-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74d75-108">Permission type</span></span>      | <span data-ttu-id="74d75-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74d75-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74d75-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74d75-110">Delegated (work or school account)</span></span> | <span data-ttu-id="74d75-111">User. ReadWrite, User. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="74d75-111">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="74d75-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74d75-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74d75-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74d75-113">User.ReadWrite</span></span>    |
|<span data-ttu-id="74d75-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74d75-114">Application</span></span> | <span data-ttu-id="74d75-115">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74d75-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74d75-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74d75-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```
## <a name="request-headers"></a><span data-ttu-id="74d75-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74d75-117">Request headers</span></span>
| <span data-ttu-id="74d75-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74d75-118">Header</span></span>       | <span data-ttu-id="74d75-119">Значение</span><span class="sxs-lookup"><span data-stu-id="74d75-119">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="74d75-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74d75-120">Authorization</span></span>  | <span data-ttu-id="74d75-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74d75-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="74d75-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="74d75-123">Content-Type</span></span>  | <span data-ttu-id="74d75-124">application/json</span><span class="sxs-lookup"><span data-stu-id="74d75-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="74d75-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74d75-125">Request body</span></span>
<span data-ttu-id="74d75-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="74d75-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="74d75-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="74d75-129">Property</span></span>     | <span data-ttu-id="74d75-130">Тип</span><span class="sxs-lookup"><span data-stu-id="74d75-130">Type</span></span>   |<span data-ttu-id="74d75-131">Описание</span><span class="sxs-lookup"><span data-stu-id="74d75-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74d75-132">aboutMe</span><span class="sxs-lookup"><span data-stu-id="74d75-132">aboutMe</span></span>|<span data-ttu-id="74d75-133">String</span><span class="sxs-lookup"><span data-stu-id="74d75-133">String</span></span>|<span data-ttu-id="74d75-134">Свободное текстовое поле, где пользователь может рассказать о себе.</span><span class="sxs-lookup"><span data-stu-id="74d75-134">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="74d75-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="74d75-135">accountEnabled</span></span>|<span data-ttu-id="74d75-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="74d75-136">Boolean</span></span>| <span data-ttu-id="74d75-p104">Значение **true** указывает, что учетная запись включена. В противном случае используется значение **false**. Это свойство обязательно указывать при создании пользователя. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="74d75-p104">**true** if the account is enabled; otherwise, **false**. This property is required when a user is created. Supports $filter.</span></span>    |
|<span data-ttu-id="74d75-140">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="74d75-140">assignedLicenses</span></span>|<span data-ttu-id="74d75-141">Коллекция [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="74d75-141">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="74d75-p105">Лицензии, назначенные пользователю. Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="74d75-p105">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="74d75-144">birthday</span><span class="sxs-lookup"><span data-stu-id="74d75-144">birthday</span></span>|<span data-ttu-id="74d75-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74d75-145">DateTimeOffset</span></span>|<span data-ttu-id="74d75-p106">День рождения пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="74d75-p106">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="74d75-149">city</span><span class="sxs-lookup"><span data-stu-id="74d75-149">city</span></span>|<span data-ttu-id="74d75-150">String</span><span class="sxs-lookup"><span data-stu-id="74d75-150">String</span></span>|<span data-ttu-id="74d75-p107">Город, в котором находится пользователь. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="74d75-p107">The city in which the user is located. Supports $filter.</span></span>|
|<span data-ttu-id="74d75-153">country</span><span class="sxs-lookup"><span data-stu-id="74d75-153">country</span></span>|<span data-ttu-id="74d75-154">String</span><span class="sxs-lookup"><span data-stu-id="74d75-154">String</span></span>|<span data-ttu-id="74d75-p108">Страна или регион, в котором находится пользователь, например "США" или "Соединенное Королевство". Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="74d75-p108">The country/region in which the user is located; for example, “US” or “UK”. Supports $filter.</span></span>|
|<span data-ttu-id="74d75-157">department</span><span class="sxs-lookup"><span data-stu-id="74d75-157">department</span></span>|<span data-ttu-id="74d75-158">String</span><span class="sxs-lookup"><span data-stu-id="74d75-158">String</span></span>|<span data-ttu-id="74d75-p109">Название отдела, в котором работает пользователь. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="74d75-p109">The name for the department in which the user works. Supports $filter.</span></span>|
|<span data-ttu-id="74d75-161">displayName</span><span class="sxs-lookup"><span data-stu-id="74d75-161">displayName</span></span>|<span data-ttu-id="74d75-162">Строка</span><span class="sxs-lookup"><span data-stu-id="74d75-162">String</span></span>|<span data-ttu-id="74d75-p110">Отображаемое имя пользователя в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="74d75-p110">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="74d75-167">employeeId</span><span class="sxs-lookup"><span data-stu-id="74d75-167">employeeId</span></span>|<span data-ttu-id="74d75-168">String</span><span class="sxs-lookup"><span data-stu-id="74d75-168">String</span></span>|<span data-ttu-id="74d75-169">Идентификатор сотрудника, назначенный пользователю организацией.</span><span class="sxs-lookup"><span data-stu-id="74d75-169">The employee identifier assigned to the user by the organization.</span></span> <span data-ttu-id="74d75-170">Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="74d75-170">Supports $filter.</span></span>|
|<span data-ttu-id="74d75-171">givenName</span><span class="sxs-lookup"><span data-stu-id="74d75-171">givenName</span></span>|<span data-ttu-id="74d75-172">String</span><span class="sxs-lookup"><span data-stu-id="74d75-172">String</span></span>|<span data-ttu-id="74d75-p112">Простое имя пользователя. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="74d75-p112">The given name (first name) of the user. Supports $filter.</span></span>|
|<span data-ttu-id="74d75-175">hireDate</span><span class="sxs-lookup"><span data-stu-id="74d75-175">hireDate</span></span>|<span data-ttu-id="74d75-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74d75-176">DateTimeOffset</span></span>|<span data-ttu-id="74d75-p113">Дата найма пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="74d75-p113">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="74d75-180">interests</span><span class="sxs-lookup"><span data-stu-id="74d75-180">interests</span></span>|<span data-ttu-id="74d75-181">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="74d75-181">String collection</span></span>|<span data-ttu-id="74d75-182">Список интересов пользователя.</span><span class="sxs-lookup"><span data-stu-id="74d75-182">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="74d75-183">jobTitle</span><span class="sxs-lookup"><span data-stu-id="74d75-183">jobTitle</span></span>|<span data-ttu-id="74d75-184">String</span><span class="sxs-lookup"><span data-stu-id="74d75-184">String</span></span>|<span data-ttu-id="74d75-p114">Должность пользователя. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="74d75-p114">The user’s job title. Supports $filter.</span></span>|
|<span data-ttu-id="74d75-187">mailNickname</span><span class="sxs-lookup"><span data-stu-id="74d75-187">mailNickname</span></span>|<span data-ttu-id="74d75-188">String</span><span class="sxs-lookup"><span data-stu-id="74d75-188">String</span></span>|<span data-ttu-id="74d75-p115">Почтовый псевдоним для пользователя. Это свойство должно быть указано при создании пользователя. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="74d75-p115">The mail alias for the user. This property must be specified when a user is created. Supports $filter.</span></span>|
|<span data-ttu-id="74d75-192">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="74d75-192">mobilePhone</span></span>|<span data-ttu-id="74d75-193">String</span><span class="sxs-lookup"><span data-stu-id="74d75-193">String</span></span>|<span data-ttu-id="74d75-194">Основной сотовый телефон пользователя.</span><span class="sxs-lookup"><span data-stu-id="74d75-194">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="74d75-195">mySite</span><span class="sxs-lookup"><span data-stu-id="74d75-195">mySite</span></span>|<span data-ttu-id="74d75-196">String</span><span class="sxs-lookup"><span data-stu-id="74d75-196">String</span></span>|<span data-ttu-id="74d75-197">URL-адрес личного сайта пользователя.</span><span class="sxs-lookup"><span data-stu-id="74d75-197">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="74d75-198">officeLocation</span><span class="sxs-lookup"><span data-stu-id="74d75-198">officeLocation</span></span>|<span data-ttu-id="74d75-199">String</span><span class="sxs-lookup"><span data-stu-id="74d75-199">String</span></span>|<span data-ttu-id="74d75-200">Расположение офиса на месте работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="74d75-200">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="74d75-201">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="74d75-201">onPremisesImmutableId</span></span>|<span data-ttu-id="74d75-202">String</span><span class="sxs-lookup"><span data-stu-id="74d75-202">String</span></span>|<span data-ttu-id="74d75-p116">Это свойство используется для сопоставления локальной учетной записи Active Directory с объектом пользователя Azure AD. Его необходимо указывать при создании учетной записи пользователя в Graph, если в качестве свойства **userPrincipalName** (имени участника-пользователя) используется федеративный домен. **Важно!** В этом свойстве не допускается использование символов **$** и **_**. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="74d75-p116">This property is used to associate an on-premises Active Directory user account to their Azure AD user object. This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property. **Important:** The **$** and **_** characters cannot be used when specifying this property. Supports $filter.</span></span>                            |
|<span data-ttu-id="74d75-207">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="74d75-207">passwordPolicies</span></span>|<span data-ttu-id="74d75-208">String</span><span class="sxs-lookup"><span data-stu-id="74d75-208">String</span></span>|<span data-ttu-id="74d75-p117">Задает политики паролей для пользователя. Это свойство представляет собой перечисление с единственным возможным значением — "DisableStrongPassword". Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение "DisablePasswordExpiration". Эти значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="74d75-p117">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="74d75-213">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="74d75-213">passwordProfile</span></span>|[<span data-ttu-id="74d75-214">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="74d75-214">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="74d75-p118">Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="74d75-p118">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="74d75-220">pastProjects</span><span class="sxs-lookup"><span data-stu-id="74d75-220">pastProjects</span></span>|<span data-ttu-id="74d75-221">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="74d75-221">String collection</span></span>|<span data-ttu-id="74d75-222">Список предыдущих проектов пользователя.</span><span class="sxs-lookup"><span data-stu-id="74d75-222">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="74d75-223">postalCode</span><span class="sxs-lookup"><span data-stu-id="74d75-223">postalCode</span></span>|<span data-ttu-id="74d75-224">String</span><span class="sxs-lookup"><span data-stu-id="74d75-224">String</span></span>|<span data-ttu-id="74d75-p119">Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код.</span><span class="sxs-lookup"><span data-stu-id="74d75-p119">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="74d75-228">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="74d75-228">preferredLanguage</span></span>|<span data-ttu-id="74d75-229">String</span><span class="sxs-lookup"><span data-stu-id="74d75-229">String</span></span>|<span data-ttu-id="74d75-p120">Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1, например "ru-RU".</span><span class="sxs-lookup"><span data-stu-id="74d75-p120">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="74d75-232">responsibilities</span><span class="sxs-lookup"><span data-stu-id="74d75-232">responsibilities</span></span>|<span data-ttu-id="74d75-233">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="74d75-233">String collection</span></span>|<span data-ttu-id="74d75-234">Список обязанностей пользователя.</span><span class="sxs-lookup"><span data-stu-id="74d75-234">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="74d75-235">schools</span><span class="sxs-lookup"><span data-stu-id="74d75-235">schools</span></span>|<span data-ttu-id="74d75-236">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="74d75-236">String collection</span></span>|<span data-ttu-id="74d75-237">Список учебных заведений, которые посещал пользователь.</span><span class="sxs-lookup"><span data-stu-id="74d75-237">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="74d75-238">skills</span><span class="sxs-lookup"><span data-stu-id="74d75-238">skills</span></span>|<span data-ttu-id="74d75-239">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="74d75-239">String collection</span></span>|<span data-ttu-id="74d75-240">Список навыков пользователя.</span><span class="sxs-lookup"><span data-stu-id="74d75-240">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="74d75-241">state</span><span class="sxs-lookup"><span data-stu-id="74d75-241">state</span></span>|<span data-ttu-id="74d75-242">Строка</span><span class="sxs-lookup"><span data-stu-id="74d75-242">String</span></span>|<span data-ttu-id="74d75-p121">Область, республика, край или округ в адресе пользователя. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="74d75-p121">The state or province in the user's address. Supports $filter.</span></span>|
|<span data-ttu-id="74d75-245">streetAddress</span><span class="sxs-lookup"><span data-stu-id="74d75-245">streetAddress</span></span>|<span data-ttu-id="74d75-246">String</span><span class="sxs-lookup"><span data-stu-id="74d75-246">String</span></span>|<span data-ttu-id="74d75-247">Почтовый адрес места работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="74d75-247">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="74d75-248">surname</span><span class="sxs-lookup"><span data-stu-id="74d75-248">surname</span></span>|<span data-ttu-id="74d75-249">String</span><span class="sxs-lookup"><span data-stu-id="74d75-249">String</span></span>|<span data-ttu-id="74d75-p122">Фамилия пользователя. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="74d75-p122">The user's surname (family name or last name). Supports $filter.</span></span>|
|<span data-ttu-id="74d75-252">usageLocation</span><span class="sxs-lookup"><span data-stu-id="74d75-252">usageLocation</span></span>|<span data-ttu-id="74d75-253">String</span><span class="sxs-lookup"><span data-stu-id="74d75-253">String</span></span>|<span data-ttu-id="74d75-p123">Двухбуквенный код страны (по стандарту ISO 3166). Необходим для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в разных странах.  Примеры: "RU", "JP" и "GB". Значение null не допускается. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="74d75-p123">A two letter country code (ISO standard 3166). Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.  Examples include: "US", "JP", and "GB". Not nullable. Supports $filter.</span></span>|
|<span data-ttu-id="74d75-259">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="74d75-259">userPrincipalName</span></span>|<span data-ttu-id="74d75-260">String</span><span class="sxs-lookup"><span data-stu-id="74d75-260">String</span></span>|<span data-ttu-id="74d75-p124">Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](../resources/organization.md). Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="74d75-p124">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="74d75-268">userType</span><span class="sxs-lookup"><span data-stu-id="74d75-268">userType</span></span>|<span data-ttu-id="74d75-269">String</span><span class="sxs-lookup"><span data-stu-id="74d75-269">String</span></span>|<span data-ttu-id="74d75-p125">Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость". Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="74d75-p125">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”. Supports $filter.</span></span>          |

<span data-ttu-id="74d75-272">Так как ресурс **User** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в пользовательских свойствах расширения в существующем **пользовательском** экземпляре.</span><span class="sxs-lookup"><span data-stu-id="74d75-272">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **user** instance.</span></span>

## <a name="response"></a><span data-ttu-id="74d75-273">Отклик</span><span class="sxs-lookup"><span data-stu-id="74d75-273">Response</span></span>

<span data-ttu-id="74d75-274">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="74d75-274">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="74d75-275">Пример</span><span class="sxs-lookup"><span data-stu-id="74d75-275">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74d75-276">Запрос</span><span class="sxs-lookup"><span data-stu-id="74d75-276">Request</span></span>
<span data-ttu-id="74d75-277">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74d75-277">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/beta/me
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-19T10:37:00Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value"
}
```
##### <a name="response"></a><span data-ttu-id="74d75-278">Отклик</span><span class="sxs-lookup"><span data-stu-id="74d75-278">Response</span></span>
<span data-ttu-id="74d75-p126">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74d75-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="74d75-282">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="74d75-282">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="74d75-283">Языках</span><span class="sxs-lookup"><span data-stu-id="74d75-283">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74d75-284">Язык</span><span class="sxs-lookup"><span data-stu-id="74d75-284">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="74d75-285">См. также</span><span class="sxs-lookup"><span data-stu-id="74d75-285">See also</span></span>

- [<span data-ttu-id="74d75-286">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="74d75-286">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="74d75-287">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="74d75-287">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="74d75-288">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="74d75-288">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
    "Error: /api-reference/beta/api/user-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
