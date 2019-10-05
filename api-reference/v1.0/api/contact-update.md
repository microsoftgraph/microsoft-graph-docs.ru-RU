---
title: Обновление контакта
description: Обновление свойств объекта contact.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2dfdcc3b47583b6f37b8b3b760a6bb435f39214b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361746"
---
# <a name="update-contact"></a><span data-ttu-id="785d4-103">Обновление контакта</span><span class="sxs-lookup"><span data-stu-id="785d4-103">Update contact</span></span>

<span data-ttu-id="785d4-104">Обновление свойств объекта contact.</span><span class="sxs-lookup"><span data-stu-id="785d4-104">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="785d4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="785d4-105">Permissions</span></span>
<span data-ttu-id="785d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="785d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="785d4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="785d4-108">Permission type</span></span>      | <span data-ttu-id="785d4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="785d4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="785d4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="785d4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="785d4-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="785d4-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="785d4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="785d4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="785d4-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="785d4-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="785d4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="785d4-114">Application</span></span> | <span data-ttu-id="785d4-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="785d4-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="785d4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="785d4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="785d4-117">Объект [contact](../resources/contact.md) из стандартной пользовательской папки [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="785d4-117">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="785d4-118">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="785d4-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="785d4-p102">Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md). Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="785d4-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="785d4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="785d4-121">Request headers</span></span>
| <span data-ttu-id="785d4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="785d4-122">Header</span></span>       | <span data-ttu-id="785d4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="785d4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="785d4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="785d4-124">Authorization</span></span>  | <span data-ttu-id="785d4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="785d4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="785d4-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="785d4-127">Content-Type</span></span>  | <span data-ttu-id="785d4-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="785d4-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="785d4-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="785d4-130">Request body</span></span>
<span data-ttu-id="785d4-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="785d4-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="785d4-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="785d4-134">Property</span></span>     | <span data-ttu-id="785d4-135">Тип</span><span class="sxs-lookup"><span data-stu-id="785d4-135">Type</span></span>   |<span data-ttu-id="785d4-136">Описание</span><span class="sxs-lookup"><span data-stu-id="785d4-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="785d4-137">assistantName</span><span class="sxs-lookup"><span data-stu-id="785d4-137">assistantName</span></span>|<span data-ttu-id="785d4-138">String</span><span class="sxs-lookup"><span data-stu-id="785d4-138">String</span></span>|<span data-ttu-id="785d4-139">Имя помощника контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-139">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="785d4-140">birthday</span><span class="sxs-lookup"><span data-stu-id="785d4-140">birthday</span></span>|<span data-ttu-id="785d4-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="785d4-141">DateTimeOffset</span></span>|<span data-ttu-id="785d4-142">Дата рождения контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-142">The contact's birthday.</span></span>|
|<span data-ttu-id="785d4-143">businessAddress</span><span class="sxs-lookup"><span data-stu-id="785d4-143">businessAddress</span></span>|[<span data-ttu-id="785d4-144">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="785d4-144">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="785d4-145">Рабочий адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-145">The contact's business address.</span></span>|
|<span data-ttu-id="785d4-146">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="785d4-146">businessHomePage</span></span>|<span data-ttu-id="785d4-147">String</span><span class="sxs-lookup"><span data-stu-id="785d4-147">String</span></span>|<span data-ttu-id="785d4-148">Домашняя страница контакта (рабочая).</span><span class="sxs-lookup"><span data-stu-id="785d4-148">The business home page of the contact.</span></span>|
|<span data-ttu-id="785d4-149">businessPhones</span><span class="sxs-lookup"><span data-stu-id="785d4-149">businessPhones</span></span>|<span data-ttu-id="785d4-150">String</span><span class="sxs-lookup"><span data-stu-id="785d4-150">String</span></span>|<span data-ttu-id="785d4-151">Рабочие номера телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-151">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="785d4-152">categories</span><span class="sxs-lookup"><span data-stu-id="785d4-152">categories</span></span>|<span data-ttu-id="785d4-153">String</span><span class="sxs-lookup"><span data-stu-id="785d4-153">String</span></span>|<span data-ttu-id="785d4-154">Категории, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="785d4-154">The categories associated with the contact.</span></span>|
|<span data-ttu-id="785d4-155">children</span><span class="sxs-lookup"><span data-stu-id="785d4-155">children</span></span>|<span data-ttu-id="785d4-156">String</span><span class="sxs-lookup"><span data-stu-id="785d4-156">String</span></span>|<span data-ttu-id="785d4-157">Имена детей контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-157">The names of the contact's children.</span></span>|
|<span data-ttu-id="785d4-158">companyName</span><span class="sxs-lookup"><span data-stu-id="785d4-158">companyName</span></span>|<span data-ttu-id="785d4-159">String</span><span class="sxs-lookup"><span data-stu-id="785d4-159">String</span></span>|<span data-ttu-id="785d4-160">Название компании контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-160">The name of the contact's company.</span></span>|
|<span data-ttu-id="785d4-161">department</span><span class="sxs-lookup"><span data-stu-id="785d4-161">department</span></span>|<span data-ttu-id="785d4-162">String</span><span class="sxs-lookup"><span data-stu-id="785d4-162">String</span></span>|<span data-ttu-id="785d4-163">Отдел контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-163">The contact's department.</span></span>|
|<span data-ttu-id="785d4-164">displayName</span><span class="sxs-lookup"><span data-stu-id="785d4-164">displayName</span></span>|<span data-ttu-id="785d4-165">Строка</span><span class="sxs-lookup"><span data-stu-id="785d4-165">String</span></span>|<span data-ttu-id="785d4-166">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-166">The contact's display name.</span></span> <span data-ttu-id="785d4-167">Обратите внимание, что последующие обновления других свойств могут привести к тому, что автоматически созданное значение перезапишет указанное значение displayName.</span><span class="sxs-lookup"><span data-stu-id="785d4-167">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="785d4-168">Чтобы сохранить существующее значение, всегда добавляйте его как displayName в операцию обновления.</span><span class="sxs-lookup"><span data-stu-id="785d4-168">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="785d4-169">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="785d4-169">emailAddresses</span></span>|<span data-ttu-id="785d4-170">Коллекция [EmailAddress](../resources/emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="785d4-170">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="785d4-171">Электронные адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-171">The contact's email addresses.</span></span>|
|<span data-ttu-id="785d4-172">fileAs</span><span class="sxs-lookup"><span data-stu-id="785d4-172">fileAs</span></span>|<span data-ttu-id="785d4-173">String</span><span class="sxs-lookup"><span data-stu-id="785d4-173">String</span></span>|<span data-ttu-id="785d4-174">Имя, под которым хранится контакт.</span><span class="sxs-lookup"><span data-stu-id="785d4-174">The name the contact is filed under.</span></span>|
|<span data-ttu-id="785d4-175">generation</span><span class="sxs-lookup"><span data-stu-id="785d4-175">generation</span></span>|<span data-ttu-id="785d4-176">String</span><span class="sxs-lookup"><span data-stu-id="785d4-176">String</span></span>|<span data-ttu-id="785d4-177">Поколение контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-177">The contact's generation.</span></span>|
|<span data-ttu-id="785d4-178">givenName</span><span class="sxs-lookup"><span data-stu-id="785d4-178">givenName</span></span>|<span data-ttu-id="785d4-179">String</span><span class="sxs-lookup"><span data-stu-id="785d4-179">String</span></span>|<span data-ttu-id="785d4-180">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-180">The contact's given name.</span></span>|
|<span data-ttu-id="785d4-181">homeAddress</span><span class="sxs-lookup"><span data-stu-id="785d4-181">homeAddress</span></span>|[<span data-ttu-id="785d4-182">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="785d4-182">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="785d4-183">Домашний адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-183">The contact's home address.</span></span>|
|<span data-ttu-id="785d4-184">homePhones</span><span class="sxs-lookup"><span data-stu-id="785d4-184">homePhones</span></span>|<span data-ttu-id="785d4-185">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="785d4-185">String collection</span></span>|<span data-ttu-id="785d4-186">Номера домашних телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-186">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="785d4-187">imAddresses</span><span class="sxs-lookup"><span data-stu-id="785d4-187">imAddresses</span></span>|<span data-ttu-id="785d4-188">String</span><span class="sxs-lookup"><span data-stu-id="785d4-188">String</span></span>|<span data-ttu-id="785d4-189">Адреса контакта для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="785d4-189">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="785d4-190">initials</span><span class="sxs-lookup"><span data-stu-id="785d4-190">initials</span></span>|<span data-ttu-id="785d4-191">String</span><span class="sxs-lookup"><span data-stu-id="785d4-191">String</span></span>|<span data-ttu-id="785d4-192">Инициалы контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-192">The contact's initials.</span></span>|
|<span data-ttu-id="785d4-193">jobTitle</span><span class="sxs-lookup"><span data-stu-id="785d4-193">jobTitle</span></span>|<span data-ttu-id="785d4-194">String</span><span class="sxs-lookup"><span data-stu-id="785d4-194">String</span></span>|<span data-ttu-id="785d4-195">Должность контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-195">The contact’s job title.</span></span>|
|<span data-ttu-id="785d4-196">manager</span><span class="sxs-lookup"><span data-stu-id="785d4-196">manager</span></span>|<span data-ttu-id="785d4-197">String</span><span class="sxs-lookup"><span data-stu-id="785d4-197">String</span></span>|<span data-ttu-id="785d4-198">Имя руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-198">The name of the contact's manager.</span></span>
|<span data-ttu-id="785d4-199">middleName</span><span class="sxs-lookup"><span data-stu-id="785d4-199">middleName</span></span>|<span data-ttu-id="785d4-200">String</span><span class="sxs-lookup"><span data-stu-id="785d4-200">String</span></span>|<span data-ttu-id="785d4-201">Отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-201">The contact's middle name.</span></span>|
|<span data-ttu-id="785d4-202">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="785d4-202">mobilePhone</span></span>|<span data-ttu-id="785d4-203">String</span><span class="sxs-lookup"><span data-stu-id="785d4-203">String</span></span>|<span data-ttu-id="785d4-204">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-204">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="785d4-205">nickName</span><span class="sxs-lookup"><span data-stu-id="785d4-205">nickName</span></span>|<span data-ttu-id="785d4-206">String</span><span class="sxs-lookup"><span data-stu-id="785d4-206">String</span></span>|<span data-ttu-id="785d4-207">Псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-207">The contact's nickname.</span></span>|
|<span data-ttu-id="785d4-208">officeLocation</span><span class="sxs-lookup"><span data-stu-id="785d4-208">officeLocation</span></span>|<span data-ttu-id="785d4-209">String</span><span class="sxs-lookup"><span data-stu-id="785d4-209">String</span></span>|<span data-ttu-id="785d4-210">Расположение офиса контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-210">The location of the contact's office.</span></span>|
|<span data-ttu-id="785d4-211">otherAddress</span><span class="sxs-lookup"><span data-stu-id="785d4-211">otherAddress</span></span>|[<span data-ttu-id="785d4-212">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="785d4-212">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="785d4-213">Другие адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-213">Other addresses for the contact.</span></span>|
|<span data-ttu-id="785d4-214">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="785d4-214">parentFolderId</span></span>|<span data-ttu-id="785d4-215">Строка</span><span class="sxs-lookup"><span data-stu-id="785d4-215">String</span></span>|<span data-ttu-id="785d4-216">Идентификатор родительской папки контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-216">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="785d4-217">personalNotes</span><span class="sxs-lookup"><span data-stu-id="785d4-217">personalNotes</span></span>|<span data-ttu-id="785d4-218">String</span><span class="sxs-lookup"><span data-stu-id="785d4-218">String</span></span>|<span data-ttu-id="785d4-219">Заметки пользователя о контакте.</span><span class="sxs-lookup"><span data-stu-id="785d4-219">The user's notes about the contact.</span></span>|
|<span data-ttu-id="785d4-220">profession</span><span class="sxs-lookup"><span data-stu-id="785d4-220">profession</span></span>|<span data-ttu-id="785d4-221">String</span><span class="sxs-lookup"><span data-stu-id="785d4-221">String</span></span>|<span data-ttu-id="785d4-222">Профессия контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-222">The contact's profession.</span></span>|
|<span data-ttu-id="785d4-223">spouseName</span><span class="sxs-lookup"><span data-stu-id="785d4-223">spouseName</span></span>|<span data-ttu-id="785d4-224">String</span><span class="sxs-lookup"><span data-stu-id="785d4-224">String</span></span>|<span data-ttu-id="785d4-225">Имя супруга или супруги контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-225">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="785d4-226">surname</span><span class="sxs-lookup"><span data-stu-id="785d4-226">surname</span></span>|<span data-ttu-id="785d4-227">String</span><span class="sxs-lookup"><span data-stu-id="785d4-227">String</span></span>|<span data-ttu-id="785d4-228">Фамилия контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-228">The contact's surname.</span></span>|
|<span data-ttu-id="785d4-229">title</span><span class="sxs-lookup"><span data-stu-id="785d4-229">title</span></span>|<span data-ttu-id="785d4-230">String</span><span class="sxs-lookup"><span data-stu-id="785d4-230">String</span></span>|<span data-ttu-id="785d4-231">Звание контакта.</span><span class="sxs-lookup"><span data-stu-id="785d4-231">The contact's title.</span></span>|
|<span data-ttu-id="785d4-232">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="785d4-232">yomiCompanyName</span></span>|<span data-ttu-id="785d4-233">String</span><span class="sxs-lookup"><span data-stu-id="785d4-233">String</span></span>|<span data-ttu-id="785d4-p107">Название компании контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="785d4-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="785d4-236">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="785d4-236">yomiGivenName</span></span>|<span data-ttu-id="785d4-237">String</span><span class="sxs-lookup"><span data-stu-id="785d4-237">String</span></span>|<span data-ttu-id="785d4-p108">Имя контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="785d4-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="785d4-240">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="785d4-240">yomiSurname</span></span>|<span data-ttu-id="785d4-241">String</span><span class="sxs-lookup"><span data-stu-id="785d4-241">String</span></span>|<span data-ttu-id="785d4-p109">Фамилия контакта, записанная так, как она звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="785d4-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="785d4-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="785d4-244">Response</span></span>

<span data-ttu-id="785d4-245">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [contact](../resources/contact.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="785d4-245">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="785d4-246">Пример</span><span class="sxs-lookup"><span data-stu-id="785d4-246">Example</span></span>
##### <a name="request"></a><span data-ttu-id="785d4-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="785d4-247">Request</span></span>
<span data-ttu-id="785d4-248">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="785d4-248">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="785d4-249">HTTP</span><span class="sxs-lookup"><span data-stu-id="785d4-249">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="785d4-250">C#</span><span class="sxs-lookup"><span data-stu-id="785d4-250">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="785d4-251">JavaScript</span><span class="sxs-lookup"><span data-stu-id="785d4-251">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="785d4-252">Objective-C</span><span class="sxs-lookup"><span data-stu-id="785d4-252">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="785d4-253">Java</span><span class="sxs-lookup"><span data-stu-id="785d4-253">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="785d4-254">Отклик</span><span class="sxs-lookup"><span data-stu-id="785d4-254">Response</span></span>
<span data-ttu-id="785d4-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="785d4-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
