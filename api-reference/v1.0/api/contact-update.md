---
title: Обновление контакта
description: Обновление свойств объекта contact.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4e26fb6521c3f9bcd6672da4241a727b3680aab1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518296"
---
# <a name="update-contact"></a><span data-ttu-id="a9fff-103">Обновление контакта</span><span class="sxs-lookup"><span data-stu-id="a9fff-103">Update contact</span></span>

<span data-ttu-id="a9fff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9fff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a9fff-105">Обновление свойств объекта contact.</span><span class="sxs-lookup"><span data-stu-id="a9fff-105">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9fff-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9fff-106">Permissions</span></span>
<span data-ttu-id="a9fff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9fff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9fff-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9fff-109">Permission type</span></span>      | <span data-ttu-id="a9fff-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9fff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9fff-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9fff-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a9fff-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9fff-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a9fff-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9fff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9fff-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9fff-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a9fff-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9fff-115">Application</span></span> | <span data-ttu-id="a9fff-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9fff-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9fff-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9fff-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a9fff-118">Объект [contact](../resources/contact.md) из стандартной пользовательской папки [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a9fff-118">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="a9fff-119">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="a9fff-119">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="a9fff-p102">Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md). Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="a9fff-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a9fff-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9fff-122">Request headers</span></span>
| <span data-ttu-id="a9fff-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9fff-123">Header</span></span>       | <span data-ttu-id="a9fff-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a9fff-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a9fff-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9fff-125">Authorization</span></span>  | <span data-ttu-id="a9fff-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9fff-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a9fff-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a9fff-128">Content-Type</span></span>  | <span data-ttu-id="a9fff-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9fff-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a9fff-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9fff-131">Request body</span></span>
<span data-ttu-id="a9fff-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a9fff-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a9fff-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9fff-135">Property</span></span>     | <span data-ttu-id="a9fff-136">Тип</span><span class="sxs-lookup"><span data-stu-id="a9fff-136">Type</span></span>   |<span data-ttu-id="a9fff-137">Описание</span><span class="sxs-lookup"><span data-stu-id="a9fff-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9fff-138">assistantName</span><span class="sxs-lookup"><span data-stu-id="a9fff-138">assistantName</span></span>|<span data-ttu-id="a9fff-139">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-139">String</span></span>|<span data-ttu-id="a9fff-140">Имя помощника контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-140">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="a9fff-141">birthday</span><span class="sxs-lookup"><span data-stu-id="a9fff-141">birthday</span></span>|<span data-ttu-id="a9fff-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9fff-142">DateTimeOffset</span></span>|<span data-ttu-id="a9fff-143">Дата рождения контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-143">The contact's birthday.</span></span>|
|<span data-ttu-id="a9fff-144">businessAddress</span><span class="sxs-lookup"><span data-stu-id="a9fff-144">businessAddress</span></span>|[<span data-ttu-id="a9fff-145">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="a9fff-145">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="a9fff-146">Рабочий адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-146">The contact's business address.</span></span>|
|<span data-ttu-id="a9fff-147">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="a9fff-147">businessHomePage</span></span>|<span data-ttu-id="a9fff-148">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-148">String</span></span>|<span data-ttu-id="a9fff-149">Домашняя страница контакта (рабочая).</span><span class="sxs-lookup"><span data-stu-id="a9fff-149">The business home page of the contact.</span></span>|
|<span data-ttu-id="a9fff-150">businessPhones</span><span class="sxs-lookup"><span data-stu-id="a9fff-150">businessPhones</span></span>|<span data-ttu-id="a9fff-151">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-151">String</span></span>|<span data-ttu-id="a9fff-152">Рабочие номера телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-152">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="a9fff-153">categories</span><span class="sxs-lookup"><span data-stu-id="a9fff-153">categories</span></span>|<span data-ttu-id="a9fff-154">String</span><span class="sxs-lookup"><span data-stu-id="a9fff-154">String</span></span>|<span data-ttu-id="a9fff-155">Категории, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="a9fff-155">The categories associated with the contact.</span></span>|
|<span data-ttu-id="a9fff-156">children</span><span class="sxs-lookup"><span data-stu-id="a9fff-156">children</span></span>|<span data-ttu-id="a9fff-157">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-157">String</span></span>|<span data-ttu-id="a9fff-158">Имена детей контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-158">The names of the contact's children.</span></span>|
|<span data-ttu-id="a9fff-159">companyName</span><span class="sxs-lookup"><span data-stu-id="a9fff-159">companyName</span></span>|<span data-ttu-id="a9fff-160">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-160">String</span></span>|<span data-ttu-id="a9fff-161">Название компании контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-161">The name of the contact's company.</span></span>|
|<span data-ttu-id="a9fff-162">department</span><span class="sxs-lookup"><span data-stu-id="a9fff-162">department</span></span>|<span data-ttu-id="a9fff-163">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-163">String</span></span>|<span data-ttu-id="a9fff-164">Отдел контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-164">The contact's department.</span></span>|
|<span data-ttu-id="a9fff-165">displayName</span><span class="sxs-lookup"><span data-stu-id="a9fff-165">displayName</span></span>|<span data-ttu-id="a9fff-166">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-166">String</span></span>|<span data-ttu-id="a9fff-167">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-167">The contact's display name.</span></span> <span data-ttu-id="a9fff-168">Обратите внимание, что последующие обновления других свойств могут привести к тому, что автоматически созданное значение перезапишет указанное значение displayName.</span><span class="sxs-lookup"><span data-stu-id="a9fff-168">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="a9fff-169">Чтобы сохранить существующее значение, всегда добавляйте его как displayName в операцию обновления.</span><span class="sxs-lookup"><span data-stu-id="a9fff-169">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="a9fff-170">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="a9fff-170">emailAddresses</span></span>|<span data-ttu-id="a9fff-171">Коллекция [EmailAddress](../resources/emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="a9fff-171">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="a9fff-172">Электронные адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-172">The contact's email addresses.</span></span>|
|<span data-ttu-id="a9fff-173">fileAs</span><span class="sxs-lookup"><span data-stu-id="a9fff-173">fileAs</span></span>|<span data-ttu-id="a9fff-174">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-174">String</span></span>|<span data-ttu-id="a9fff-175">Имя, под которым хранится контакт.</span><span class="sxs-lookup"><span data-stu-id="a9fff-175">The name the contact is filed under.</span></span>|
|<span data-ttu-id="a9fff-176">generation</span><span class="sxs-lookup"><span data-stu-id="a9fff-176">generation</span></span>|<span data-ttu-id="a9fff-177">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-177">String</span></span>|<span data-ttu-id="a9fff-178">Поколение контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-178">The contact's generation.</span></span>|
|<span data-ttu-id="a9fff-179">givenName</span><span class="sxs-lookup"><span data-stu-id="a9fff-179">givenName</span></span>|<span data-ttu-id="a9fff-180">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-180">String</span></span>|<span data-ttu-id="a9fff-181">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-181">The contact's given name.</span></span>|
|<span data-ttu-id="a9fff-182">homeAddress</span><span class="sxs-lookup"><span data-stu-id="a9fff-182">homeAddress</span></span>|[<span data-ttu-id="a9fff-183">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="a9fff-183">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="a9fff-184">Домашний адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-184">The contact's home address.</span></span>|
|<span data-ttu-id="a9fff-185">homePhones</span><span class="sxs-lookup"><span data-stu-id="a9fff-185">homePhones</span></span>|<span data-ttu-id="a9fff-186">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a9fff-186">String collection</span></span>|<span data-ttu-id="a9fff-187">Номера домашних телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-187">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="a9fff-188">imAddresses</span><span class="sxs-lookup"><span data-stu-id="a9fff-188">imAddresses</span></span>|<span data-ttu-id="a9fff-189">String</span><span class="sxs-lookup"><span data-stu-id="a9fff-189">String</span></span>|<span data-ttu-id="a9fff-190">Адреса контакта для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="a9fff-190">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="a9fff-191">initials</span><span class="sxs-lookup"><span data-stu-id="a9fff-191">initials</span></span>|<span data-ttu-id="a9fff-192">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-192">String</span></span>|<span data-ttu-id="a9fff-193">Инициалы контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-193">The contact's initials.</span></span>|
|<span data-ttu-id="a9fff-194">jobTitle</span><span class="sxs-lookup"><span data-stu-id="a9fff-194">jobTitle</span></span>|<span data-ttu-id="a9fff-195">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-195">String</span></span>|<span data-ttu-id="a9fff-196">Должность контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-196">The contact’s job title.</span></span>|
|<span data-ttu-id="a9fff-197">manager</span><span class="sxs-lookup"><span data-stu-id="a9fff-197">manager</span></span>|<span data-ttu-id="a9fff-198">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-198">String</span></span>|<span data-ttu-id="a9fff-199">Имя руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-199">The name of the contact's manager.</span></span>
|<span data-ttu-id="a9fff-200">middleName</span><span class="sxs-lookup"><span data-stu-id="a9fff-200">middleName</span></span>|<span data-ttu-id="a9fff-201">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-201">String</span></span>|<span data-ttu-id="a9fff-202">Отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-202">The contact's middle name.</span></span>|
|<span data-ttu-id="a9fff-203">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="a9fff-203">mobilePhone</span></span>|<span data-ttu-id="a9fff-204">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-204">String</span></span>|<span data-ttu-id="a9fff-205">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-205">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="a9fff-206">nickName</span><span class="sxs-lookup"><span data-stu-id="a9fff-206">nickName</span></span>|<span data-ttu-id="a9fff-207">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-207">String</span></span>|<span data-ttu-id="a9fff-208">Псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-208">The contact's nickname.</span></span>|
|<span data-ttu-id="a9fff-209">officeLocation</span><span class="sxs-lookup"><span data-stu-id="a9fff-209">officeLocation</span></span>|<span data-ttu-id="a9fff-210">String</span><span class="sxs-lookup"><span data-stu-id="a9fff-210">String</span></span>|<span data-ttu-id="a9fff-211">Расположение офиса контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-211">The location of the contact's office.</span></span>|
|<span data-ttu-id="a9fff-212">otherAddress</span><span class="sxs-lookup"><span data-stu-id="a9fff-212">otherAddress</span></span>|[<span data-ttu-id="a9fff-213">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="a9fff-213">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="a9fff-214">Другие адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-214">Other addresses for the contact.</span></span>|
|<span data-ttu-id="a9fff-215">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="a9fff-215">parentFolderId</span></span>|<span data-ttu-id="a9fff-216">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-216">String</span></span>|<span data-ttu-id="a9fff-217">Идентификатор родительской папки контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-217">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="a9fff-218">personalNotes</span><span class="sxs-lookup"><span data-stu-id="a9fff-218">personalNotes</span></span>|<span data-ttu-id="a9fff-219">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-219">String</span></span>|<span data-ttu-id="a9fff-220">Заметки пользователя о контакте.</span><span class="sxs-lookup"><span data-stu-id="a9fff-220">The user's notes about the contact.</span></span>|
|<span data-ttu-id="a9fff-221">profession</span><span class="sxs-lookup"><span data-stu-id="a9fff-221">profession</span></span>|<span data-ttu-id="a9fff-222">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-222">String</span></span>|<span data-ttu-id="a9fff-223">Профессия контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-223">The contact's profession.</span></span>|
|<span data-ttu-id="a9fff-224">spouseName</span><span class="sxs-lookup"><span data-stu-id="a9fff-224">spouseName</span></span>|<span data-ttu-id="a9fff-225">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-225">String</span></span>|<span data-ttu-id="a9fff-226">Имя супруга или супруги контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-226">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="a9fff-227">surname</span><span class="sxs-lookup"><span data-stu-id="a9fff-227">surname</span></span>|<span data-ttu-id="a9fff-228">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-228">String</span></span>|<span data-ttu-id="a9fff-229">Фамилия контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-229">The contact's surname.</span></span>|
|<span data-ttu-id="a9fff-230">title</span><span class="sxs-lookup"><span data-stu-id="a9fff-230">title</span></span>|<span data-ttu-id="a9fff-231">String</span><span class="sxs-lookup"><span data-stu-id="a9fff-231">String</span></span>|<span data-ttu-id="a9fff-232">Звание контакта.</span><span class="sxs-lookup"><span data-stu-id="a9fff-232">The contact's title.</span></span>|
|<span data-ttu-id="a9fff-233">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="a9fff-233">yomiCompanyName</span></span>|<span data-ttu-id="a9fff-234">Строка</span><span class="sxs-lookup"><span data-stu-id="a9fff-234">String</span></span>|<span data-ttu-id="a9fff-p107">Название компании контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a9fff-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="a9fff-237">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="a9fff-237">yomiGivenName</span></span>|<span data-ttu-id="a9fff-238">String</span><span class="sxs-lookup"><span data-stu-id="a9fff-238">String</span></span>|<span data-ttu-id="a9fff-p108">Имя контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a9fff-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="a9fff-241">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="a9fff-241">yomiSurname</span></span>|<span data-ttu-id="a9fff-242">String</span><span class="sxs-lookup"><span data-stu-id="a9fff-242">String</span></span>|<span data-ttu-id="a9fff-p109">Фамилия контакта, записанная так, как она звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a9fff-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="a9fff-245">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9fff-245">Response</span></span>

<span data-ttu-id="a9fff-246">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [contact](../resources/contact.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a9fff-246">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a9fff-247">Пример</span><span class="sxs-lookup"><span data-stu-id="a9fff-247">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9fff-248">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9fff-248">Request</span></span>
<span data-ttu-id="a9fff-249">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9fff-249">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9fff-250">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9fff-250">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contacts/{id}
Content-type: application/json
Content-length: 1977

{
  "homeAddress": {
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98121"
  },
  "birthday": "1974-07-22"
}
```
# <a name="c"></a>[<span data-ttu-id="a9fff-251">C#</span><span class="sxs-lookup"><span data-stu-id="a9fff-251">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9fff-252">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9fff-252">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9fff-253">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9fff-253">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9fff-254">Java</span><span class="sxs-lookup"><span data-stu-id="a9fff-254">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a9fff-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9fff-255">Response</span></span>
<span data-ttu-id="a9fff-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9fff-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1977

{
  "id": "AAMkAGI2THk0AAA=",
  "createdDateTime": "2014-10-19T23:08:24Z",
  "lastModifiedDateTime": "2014-10-19T23:08:24Z",
  "changeKey": "EQAAABYAAACd9nJ/tVysQos2hTfspaWRAAADTIa4",
  "categories": [],
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "birthday": "1974-07-22",
  "fileAs": "Fort, Garth",
  "displayName": "Garth Fort",
  "givenName": "Garth",
  "initials": "G.F.",
  "middleName": null,
  "nickName": "Garth",
  "surname": "Fort",
  "title": null,
  "yomiGivenName": null,
  "yomiSurname": null,
  "yomiCompanyName": null,
  "generation": null,
  "emailAddresses": [
    {
      "name": "Garth",
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com"
    }
  ],
  "imAddresses": [
    "sip:garthf@a830edad9050849nda1.onmicrosoft.com"
  ],
  "jobTitle": "Web Marketing Manager",
  "companyName": "Contoso, Inc.",
  "department": "Sales & Marketing",
  "officeLocation": "20/1101",
  "profession": null,
  "businessHomePage": "https://www.contoso.com",
  "assistantName": null,
  "manager": null,
  "homePhones": [],
  "mobilePhone": null,
  "businessPhones": [
    "+1 918 555 0101"
  ],
  "homeAddress": {
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98121"
  },
  "businessAddress": {
      "street": "10 Contoso Way",
      "city": "Redmond",
      "state": "WA",
      "countryOrRegion": "USA",
      "postalCode": "98075"  
  },
  "otherAddress": {},
  "spouseName": null,
  "personalNotes": null,
  "children": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
