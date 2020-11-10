---
title: Обновление контакта
description: Обновление свойств объекта Contact.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b52e2f0089a8793956ec481932e2aa36cd200d7d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957161"
---
# <a name="update-contact"></a><span data-ttu-id="dc06a-103">Обновление контакта</span><span class="sxs-lookup"><span data-stu-id="dc06a-103">Update contact</span></span>

<span data-ttu-id="dc06a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc06a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc06a-105">Обновление свойств объекта Contact.</span><span class="sxs-lookup"><span data-stu-id="dc06a-105">Update the properties of contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dc06a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc06a-106">Permissions</span></span>
<span data-ttu-id="dc06a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc06a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc06a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc06a-109">Permission type</span></span>      | <span data-ttu-id="dc06a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc06a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc06a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc06a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dc06a-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc06a-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="dc06a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc06a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc06a-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc06a-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="dc06a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc06a-115">Application</span></span> | <span data-ttu-id="dc06a-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc06a-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc06a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc06a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="dc06a-118">[Контакт](../resources/contact.md) от [contactFolder](../resources/contactfolder.md)пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc06a-118">A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="dc06a-119">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="dc06a-119">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="dc06a-120">Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="dc06a-120">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="dc06a-121">Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="dc06a-121">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="dc06a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc06a-122">Request headers</span></span>
| <span data-ttu-id="dc06a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc06a-123">Header</span></span>       | <span data-ttu-id="dc06a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="dc06a-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dc06a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc06a-125">Authorization</span></span>  | <span data-ttu-id="dc06a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc06a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dc06a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dc06a-128">Content-Type</span></span>  | <span data-ttu-id="dc06a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc06a-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dc06a-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc06a-131">Request body</span></span>
<span data-ttu-id="dc06a-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="dc06a-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dc06a-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc06a-135">Property</span></span>     | <span data-ttu-id="dc06a-136">Тип</span><span class="sxs-lookup"><span data-stu-id="dc06a-136">Type</span></span>   |<span data-ttu-id="dc06a-137">Описание</span><span class="sxs-lookup"><span data-stu-id="dc06a-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc06a-138">assistantName</span><span class="sxs-lookup"><span data-stu-id="dc06a-138">assistantName</span></span>|<span data-ttu-id="dc06a-139">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-139">String</span></span>|<span data-ttu-id="dc06a-140">Имя помощника контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-140">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="dc06a-141">birthday</span><span class="sxs-lookup"><span data-stu-id="dc06a-141">birthday</span></span>|<span data-ttu-id="dc06a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc06a-142">DateTimeOffset</span></span>|<span data-ttu-id="dc06a-143">Дата рождения контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-143">The contact's birthday.</span></span>|
|<span data-ttu-id="dc06a-144">categories</span><span class="sxs-lookup"><span data-stu-id="dc06a-144">categories</span></span>|<span data-ttu-id="dc06a-145">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-145">String</span></span>|<span data-ttu-id="dc06a-146">Категории, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="dc06a-146">The categories associated with the contact.</span></span>|
|<span data-ttu-id="dc06a-147">children</span><span class="sxs-lookup"><span data-stu-id="dc06a-147">children</span></span>|<span data-ttu-id="dc06a-148">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-148">String</span></span>||
|<span data-ttu-id="dc06a-149">companyName</span><span class="sxs-lookup"><span data-stu-id="dc06a-149">companyName</span></span>|<span data-ttu-id="dc06a-150">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-150">String</span></span>|<span data-ttu-id="dc06a-151">Название компании контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-151">The name of the contact's company.</span></span>|
|<span data-ttu-id="dc06a-152">department</span><span class="sxs-lookup"><span data-stu-id="dc06a-152">department</span></span>|<span data-ttu-id="dc06a-153">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-153">String</span></span>|<span data-ttu-id="dc06a-154">Отдел контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-154">The contact's department.</span></span>|
|<span data-ttu-id="dc06a-155">displayName</span><span class="sxs-lookup"><span data-stu-id="dc06a-155">displayName</span></span>|<span data-ttu-id="dc06a-156">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-156">String</span></span>|<span data-ttu-id="dc06a-157">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-157">The contact's display name.</span></span> <span data-ttu-id="dc06a-158">Обратите внимание, что последующие обновления других свойств могут привести к тому, что автоматически созданное значение перезапишет указанное значение displayName.</span><span class="sxs-lookup"><span data-stu-id="dc06a-158">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="dc06a-159">Чтобы сохранить существующее значение, всегда добавляйте его как displayName в операцию обновления.</span><span class="sxs-lookup"><span data-stu-id="dc06a-159">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="dc06a-160">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="dc06a-160">emailAddresses</span></span>|<span data-ttu-id="dc06a-161">Коллекция [типедемаиладдресс](../resources/typedemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="dc06a-161">[typedEmailAddress](../resources/typedemailaddress.md) collection</span></span>|<span data-ttu-id="dc06a-162">Электронные адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-162">The contact's email addresses.</span></span>|
|<span data-ttu-id="dc06a-163">fileAs</span><span class="sxs-lookup"><span data-stu-id="dc06a-163">fileAs</span></span>|<span data-ttu-id="dc06a-164">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-164">String</span></span>|<span data-ttu-id="dc06a-165">Имя, под которым хранится контакт.</span><span class="sxs-lookup"><span data-stu-id="dc06a-165">The name the contact is filed under.</span></span>|
|<span data-ttu-id="dc06a-166">gender</span><span class="sxs-lookup"><span data-stu-id="dc06a-166">gender</span></span> |<span data-ttu-id="dc06a-167">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-167">String</span></span> |<span data-ttu-id="dc06a-168">Пол контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-168">The contact's gender.</span></span> |
|<span data-ttu-id="dc06a-169">generation</span><span class="sxs-lookup"><span data-stu-id="dc06a-169">generation</span></span>|<span data-ttu-id="dc06a-170">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-170">String</span></span>|<span data-ttu-id="dc06a-171">Поколение контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-171">The contact's generation.</span></span>|
|<span data-ttu-id="dc06a-172">givenName</span><span class="sxs-lookup"><span data-stu-id="dc06a-172">givenName</span></span>|<span data-ttu-id="dc06a-173">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-173">String</span></span>|<span data-ttu-id="dc06a-174">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-174">The contact's given name.</span></span>|
|<span data-ttu-id="dc06a-175">imAddresses</span><span class="sxs-lookup"><span data-stu-id="dc06a-175">imAddresses</span></span>|<span data-ttu-id="dc06a-176">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-176">String</span></span>|<span data-ttu-id="dc06a-177">Адреса контакта для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="dc06a-177">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="dc06a-178">initials</span><span class="sxs-lookup"><span data-stu-id="dc06a-178">initials</span></span>|<span data-ttu-id="dc06a-179">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-179">String</span></span>|<span data-ttu-id="dc06a-180">Инициалы контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-180">The contact's initials.</span></span>|
|<span data-ttu-id="dc06a-181">jobTitle</span><span class="sxs-lookup"><span data-stu-id="dc06a-181">jobTitle</span></span>|<span data-ttu-id="dc06a-182">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-182">String</span></span>|<span data-ttu-id="dc06a-183">Должность контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-183">The contact’s job title.</span></span>|
|<span data-ttu-id="dc06a-184">manager</span><span class="sxs-lookup"><span data-stu-id="dc06a-184">manager</span></span>|<span data-ttu-id="dc06a-185">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-185">String</span></span>|<span data-ttu-id="dc06a-186">Имя руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-186">The name of the contact's manager.</span></span>
|<span data-ttu-id="dc06a-187">middleName</span><span class="sxs-lookup"><span data-stu-id="dc06a-187">middleName</span></span>|<span data-ttu-id="dc06a-188">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-188">String</span></span>|<span data-ttu-id="dc06a-189">Отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-189">The contact's middle name.</span></span>|
|<span data-ttu-id="dc06a-190">nickName</span><span class="sxs-lookup"><span data-stu-id="dc06a-190">nickName</span></span>|<span data-ttu-id="dc06a-191">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-191">String</span></span>|<span data-ttu-id="dc06a-192">Псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-192">The contact's nickname.</span></span>|
|<span data-ttu-id="dc06a-193">officeLocation</span><span class="sxs-lookup"><span data-stu-id="dc06a-193">officeLocation</span></span>|<span data-ttu-id="dc06a-194">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-194">String</span></span>|<span data-ttu-id="dc06a-195">Расположение офиса контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-195">The location of the contact's office.</span></span>|
|<span data-ttu-id="dc06a-196">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="dc06a-196">parentFolderId</span></span>|<span data-ttu-id="dc06a-197">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-197">String</span></span>|<span data-ttu-id="dc06a-198">Идентификатор родительской папки контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-198">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="dc06a-199">personalNotes</span><span class="sxs-lookup"><span data-stu-id="dc06a-199">personalNotes</span></span>|<span data-ttu-id="dc06a-200">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-200">String</span></span>|<span data-ttu-id="dc06a-201">Заметки пользователя о контакте.</span><span class="sxs-lookup"><span data-stu-id="dc06a-201">The user's notes about the contact.</span></span>|
|<span data-ttu-id="dc06a-202">phones</span><span class="sxs-lookup"><span data-stu-id="dc06a-202">phones</span></span> |<span data-ttu-id="dc06a-203">Коллекция [phone](../resources/phone.md)</span><span class="sxs-lookup"><span data-stu-id="dc06a-203">[phone](../resources/phone.md) collection</span></span> |<span data-ttu-id="dc06a-204">Номера телефонов, связанные с контактом, например домашний телефон, мобильный телефон и служебный телефон.</span><span class="sxs-lookup"><span data-stu-id="dc06a-204">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="dc06a-205">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="dc06a-205">postalAddresses</span></span> |<span data-ttu-id="dc06a-206">Коллекция [physicalAddress](../resources/physicaladdress.md)</span><span class="sxs-lookup"><span data-stu-id="dc06a-206">[physicalAddress](../resources/physicaladdress.md) collection</span></span> |<span data-ttu-id="dc06a-207">Адреса, связанные с контактом, например домашний адрес и служебный адрес.</span><span class="sxs-lookup"><span data-stu-id="dc06a-207">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="dc06a-208">profession</span><span class="sxs-lookup"><span data-stu-id="dc06a-208">profession</span></span>|<span data-ttu-id="dc06a-209">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-209">String</span></span>|<span data-ttu-id="dc06a-210">Профессия контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-210">The contact's profession.</span></span>|
|<span data-ttu-id="dc06a-211">spouseName</span><span class="sxs-lookup"><span data-stu-id="dc06a-211">spouseName</span></span>|<span data-ttu-id="dc06a-212">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-212">String</span></span>|<span data-ttu-id="dc06a-213">Имя супруга или супруги контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-213">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="dc06a-214">surname</span><span class="sxs-lookup"><span data-stu-id="dc06a-214">surname</span></span>|<span data-ttu-id="dc06a-215">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-215">String</span></span>|<span data-ttu-id="dc06a-216">Фамилия контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-216">The contact's surname.</span></span>|
|<span data-ttu-id="dc06a-217">title</span><span class="sxs-lookup"><span data-stu-id="dc06a-217">title</span></span>|<span data-ttu-id="dc06a-218">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-218">String</span></span>|<span data-ttu-id="dc06a-219">Звание контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-219">The contact's title.</span></span>|
|<span data-ttu-id="dc06a-220">websites</span><span class="sxs-lookup"><span data-stu-id="dc06a-220">websites</span></span> |<span data-ttu-id="dc06a-221">Коллекция [website](../resources/website.md)</span><span class="sxs-lookup"><span data-stu-id="dc06a-221">[website](../resources/website.md) collection</span></span>|<span data-ttu-id="dc06a-222">Веб-сайты, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="dc06a-222">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="dc06a-223">веддинганниверсари</span><span class="sxs-lookup"><span data-stu-id="dc06a-223">weddingAnniversary</span></span> |<span data-ttu-id="dc06a-224">Дата</span><span class="sxs-lookup"><span data-stu-id="dc06a-224">Date</span></span> |<span data-ttu-id="dc06a-225">Годовщина свадьбы контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-225">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="dc06a-226">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="dc06a-226">yomiCompanyName</span></span>|<span data-ttu-id="dc06a-227">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-227">String</span></span>|<span data-ttu-id="dc06a-p107">Название компании контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="dc06a-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="dc06a-230">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="dc06a-230">yomiGivenName</span></span>|<span data-ttu-id="dc06a-231">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-231">String</span></span>|<span data-ttu-id="dc06a-p108">Имя контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="dc06a-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="dc06a-234">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="dc06a-234">yomiSurname</span></span>|<span data-ttu-id="dc06a-235">String</span><span class="sxs-lookup"><span data-stu-id="dc06a-235">String</span></span>|<span data-ttu-id="dc06a-p109">Фамилия контакта, записанная так, как она звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="dc06a-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

