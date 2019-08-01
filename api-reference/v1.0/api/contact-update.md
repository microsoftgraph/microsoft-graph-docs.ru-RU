---
title: Обновление контакта
description: Обновление свойств объекта contact.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 214f9d019a1b3fcf7813c29ebcce2244bc7de98e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003233"
---
# <a name="update-contact"></a><span data-ttu-id="8bbf2-103">Обновление контакта</span><span class="sxs-lookup"><span data-stu-id="8bbf2-103">Update contact</span></span>

<span data-ttu-id="8bbf2-104">Обновление свойств объекта contact.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-104">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8bbf2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8bbf2-105">Permissions</span></span>
<span data-ttu-id="8bbf2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bbf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bbf2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bbf2-108">Permission type</span></span>      | <span data-ttu-id="8bbf2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bbf2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bbf2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bbf2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8bbf2-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bbf2-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8bbf2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bbf2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bbf2-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bbf2-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8bbf2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bbf2-114">Application</span></span> | <span data-ttu-id="8bbf2-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bbf2-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bbf2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bbf2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="8bbf2-117">Объект [contact](../resources/contact.md) из стандартной пользовательской папки [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="8bbf2-117">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="8bbf2-118">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="8bbf2-p102">Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md). Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8bbf2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bbf2-121">Request headers</span></span>
| <span data-ttu-id="8bbf2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8bbf2-122">Header</span></span>       | <span data-ttu-id="8bbf2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8bbf2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8bbf2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8bbf2-124">Authorization</span></span>  | <span data-ttu-id="8bbf2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8bbf2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8bbf2-127">Content-Type</span></span>  | <span data-ttu-id="8bbf2-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8bbf2-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8bbf2-130">Request body</span></span>
<span data-ttu-id="8bbf2-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8bbf2-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bbf2-134">Property</span></span>     | <span data-ttu-id="8bbf2-135">Тип</span><span class="sxs-lookup"><span data-stu-id="8bbf2-135">Type</span></span>   |<span data-ttu-id="8bbf2-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8bbf2-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bbf2-137">assistantName</span><span class="sxs-lookup"><span data-stu-id="8bbf2-137">assistantName</span></span>|<span data-ttu-id="8bbf2-138">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-138">String</span></span>|<span data-ttu-id="8bbf2-139">Имя помощника контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-139">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="8bbf2-140">birthday</span><span class="sxs-lookup"><span data-stu-id="8bbf2-140">birthday</span></span>|<span data-ttu-id="8bbf2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bbf2-141">DateTimeOffset</span></span>|<span data-ttu-id="8bbf2-142">Дата рождения контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-142">The contact's birthday.</span></span>|
|<span data-ttu-id="8bbf2-143">businessAddress</span><span class="sxs-lookup"><span data-stu-id="8bbf2-143">businessAddress</span></span>|[<span data-ttu-id="8bbf2-144">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="8bbf2-144">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="8bbf2-145">Рабочий адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-145">The contact's business address.</span></span>|
|<span data-ttu-id="8bbf2-146">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="8bbf2-146">businessHomePage</span></span>|<span data-ttu-id="8bbf2-147">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-147">String</span></span>|<span data-ttu-id="8bbf2-148">Домашняя страница контакта (рабочая).</span><span class="sxs-lookup"><span data-stu-id="8bbf2-148">The business home page of the contact.</span></span>|
|<span data-ttu-id="8bbf2-149">businessPhones</span><span class="sxs-lookup"><span data-stu-id="8bbf2-149">businessPhones</span></span>|<span data-ttu-id="8bbf2-150">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-150">String</span></span>|<span data-ttu-id="8bbf2-151">Рабочие номера телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-151">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="8bbf2-152">categories</span><span class="sxs-lookup"><span data-stu-id="8bbf2-152">categories</span></span>|<span data-ttu-id="8bbf2-153">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-153">String</span></span>|<span data-ttu-id="8bbf2-154">Категории, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-154">The categories associated with the contact.</span></span>|
|<span data-ttu-id="8bbf2-155">children</span><span class="sxs-lookup"><span data-stu-id="8bbf2-155">children</span></span>|<span data-ttu-id="8bbf2-156">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-156">String</span></span>|<span data-ttu-id="8bbf2-157">Имена детей контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-157">The names of the contact's children.</span></span>|
|<span data-ttu-id="8bbf2-158">companyName</span><span class="sxs-lookup"><span data-stu-id="8bbf2-158">companyName</span></span>|<span data-ttu-id="8bbf2-159">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-159">String</span></span>|<span data-ttu-id="8bbf2-160">Название компании контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-160">The name of the contact's company.</span></span>|
|<span data-ttu-id="8bbf2-161">department</span><span class="sxs-lookup"><span data-stu-id="8bbf2-161">department</span></span>|<span data-ttu-id="8bbf2-162">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-162">String</span></span>|<span data-ttu-id="8bbf2-163">Отдел контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-163">The contact's department.</span></span>|
|<span data-ttu-id="8bbf2-164">displayName</span><span class="sxs-lookup"><span data-stu-id="8bbf2-164">displayName</span></span>|<span data-ttu-id="8bbf2-165">Строка</span><span class="sxs-lookup"><span data-stu-id="8bbf2-165">String</span></span>|<span data-ttu-id="8bbf2-166">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-166">The contact's display name.</span></span> <span data-ttu-id="8bbf2-167">Обратите внимание, что последующие обновления других свойств могут привести к тому, что автоматически созданное значение перезапишет указанное значение displayName.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-167">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="8bbf2-168">Чтобы сохранить существующее значение, всегда добавляйте его как displayName в операцию обновления.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-168">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="8bbf2-169">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="8bbf2-169">emailAddresses</span></span>|<span data-ttu-id="8bbf2-170">Коллекция [EmailAddress](../resources/emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="8bbf2-170">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="8bbf2-171">Электронные адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-171">The contact's email addresses.</span></span>|
|<span data-ttu-id="8bbf2-172">fileAs</span><span class="sxs-lookup"><span data-stu-id="8bbf2-172">fileAs</span></span>|<span data-ttu-id="8bbf2-173">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-173">String</span></span>|<span data-ttu-id="8bbf2-174">Имя, под которым хранится контакт.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-174">The name the contact is filed under.</span></span>|
|<span data-ttu-id="8bbf2-175">generation</span><span class="sxs-lookup"><span data-stu-id="8bbf2-175">generation</span></span>|<span data-ttu-id="8bbf2-176">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-176">String</span></span>|<span data-ttu-id="8bbf2-177">Поколение контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-177">The contact's generation.</span></span>|
|<span data-ttu-id="8bbf2-178">givenName</span><span class="sxs-lookup"><span data-stu-id="8bbf2-178">givenName</span></span>|<span data-ttu-id="8bbf2-179">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-179">String</span></span>|<span data-ttu-id="8bbf2-180">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-180">The contact's given name.</span></span>|
|<span data-ttu-id="8bbf2-181">homeAddress</span><span class="sxs-lookup"><span data-stu-id="8bbf2-181">homeAddress</span></span>|[<span data-ttu-id="8bbf2-182">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="8bbf2-182">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="8bbf2-183">Домашний адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-183">The contact's home address.</span></span>|
|<span data-ttu-id="8bbf2-184">homePhones</span><span class="sxs-lookup"><span data-stu-id="8bbf2-184">homePhones</span></span>|<span data-ttu-id="8bbf2-185">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-185">String collection</span></span>|<span data-ttu-id="8bbf2-186">Номера домашних телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-186">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="8bbf2-187">imAddresses</span><span class="sxs-lookup"><span data-stu-id="8bbf2-187">imAddresses</span></span>|<span data-ttu-id="8bbf2-188">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-188">String</span></span>|<span data-ttu-id="8bbf2-189">Адреса контакта для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-189">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="8bbf2-190">initials</span><span class="sxs-lookup"><span data-stu-id="8bbf2-190">initials</span></span>|<span data-ttu-id="8bbf2-191">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-191">String</span></span>|<span data-ttu-id="8bbf2-192">Инициалы контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-192">The contact's initials.</span></span>|
|<span data-ttu-id="8bbf2-193">jobTitle</span><span class="sxs-lookup"><span data-stu-id="8bbf2-193">jobTitle</span></span>|<span data-ttu-id="8bbf2-194">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-194">String</span></span>|<span data-ttu-id="8bbf2-195">Должность контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-195">The contact’s job title.</span></span>|
|<span data-ttu-id="8bbf2-196">manager</span><span class="sxs-lookup"><span data-stu-id="8bbf2-196">manager</span></span>|<span data-ttu-id="8bbf2-197">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-197">String</span></span>|<span data-ttu-id="8bbf2-198">Имя руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-198">The name of the contact's manager.</span></span>
|<span data-ttu-id="8bbf2-199">middleName</span><span class="sxs-lookup"><span data-stu-id="8bbf2-199">middleName</span></span>|<span data-ttu-id="8bbf2-200">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-200">String</span></span>|<span data-ttu-id="8bbf2-201">Отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-201">The contact's middle name.</span></span>|
|<span data-ttu-id="8bbf2-202">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="8bbf2-202">mobilePhone</span></span>|<span data-ttu-id="8bbf2-203">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-203">String</span></span>|<span data-ttu-id="8bbf2-204">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-204">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="8bbf2-205">nickName</span><span class="sxs-lookup"><span data-stu-id="8bbf2-205">nickName</span></span>|<span data-ttu-id="8bbf2-206">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-206">String</span></span>|<span data-ttu-id="8bbf2-207">Псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-207">The contact's nickname.</span></span>|
|<span data-ttu-id="8bbf2-208">officeLocation</span><span class="sxs-lookup"><span data-stu-id="8bbf2-208">officeLocation</span></span>|<span data-ttu-id="8bbf2-209">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-209">String</span></span>|<span data-ttu-id="8bbf2-210">Расположение офиса контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-210">The location of the contact's office.</span></span>|
|<span data-ttu-id="8bbf2-211">otherAddress</span><span class="sxs-lookup"><span data-stu-id="8bbf2-211">otherAddress</span></span>|[<span data-ttu-id="8bbf2-212">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="8bbf2-212">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="8bbf2-213">Другие адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-213">Other addresses for the contact.</span></span>|
|<span data-ttu-id="8bbf2-214">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="8bbf2-214">parentFolderId</span></span>|<span data-ttu-id="8bbf2-215">Строка</span><span class="sxs-lookup"><span data-stu-id="8bbf2-215">String</span></span>|<span data-ttu-id="8bbf2-216">Идентификатор родительской папки контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-216">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="8bbf2-217">personalNotes</span><span class="sxs-lookup"><span data-stu-id="8bbf2-217">personalNotes</span></span>|<span data-ttu-id="8bbf2-218">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-218">String</span></span>|<span data-ttu-id="8bbf2-219">Заметки пользователя о контакте.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-219">The user's notes about the contact.</span></span>|
|<span data-ttu-id="8bbf2-220">profession</span><span class="sxs-lookup"><span data-stu-id="8bbf2-220">profession</span></span>|<span data-ttu-id="8bbf2-221">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-221">String</span></span>|<span data-ttu-id="8bbf2-222">Профессия контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-222">The contact's profession.</span></span>|
|<span data-ttu-id="8bbf2-223">spouseName</span><span class="sxs-lookup"><span data-stu-id="8bbf2-223">spouseName</span></span>|<span data-ttu-id="8bbf2-224">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-224">String</span></span>|<span data-ttu-id="8bbf2-225">Имя супруга или супруги контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-225">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="8bbf2-226">surname</span><span class="sxs-lookup"><span data-stu-id="8bbf2-226">surname</span></span>|<span data-ttu-id="8bbf2-227">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-227">String</span></span>|<span data-ttu-id="8bbf2-228">Фамилия контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-228">The contact's surname.</span></span>|
|<span data-ttu-id="8bbf2-229">title</span><span class="sxs-lookup"><span data-stu-id="8bbf2-229">title</span></span>|<span data-ttu-id="8bbf2-230">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-230">String</span></span>|<span data-ttu-id="8bbf2-231">Звание контакта.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-231">The contact's title.</span></span>|
|<span data-ttu-id="8bbf2-232">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="8bbf2-232">yomiCompanyName</span></span>|<span data-ttu-id="8bbf2-233">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-233">String</span></span>|<span data-ttu-id="8bbf2-p107">Название компании контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="8bbf2-236">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="8bbf2-236">yomiGivenName</span></span>|<span data-ttu-id="8bbf2-237">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-237">String</span></span>|<span data-ttu-id="8bbf2-p108">Имя контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="8bbf2-240">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="8bbf2-240">yomiSurname</span></span>|<span data-ttu-id="8bbf2-241">String</span><span class="sxs-lookup"><span data-stu-id="8bbf2-241">String</span></span>|<span data-ttu-id="8bbf2-p109">Фамилия контакта, записанная так, как она звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="8bbf2-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bbf2-244">Response</span></span>

<span data-ttu-id="8bbf2-245">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [contact](../resources/contact.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-245">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8bbf2-246">Пример</span><span class="sxs-lookup"><span data-stu-id="8bbf2-246">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8bbf2-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bbf2-247">Request</span></span>
<span data-ttu-id="8bbf2-248">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-248">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8bbf2-249">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bbf2-249">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8bbf2-250">C#</span><span class="sxs-lookup"><span data-stu-id="8bbf2-250">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8bbf2-251">Javascript</span><span class="sxs-lookup"><span data-stu-id="8bbf2-251">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8bbf2-252">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8bbf2-252">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8bbf2-253">Java</span><span class="sxs-lookup"><span data-stu-id="8bbf2-253">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8bbf2-254">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bbf2-254">Response</span></span>
<span data-ttu-id="8bbf2-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8bbf2-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
