---
title: Создание educationUser
description: Создание нового объекта educationUser.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b26e0530fd4beea6d2f604fa46f891e154fefa61
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232286"
---
# <a name="create-educationuser"></a><span data-ttu-id="72027-103">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="72027-103">Create educationUser</span></span>

<span data-ttu-id="72027-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72027-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="72027-105">Создание нового [объекта educationUser.](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="72027-105">Create a new [educationUser](../resources/educationuser.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="72027-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72027-106">Permissions</span></span>

<span data-ttu-id="72027-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72027-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72027-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72027-109">Permission type</span></span>                        | <span data-ttu-id="72027-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72027-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="72027-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72027-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="72027-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72027-112">Not supported.</span></span>                              |
| <span data-ttu-id="72027-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72027-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72027-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72027-114">Not supported.</span></span>                              |
| <span data-ttu-id="72027-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="72027-115">Application</span></span>                            | <span data-ttu-id="72027-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72027-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="72027-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72027-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /education/users
```

## <a name="request-headers"></a><span data-ttu-id="72027-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72027-118">Request headers</span></span>

| <span data-ttu-id="72027-119">Имя</span><span class="sxs-lookup"><span data-stu-id="72027-119">Name</span></span>          | <span data-ttu-id="72027-120">Описание</span><span class="sxs-lookup"><span data-stu-id="72027-120">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="72027-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72027-121">Authorization</span></span> | <span data-ttu-id="72027-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72027-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="72027-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72027-124">Content-Type</span></span>  | <span data-ttu-id="72027-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72027-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72027-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72027-127">Request body</span></span>

<span data-ttu-id="72027-128">В теле запроса поставляем представление JSON объекта [educationUser.](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="72027-128">In the request body, supply a JSON representation of the [educationUser](../resources/educationuser.md) object.</span></span>

<span data-ttu-id="72027-129">В следующей таблице показаны свойства, необходимые при создании [educationUser.](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="72027-129">The following table shows the properties that are required when you create the [educationUser](../resources/educationuser.md).</span></span>

| <span data-ttu-id="72027-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="72027-130">Property</span></span>             | <span data-ttu-id="72027-131">Тип</span><span class="sxs-lookup"><span data-stu-id="72027-131">Type</span></span>                                                               | <span data-ttu-id="72027-132">Описание</span><span class="sxs-lookup"><span data-stu-id="72027-132">Description</span></span>                                                                                                                                                                                                                                                                                                                                                 |
| :------------------- | :----------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="72027-133">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="72027-133">accountEnabled</span></span>       | <span data-ttu-id="72027-134">Логический</span><span class="sxs-lookup"><span data-stu-id="72027-134">Boolean</span></span>                                                            | <span data-ttu-id="72027-135">Если учетная запись обеспечена — значение **true**, в противном случае — **false**.</span><span class="sxs-lookup"><span data-stu-id="72027-135">**True** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="72027-136">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="72027-136">This property is required when a user is created.</span></span> <span data-ttu-id="72027-137">Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="72027-137">Supports $filter.</span></span>                                                                                                                                                                                                                               |
| <span data-ttu-id="72027-138">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="72027-138">assignedLicenses</span></span>     | <span data-ttu-id="72027-139">Коллекция [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="72027-139">[assignedLicense](../resources/assignedlicense.md) collection</span></span>      | <span data-ttu-id="72027-p105">Лицензии, назначенные пользователю. Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="72027-p105">The licenses that are assigned to the user. Not nullable.</span></span>                                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="72027-142">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="72027-142">assignedPlans</span></span>        | <span data-ttu-id="72027-143">Коллекция [assignedPlan](../resources/assignedplan.md)</span><span class="sxs-lookup"><span data-stu-id="72027-143">[assignedPlan](../resources/assignedplan.md) collection</span></span>            | <span data-ttu-id="72027-p106">Планы, назначенные пользователю. Только для чтения. Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="72027-p106">The plans that are assigned to the user. Read-only. Not nullable.</span></span>                                                                                                                                                                                                                                                                                           |
| <span data-ttu-id="72027-147">businessPhones</span><span class="sxs-lookup"><span data-stu-id="72027-147">businessPhones</span></span>       | <span data-ttu-id="72027-148">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="72027-148">String collection</span></span>                                                  | <span data-ttu-id="72027-149">Номера телефонов пользователя.</span><span class="sxs-lookup"><span data-stu-id="72027-149">The telephone numbers for the user.</span></span> <span data-ttu-id="72027-150">**Примечание.** Несмотря на то что это коллекция строк, для этого свойства можно задать только один номер.</span><span class="sxs-lookup"><span data-stu-id="72027-150">**Note:** Although this is a string collection, only one number can be set for this property.</span></span>                                                                                                                                                                                                                           |
| <span data-ttu-id="72027-151">createdBy</span><span class="sxs-lookup"><span data-stu-id="72027-151">createdBy</span></span>            | [<span data-ttu-id="72027-152">identitySet</span><span class="sxs-lookup"><span data-stu-id="72027-152">identitySet</span></span>](../resources/identityset.md)                         | <span data-ttu-id="72027-153">Объект, который создал пользователя.</span><span class="sxs-lookup"><span data-stu-id="72027-153">Entity who created the user.</span></span>                                                                                                                                                                                                                                                                                                                                |
| <span data-ttu-id="72027-154">department</span><span class="sxs-lookup"><span data-stu-id="72027-154">department</span></span>           | <span data-ttu-id="72027-155">String</span><span class="sxs-lookup"><span data-stu-id="72027-155">String</span></span>                                                             | <span data-ttu-id="72027-p108">Название отдела, в котором работает пользователь. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="72027-p108">The name for the department in which the user works. Supports $filter.</span></span>                                                                                                                                                                                                                                                                                      |
| <span data-ttu-id="72027-158">displayName</span><span class="sxs-lookup"><span data-stu-id="72027-158">displayName</span></span>          | <span data-ttu-id="72027-159">String</span><span class="sxs-lookup"><span data-stu-id="72027-159">String</span></span>                                                             | <span data-ttu-id="72027-160">Имя пользователя, отображаемое в адресной книге.</span><span class="sxs-lookup"><span data-stu-id="72027-160">The name displayed in the address book for the user.</span></span> <span data-ttu-id="72027-161">Обычно это сочетание имени, отчества и фамилии пользователя.</span><span class="sxs-lookup"><span data-stu-id="72027-161">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="72027-162">Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении.</span><span class="sxs-lookup"><span data-stu-id="72027-162">This property is required when a user is created and it cannot be cleared during updates.</span></span> <span data-ttu-id="72027-163">Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="72027-163">Supports $filter and $orderby.</span></span>                                                                                      |
| <span data-ttu-id="72027-164">externalSource</span><span class="sxs-lookup"><span data-stu-id="72027-164">externalSource</span></span>       | <span data-ttu-id="72027-165">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="72027-165">educationExternalSource</span></span>                                            | <span data-ttu-id="72027-166">Источник для создания пользователя.</span><span class="sxs-lookup"><span data-stu-id="72027-166">Where this user was created from.</span></span> <span data-ttu-id="72027-167">Возможные значения: `sis`, `manual`.</span><span class="sxs-lookup"><span data-stu-id="72027-167">Possible values are: `sis`, `manual`.</span></span>                                                                                                                                                                                                                                                                                     |
| <span data-ttu-id="72027-168">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="72027-168">externalSourceDetail</span></span> | <span data-ttu-id="72027-169">Строка</span><span class="sxs-lookup"><span data-stu-id="72027-169">String</span></span>                                                             | <span data-ttu-id="72027-170">Имя внешнего источника, из которого были созданы эти ресурсы.</span><span class="sxs-lookup"><span data-stu-id="72027-170">The name of the external source this resources was generated from.</span></span>                                                                                                                                                                                                                                                                                          |
| <span data-ttu-id="72027-171">givenName</span><span class="sxs-lookup"><span data-stu-id="72027-171">givenName</span></span>            | <span data-ttu-id="72027-172">String</span><span class="sxs-lookup"><span data-stu-id="72027-172">String</span></span>                                                             | <span data-ttu-id="72027-p111">Простое имя пользователя. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="72027-p111">The given name (first name) of the user. Supports $filter.</span></span>                                                                                                                                                                                                                                                                                                  |
| <span data-ttu-id="72027-175">mail</span><span class="sxs-lookup"><span data-stu-id="72027-175">mail</span></span>                 | <span data-ttu-id="72027-176">String</span><span class="sxs-lookup"><span data-stu-id="72027-176">String</span></span>                                                             | <span data-ttu-id="72027-177">SMTP-адрес пользователя, например "victor@contoso.onmicrosoft.com".</span><span class="sxs-lookup"><span data-stu-id="72027-177">The SMTP address for the user; for example, "jeff@contoso.onmicrosoft.com".</span></span> <span data-ttu-id="72027-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72027-178">Read-Only.</span></span> <span data-ttu-id="72027-179">Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="72027-179">Supports $filter.</span></span>                                                                                                                                                                                                                                                    |
| <span data-ttu-id="72027-180">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="72027-180">mailingAddress</span></span>       | [<span data-ttu-id="72027-181">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="72027-181">physicalAddress</span></span>](../resources/physicaladdress.md)                 | <span data-ttu-id="72027-182">Почтовый адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="72027-182">Mail address of user.</span></span>                                                                                                                                                                                                                                                                                                                                       |
| <span data-ttu-id="72027-183">mailNickname</span><span class="sxs-lookup"><span data-stu-id="72027-183">mailNickname</span></span>         | <span data-ttu-id="72027-184">String</span><span class="sxs-lookup"><span data-stu-id="72027-184">String</span></span>                                                             | <span data-ttu-id="72027-p113">Почтовый псевдоним для пользователя. Это свойство должно быть указано при создании пользователя. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="72027-p113">The mail alias for the user. This property must be specified when a user is created. Supports $filter.</span></span>                                                                                                                                                                                                                                                      |
| <span data-ttu-id="72027-188">middleName</span><span class="sxs-lookup"><span data-stu-id="72027-188">middleName</span></span>           | <span data-ttu-id="72027-189">String</span><span class="sxs-lookup"><span data-stu-id="72027-189">String</span></span>                                                             | <span data-ttu-id="72027-190">Отчество пользователя.</span><span class="sxs-lookup"><span data-stu-id="72027-190">The middle name of user.</span></span>                                                                                                                                                                                                                                                                                                                                    |
| <span data-ttu-id="72027-191">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="72027-191">mobilePhone</span></span>          | <span data-ttu-id="72027-192">String</span><span class="sxs-lookup"><span data-stu-id="72027-192">String</span></span>                                                             | <span data-ttu-id="72027-193">Основной сотовый телефон пользователя.</span><span class="sxs-lookup"><span data-stu-id="72027-193">The primary cellular telephone number for the user.</span></span>                                                                                                                                                                                                                                                                                                         |
| <span data-ttu-id="72027-194">onPremisesInfo</span><span class="sxs-lookup"><span data-stu-id="72027-194">onPremisesInfo</span></span>       | [<span data-ttu-id="72027-195">educationOnPremisesInfo</span><span class="sxs-lookup"><span data-stu-id="72027-195">educationOnPremisesInfo</span></span>](../resources/educationonpremisesinfo.md) | <span data-ttu-id="72027-196">Дополнительные сведения, используемые для связи пользователя AAD с его аналогом Active Directory.</span><span class="sxs-lookup"><span data-stu-id="72027-196">Additional information used to associate the AAD user with it's Active Directory counterpart.</span></span>                                                                                                                                                                                                                                                               |
| <span data-ttu-id="72027-197">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="72027-197">passwordPolicies</span></span>     | <span data-ttu-id="72027-198">String</span><span class="sxs-lookup"><span data-stu-id="72027-198">String</span></span>                                                             | <span data-ttu-id="72027-199">Задает политики паролей для пользователя.</span><span class="sxs-lookup"><span data-stu-id="72027-199">Specifies password policies for the user.</span></span> <span data-ttu-id="72027-200">Это свойство представляет собой перечисление с возможным значением DisableStrongPassword. Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="72027-200">This value is an enumeration with one possible value being "DisableStrongPassword", which allows weaker passwords than the default policy to be specified.</span></span> <span data-ttu-id="72027-201">Вы также можете указать значение DisablePasswordExpiration.</span><span class="sxs-lookup"><span data-stu-id="72027-201">"DisablePasswordExpiration" can also be specified.</span></span> <span data-ttu-id="72027-202">Два значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword".</span><span class="sxs-lookup"><span data-stu-id="72027-202">The two can be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span> |
| <span data-ttu-id="72027-203">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="72027-203">passwordProfile</span></span>      | [<span data-ttu-id="72027-204">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="72027-204">passwordProfile</span></span>](../resources/passwordprofile.md)                 | <span data-ttu-id="72027-205">Задает профиль пароля для пользователя.</span><span class="sxs-lookup"><span data-stu-id="72027-205">Specifies the password profile for the user.</span></span> <span data-ttu-id="72027-206">Профиль содержит пароль пользователя.</span><span class="sxs-lookup"><span data-stu-id="72027-206">The profile contains the user's password.</span></span> <span data-ttu-id="72027-207">Это свойство обязательно указывать при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="72027-207">This property is required when a user is created.</span></span> <span data-ttu-id="72027-208">Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**.</span><span class="sxs-lookup"><span data-stu-id="72027-208">The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property.</span></span> <span data-ttu-id="72027-209">По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="72027-209">By default, a strong password is required.</span></span>                                                        |
| <span data-ttu-id="72027-210">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="72027-210">preferredLanguage</span></span>    | <span data-ttu-id="72027-211">String</span><span class="sxs-lookup"><span data-stu-id="72027-211">String</span></span>                                                             | <span data-ttu-id="72027-212">Предпочитаемый язык для пользователя.</span><span class="sxs-lookup"><span data-stu-id="72027-212">The preferred language for the user.</span></span> <span data-ttu-id="72027-213">Он должен быть представлен в формате ISO 639-1. Пример: "ru-RU".</span><span class="sxs-lookup"><span data-stu-id="72027-213">Should follow ISO 639-1 Code; for example, "en-US".</span></span>                                                                                                                                                                                                                                                                    |
| <span data-ttu-id="72027-214">primaryRole</span><span class="sxs-lookup"><span data-stu-id="72027-214">primaryRole</span></span>          | <span data-ttu-id="72027-215">educationUserRole</span><span class="sxs-lookup"><span data-stu-id="72027-215">educationUserRole</span></span>                                                  | <span data-ttu-id="72027-216">Роль по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="72027-216">Default role for a user.</span></span> <span data-ttu-id="72027-217">Роль пользователя для отдельного курса может отличаться.</span><span class="sxs-lookup"><span data-stu-id="72027-217">The user's role might be different in an individual class.</span></span> <span data-ttu-id="72027-218">Возможные значения: `student`, `teacher`, `none`.</span><span class="sxs-lookup"><span data-stu-id="72027-218">Possible values are: `student`, `teacher`, `none`.</span></span>                                                                                                                                                                                                                      |
| <span data-ttu-id="72027-219">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="72027-219">provisionedPlans</span></span>     | <span data-ttu-id="72027-220">Коллекция [provisionedPlan](../resources/provisionedplan.md)</span><span class="sxs-lookup"><span data-stu-id="72027-220">[provisionedPlan](../resources/provisionedplan.md) collection</span></span>      | <span data-ttu-id="72027-p118">Планы, подготовленные для пользователя. Только для чтения. Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="72027-p118">The plans that are provisioned for the user. Read-only. Not nullable.</span></span>                                                                                                                                                                                                                                                                                       |
| <span data-ttu-id="72027-224">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="72027-224">residenceAddress</span></span>     | [<span data-ttu-id="72027-225">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="72027-225">physicalAddress</span></span>](../resources/physicaladdress.md)                 | <span data-ttu-id="72027-226">Адрес проживания пользователя.</span><span class="sxs-lookup"><span data-stu-id="72027-226">Address where user lives.</span></span>                                                                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="72027-227">student</span><span class="sxs-lookup"><span data-stu-id="72027-227">student</span></span>              | [<span data-ttu-id="72027-228">educationStudent</span><span class="sxs-lookup"><span data-stu-id="72027-228">educationStudent</span></span>](../resources/educationstudent.md)               | <span data-ttu-id="72027-229">Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.</span><span class="sxs-lookup"><span data-stu-id="72027-229">If the primary role is student, this block will contain student specific data.</span></span>                                                                                                                                                                                                                                                                              |
| <span data-ttu-id="72027-230">surname</span><span class="sxs-lookup"><span data-stu-id="72027-230">surname</span></span>              | <span data-ttu-id="72027-231">String</span><span class="sxs-lookup"><span data-stu-id="72027-231">String</span></span>                                                             | <span data-ttu-id="72027-p119">Фамилия пользователя. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="72027-p119">The user's surname (family name or last name). Supports $filter.</span></span>                                                                                                                                                                                                                                                                                            |
| <span data-ttu-id="72027-234">teacher</span><span class="sxs-lookup"><span data-stu-id="72027-234">teacher</span></span>              | [<span data-ttu-id="72027-235">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="72027-235">educationTeacher</span></span>](../resources/educationteacher.md)               | <span data-ttu-id="72027-236">Если основной ролью является учитель, этот блок будет содержать определенные данные учителя.</span><span class="sxs-lookup"><span data-stu-id="72027-236">If the primary role is teacher, this block will contain teacher specific data.</span></span>                                                                                                                                                                                                                                                                              |
| <span data-ttu-id="72027-237">usageLocation</span><span class="sxs-lookup"><span data-stu-id="72027-237">usageLocation</span></span>        | <span data-ttu-id="72027-238">String</span><span class="sxs-lookup"><span data-stu-id="72027-238">String</span></span>                                                             | <span data-ttu-id="72027-239">Двухбуквенный код страны (по стандарту ISO 3166).</span><span class="sxs-lookup"><span data-stu-id="72027-239">A two-letter country code (ISO standard 3166).</span></span> <span data-ttu-id="72027-240">Свойство необходимо указывать для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в странах или регионах.</span><span class="sxs-lookup"><span data-stu-id="72027-240">Required for users who will be assigned licenses due to a legal requirement to check for availability of services in countries or regions.</span></span> <span data-ttu-id="72027-241">Примеры: "RU", "JP", "GB".</span><span class="sxs-lookup"><span data-stu-id="72027-241">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="72027-242">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="72027-242">Not nullable.</span></span> <span data-ttu-id="72027-243">Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="72027-243">Supports $filter.</span></span>                                                                                           |
| <span data-ttu-id="72027-244">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="72027-244">userPrincipalName</span></span>    | <span data-ttu-id="72027-245">String</span><span class="sxs-lookup"><span data-stu-id="72027-245">String</span></span>                                                             | <span data-ttu-id="72027-246">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="72027-246">The user principal name (UPN) of the user.</span></span>                                                                                                                                                                                                                                                                                                                  |
| <span data-ttu-id="72027-247">userType</span><span class="sxs-lookup"><span data-stu-id="72027-247">userType</span></span>             | <span data-ttu-id="72027-248">String</span><span class="sxs-lookup"><span data-stu-id="72027-248">String</span></span>                                                             | <span data-ttu-id="72027-p121">Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость". Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="72027-p121">A string value that can be used to classify user types in your directory, such as "Member" and "Guest". Supports $filter.</span></span>                                                                                                                                                                                                                                   |

## <a name="response"></a><span data-ttu-id="72027-251">Отклик</span><span class="sxs-lookup"><span data-stu-id="72027-251">Response</span></span>

<span data-ttu-id="72027-252">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="72027-252">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72027-253">Примеры</span><span class="sxs-lookup"><span data-stu-id="72027-253">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72027-254">Запрос</span><span class="sxs-lookup"><span data-stu-id="72027-254">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/users
Content-Type: application/json
Content-length: 1585

{
  "@odata.type": "#microsoft.graph.educationUser",
  "primaryRole": "String",
  "middleName": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "accountEnabled": "Boolean",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "showInAddressList": "Boolean",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo"
  }
}
```

### <a name="response"></a><span data-ttu-id="72027-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="72027-255">Response</span></span>

> <span data-ttu-id="72027-256">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="72027-256">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationUser",
  "id": "90eedea1-dea1-90ee-a1de-ee90a1deee90",
  "primaryRole": "String",
  "middleName": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "accountEnabled": "Boolean",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "showInAddressList": "Boolean",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo"
  }
}
```