<span data-ttu-id="dc06a-238">Так как **контактный** ресурс поддерживает [расширения](/graph/extensibility-overview), с помощью операции можно `PATCH` добавлять, обновлять или удалять собственные данные, относящиеся к приложению, в пользовательских свойствах расширения в существующем экземпляре **контакта** .</span><span class="sxs-lookup"><span data-stu-id="dc06a-238">Since the **contact** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **contact** instance.</span></span>

## <a name="response"></a><span data-ttu-id="dc06a-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc06a-239">Response</span></span>

<span data-ttu-id="dc06a-240">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dc06a-240">If successful, this method returns a `200 OK` response code and updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dc06a-241">Пример</span><span class="sxs-lookup"><span data-stu-id="dc06a-241">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc06a-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc06a-242">Request</span></span>
<span data-ttu-id="dc06a-243">В следующем примере обновляется личный адрес электронной почты указанного контакта.</span><span class="sxs-lookup"><span data-stu-id="dc06a-243">The following example updates the personal email address of the specified contact.</span></span>

# <a name="http"></a>[<span data-ttu-id="dc06a-244">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc06a-244">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dc06a-245">C#</span><span class="sxs-lookup"><span data-stu-id="dc06a-245">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc06a-246">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc06a-246">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc06a-247">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc06a-247">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dc06a-248">Java</span><span class="sxs-lookup"><span data-stu-id="dc06a-248">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dc06a-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc06a-249">Response</span></span>
<span data-ttu-id="dc06a-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc06a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="dc06a-253">См. также</span><span class="sxs-lookup"><span data-stu-id="dc06a-253">See also</span></span>

- [<span data-ttu-id="dc06a-254">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="dc06a-254">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="dc06a-255">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="dc06a-255">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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


