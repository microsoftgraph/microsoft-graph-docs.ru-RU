---
title: Обновление контакта
description: Обновление свойств контактного объекта.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3108edc3db30865cfd9541c053dbe1ea5105dd63
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047114"
---
# <a name="update-contact"></a><span data-ttu-id="27665-103">Обновление контакта</span><span class="sxs-lookup"><span data-stu-id="27665-103">Update contact</span></span>

<span data-ttu-id="27665-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27665-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27665-105">Обновление свойств контактного объекта.</span><span class="sxs-lookup"><span data-stu-id="27665-105">Update the properties of contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="27665-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27665-106">Permissions</span></span>
<span data-ttu-id="27665-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27665-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27665-109">Permission type</span></span>      | <span data-ttu-id="27665-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27665-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27665-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27665-111">Delegated (work or school account)</span></span> | <span data-ttu-id="27665-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27665-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="27665-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27665-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27665-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27665-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="27665-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27665-115">Application</span></span> | <span data-ttu-id="27665-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27665-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="27665-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27665-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="27665-118">Контакт [от](../resources/contact.md) пользователя по умолчанию [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="27665-118">A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="27665-119">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="27665-119">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="27665-120">Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="27665-120">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="27665-121">Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="27665-121">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="27665-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27665-122">Request headers</span></span>
| <span data-ttu-id="27665-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27665-123">Header</span></span>       | <span data-ttu-id="27665-124">Значение</span><span class="sxs-lookup"><span data-stu-id="27665-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="27665-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27665-125">Authorization</span></span>  | <span data-ttu-id="27665-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27665-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="27665-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27665-128">Content-Type</span></span>  | <span data-ttu-id="27665-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27665-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="27665-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27665-131">Request body</span></span>
<span data-ttu-id="27665-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="27665-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="27665-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="27665-135">Property</span></span>     | <span data-ttu-id="27665-136">Тип</span><span class="sxs-lookup"><span data-stu-id="27665-136">Type</span></span>   |<span data-ttu-id="27665-137">Описание</span><span class="sxs-lookup"><span data-stu-id="27665-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27665-138">assistantName</span><span class="sxs-lookup"><span data-stu-id="27665-138">assistantName</span></span>|<span data-ttu-id="27665-139">String</span><span class="sxs-lookup"><span data-stu-id="27665-139">String</span></span>|<span data-ttu-id="27665-140">Имя помощника контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-140">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="27665-141">birthday</span><span class="sxs-lookup"><span data-stu-id="27665-141">birthday</span></span>|<span data-ttu-id="27665-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27665-142">DateTimeOffset</span></span>|<span data-ttu-id="27665-143">Дата рождения контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-143">The contact's birthday.</span></span>|
|<span data-ttu-id="27665-144">categories</span><span class="sxs-lookup"><span data-stu-id="27665-144">categories</span></span>|<span data-ttu-id="27665-145">String</span><span class="sxs-lookup"><span data-stu-id="27665-145">String</span></span>|<span data-ttu-id="27665-146">Категории, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="27665-146">The categories associated with the contact.</span></span>|
|<span data-ttu-id="27665-147">children</span><span class="sxs-lookup"><span data-stu-id="27665-147">children</span></span>|<span data-ttu-id="27665-148">String</span><span class="sxs-lookup"><span data-stu-id="27665-148">String</span></span>||
|<span data-ttu-id="27665-149">companyName</span><span class="sxs-lookup"><span data-stu-id="27665-149">companyName</span></span>|<span data-ttu-id="27665-150">String</span><span class="sxs-lookup"><span data-stu-id="27665-150">String</span></span>|<span data-ttu-id="27665-151">Название компании контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-151">The name of the contact's company.</span></span>|
|<span data-ttu-id="27665-152">department</span><span class="sxs-lookup"><span data-stu-id="27665-152">department</span></span>|<span data-ttu-id="27665-153">String</span><span class="sxs-lookup"><span data-stu-id="27665-153">String</span></span>|<span data-ttu-id="27665-154">Отдел контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-154">The contact's department.</span></span>|
|<span data-ttu-id="27665-155">displayName</span><span class="sxs-lookup"><span data-stu-id="27665-155">displayName</span></span>|<span data-ttu-id="27665-156">String</span><span class="sxs-lookup"><span data-stu-id="27665-156">String</span></span>|<span data-ttu-id="27665-157">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-157">The contact's display name.</span></span> <span data-ttu-id="27665-158">Обратите внимание, что последующие обновления других свойств могут привести к тому, что автоматически созданное значение перезапишет указанное значение displayName.</span><span class="sxs-lookup"><span data-stu-id="27665-158">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="27665-159">Чтобы сохранить существующее значение, всегда добавляйте его как displayName в операцию обновления.</span><span class="sxs-lookup"><span data-stu-id="27665-159">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="27665-160">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="27665-160">emailAddresses</span></span>|<span data-ttu-id="27665-161">[коллекция typedEmailAddress](../resources/typedemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="27665-161">[typedEmailAddress](../resources/typedemailaddress.md) collection</span></span>|<span data-ttu-id="27665-162">Электронные адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-162">The contact's email addresses.</span></span>|
|<span data-ttu-id="27665-163">fileAs</span><span class="sxs-lookup"><span data-stu-id="27665-163">fileAs</span></span>|<span data-ttu-id="27665-164">String</span><span class="sxs-lookup"><span data-stu-id="27665-164">String</span></span>|<span data-ttu-id="27665-165">Имя, под которым хранится контакт.</span><span class="sxs-lookup"><span data-stu-id="27665-165">The name the contact is filed under.</span></span>|
|<span data-ttu-id="27665-166">gender</span><span class="sxs-lookup"><span data-stu-id="27665-166">gender</span></span> |<span data-ttu-id="27665-167">String</span><span class="sxs-lookup"><span data-stu-id="27665-167">String</span></span> |<span data-ttu-id="27665-168">Пол контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-168">The contact's gender.</span></span> |
|<span data-ttu-id="27665-169">generation</span><span class="sxs-lookup"><span data-stu-id="27665-169">generation</span></span>|<span data-ttu-id="27665-170">String</span><span class="sxs-lookup"><span data-stu-id="27665-170">String</span></span>|<span data-ttu-id="27665-171">Поколение контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-171">The contact's generation.</span></span>|
|<span data-ttu-id="27665-172">givenName</span><span class="sxs-lookup"><span data-stu-id="27665-172">givenName</span></span>|<span data-ttu-id="27665-173">String</span><span class="sxs-lookup"><span data-stu-id="27665-173">String</span></span>|<span data-ttu-id="27665-174">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-174">The contact's given name.</span></span>|
|<span data-ttu-id="27665-175">imAddresses</span><span class="sxs-lookup"><span data-stu-id="27665-175">imAddresses</span></span>|<span data-ttu-id="27665-176">String</span><span class="sxs-lookup"><span data-stu-id="27665-176">String</span></span>|<span data-ttu-id="27665-177">Адреса контакта для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="27665-177">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="27665-178">initials</span><span class="sxs-lookup"><span data-stu-id="27665-178">initials</span></span>|<span data-ttu-id="27665-179">String</span><span class="sxs-lookup"><span data-stu-id="27665-179">String</span></span>|<span data-ttu-id="27665-180">Инициалы контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-180">The contact's initials.</span></span>|
|<span data-ttu-id="27665-181">jobTitle</span><span class="sxs-lookup"><span data-stu-id="27665-181">jobTitle</span></span>|<span data-ttu-id="27665-182">String</span><span class="sxs-lookup"><span data-stu-id="27665-182">String</span></span>|<span data-ttu-id="27665-183">Должность контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-183">The contact’s job title.</span></span>|
|<span data-ttu-id="27665-184">manager</span><span class="sxs-lookup"><span data-stu-id="27665-184">manager</span></span>|<span data-ttu-id="27665-185">String</span><span class="sxs-lookup"><span data-stu-id="27665-185">String</span></span>|<span data-ttu-id="27665-186">Имя руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-186">The name of the contact's manager.</span></span>
|<span data-ttu-id="27665-187">middleName</span><span class="sxs-lookup"><span data-stu-id="27665-187">middleName</span></span>|<span data-ttu-id="27665-188">String</span><span class="sxs-lookup"><span data-stu-id="27665-188">String</span></span>|<span data-ttu-id="27665-189">Отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-189">The contact's middle name.</span></span>|
|<span data-ttu-id="27665-190">nickName</span><span class="sxs-lookup"><span data-stu-id="27665-190">nickName</span></span>|<span data-ttu-id="27665-191">String</span><span class="sxs-lookup"><span data-stu-id="27665-191">String</span></span>|<span data-ttu-id="27665-192">Псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-192">The contact's nickname.</span></span>|
|<span data-ttu-id="27665-193">officeLocation</span><span class="sxs-lookup"><span data-stu-id="27665-193">officeLocation</span></span>|<span data-ttu-id="27665-194">String</span><span class="sxs-lookup"><span data-stu-id="27665-194">String</span></span>|<span data-ttu-id="27665-195">Расположение офиса контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-195">The location of the contact's office.</span></span>|
|<span data-ttu-id="27665-196">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="27665-196">parentFolderId</span></span>|<span data-ttu-id="27665-197">String</span><span class="sxs-lookup"><span data-stu-id="27665-197">String</span></span>|<span data-ttu-id="27665-198">Идентификатор родительской папки контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-198">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="27665-199">personalNotes</span><span class="sxs-lookup"><span data-stu-id="27665-199">personalNotes</span></span>|<span data-ttu-id="27665-200">String</span><span class="sxs-lookup"><span data-stu-id="27665-200">String</span></span>|<span data-ttu-id="27665-201">Заметки пользователя о контакте.</span><span class="sxs-lookup"><span data-stu-id="27665-201">The user's notes about the contact.</span></span>|
|<span data-ttu-id="27665-202">phones</span><span class="sxs-lookup"><span data-stu-id="27665-202">phones</span></span> |<span data-ttu-id="27665-203">Коллекция [phone](../resources/phone.md)</span><span class="sxs-lookup"><span data-stu-id="27665-203">[phone](../resources/phone.md) collection</span></span> |<span data-ttu-id="27665-204">Телефон, связанные с контактом, например домашний телефон, мобильный телефон и бизнес-телефон.</span><span class="sxs-lookup"><span data-stu-id="27665-204">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="27665-205">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="27665-205">postalAddresses</span></span> |<span data-ttu-id="27665-206">[коллекция physicalAddress](../resources/physicaladdress.md)</span><span class="sxs-lookup"><span data-stu-id="27665-206">[physicalAddress](../resources/physicaladdress.md) collection</span></span> |<span data-ttu-id="27665-207">Адреса, связанные с контактом, например домашний адрес и бизнес-адрес.</span><span class="sxs-lookup"><span data-stu-id="27665-207">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="27665-208">profession</span><span class="sxs-lookup"><span data-stu-id="27665-208">profession</span></span>|<span data-ttu-id="27665-209">String</span><span class="sxs-lookup"><span data-stu-id="27665-209">String</span></span>|<span data-ttu-id="27665-210">Профессия контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-210">The contact's profession.</span></span>|
|<span data-ttu-id="27665-211">spouseName</span><span class="sxs-lookup"><span data-stu-id="27665-211">spouseName</span></span>|<span data-ttu-id="27665-212">String</span><span class="sxs-lookup"><span data-stu-id="27665-212">String</span></span>|<span data-ttu-id="27665-213">Имя супруга или супруги контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-213">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="27665-214">surname</span><span class="sxs-lookup"><span data-stu-id="27665-214">surname</span></span>|<span data-ttu-id="27665-215">String</span><span class="sxs-lookup"><span data-stu-id="27665-215">String</span></span>|<span data-ttu-id="27665-216">Фамилия контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-216">The contact's surname.</span></span>|
|<span data-ttu-id="27665-217">title</span><span class="sxs-lookup"><span data-stu-id="27665-217">title</span></span>|<span data-ttu-id="27665-218">String</span><span class="sxs-lookup"><span data-stu-id="27665-218">String</span></span>|<span data-ttu-id="27665-219">Звание контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-219">The contact's title.</span></span>|
|<span data-ttu-id="27665-220">websites</span><span class="sxs-lookup"><span data-stu-id="27665-220">websites</span></span> |<span data-ttu-id="27665-221">Коллекция [website](../resources/website.md)</span><span class="sxs-lookup"><span data-stu-id="27665-221">[website](../resources/website.md) collection</span></span>|<span data-ttu-id="27665-222">Веб-сайты, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="27665-222">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="27665-223">weddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="27665-223">weddingAnniversary</span></span> |<span data-ttu-id="27665-224">Date</span><span class="sxs-lookup"><span data-stu-id="27665-224">Date</span></span> |<span data-ttu-id="27665-225">Годовщина свадьбы контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-225">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="27665-226">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="27665-226">yomiCompanyName</span></span>|<span data-ttu-id="27665-227">String</span><span class="sxs-lookup"><span data-stu-id="27665-227">String</span></span>|<span data-ttu-id="27665-p107">Название компании контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="27665-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="27665-230">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="27665-230">yomiGivenName</span></span>|<span data-ttu-id="27665-231">String</span><span class="sxs-lookup"><span data-stu-id="27665-231">String</span></span>|<span data-ttu-id="27665-p108">Имя контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="27665-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="27665-234">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="27665-234">yomiSurname</span></span>|<span data-ttu-id="27665-235">String</span><span class="sxs-lookup"><span data-stu-id="27665-235">String</span></span>|<span data-ttu-id="27665-p109">Фамилия контакта, записанная так, как она звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="27665-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

<span data-ttu-id="27665-238">Так **как** контактный ресурс поддерживает [расширения,](/graph/extensibility-overview)операцию можно использовать для добавления, обновления или удаления собственных данных, определенных для приложения, в настраиваемом свойстве расширения в существующем экземпляре `PATCH` контакта. </span><span class="sxs-lookup"><span data-stu-id="27665-238">Since the **contact** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **contact** instance.</span></span>

## <a name="response"></a><span data-ttu-id="27665-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="27665-239">Response</span></span>

<span data-ttu-id="27665-240">В случае успешной работы этот метод возвращает код ответа и `200 OK` обновленный контактный объект в [](../resources/contact.md) тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="27665-240">If successful, this method returns a `200 OK` response code and updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="27665-241">Пример</span><span class="sxs-lookup"><span data-stu-id="27665-241">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27665-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="27665-242">Request</span></span>
<span data-ttu-id="27665-243">В следующем примере обновляется личный электронный адрес указанного контакта.</span><span class="sxs-lookup"><span data-stu-id="27665-243">The following example updates the personal email address of the specified contact.</span></span>

# <a name="http"></a>[<span data-ttu-id="27665-244">HTTP</span><span class="sxs-lookup"><span data-stu-id="27665-244">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contacts/AAMkADh6v5AAAvgTCEAAA=
Content-type: application/json

{
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
          "address": "pavelb@fabrikam.onmicrosoft.com",
          "name": "Pavel Bansky",
          "type": "other",
          "otherLabel": "Volunteer work"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="27665-245">C#</span><span class="sxs-lookup"><span data-stu-id="27665-245">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27665-246">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27665-246">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27665-247">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27665-247">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27665-248">Java</span><span class="sxs-lookup"><span data-stu-id="27665-248">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="27665-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="27665-249">Response</span></span>
<span data-ttu-id="27665-250">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27665-250">Here is an example of the response.</span></span> <span data-ttu-id="27665-251">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="27665-251">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts/$entity",
    "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh\"",
    "id":"AAMkADh6v5AAAvgTCEAAA=",
    "createdDateTime":"2018-06-11T19:56:07Z",
    "lastModifiedDateTime":"2018-06-11T20:26:23Z",
    "changeKey":"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh",
    "categories":[

    ],
    "parentFolderId":"AAMkADh6v5AAAAAAEOAAA=",
    "birthday":null,
    "fileAs":"",
    "displayName":"Pavel Bansky",
    "givenName":"Pavel",
    "initials":null,
    "middleName":null,
    "nickName":null,
    "surname":"Bansky",
    "title":null,
    "yomiGivenName":null,
    "yomiSurname":null,
    "yomiCompanyName":null,
    "generation":null,
    "imAddresses":[

    ],
    "jobTitle":null,
    "companyName":null,
    "department":null,
    "officeLocation":null,
    "profession":null,
    "assistantName":null,
    "manager":null,
    "spouseName":null,
    "personalNotes":"",
    "children":[

    ],
    "gender":null,
    "isFavorite":null,
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
            "type":"other",
            "otherLabel":"Volunteer work",
            "name":"Pavel Bansky",
            "address":"pavelb@fabrikam.onmicrosoft.com"
        }
    ],
    "websites":[

    ],
    "phones":[
        {
            "type":"business",
            "number":"+1 732 555 0102"
        }
    ],
    "postalAddresses":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

## <a name="see-also"></a><span data-ttu-id="27665-252">См. также</span><span class="sxs-lookup"><span data-stu-id="27665-252">See also</span></span>

- [<span data-ttu-id="27665-253">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="27665-253">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="27665-254">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="27665-254">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


