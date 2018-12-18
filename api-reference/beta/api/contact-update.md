---
title: Обновление контакта
description: Обновляет свойства объекта контакта.
author: angelgolfer-ms
ms.openlocfilehash: d25efb55a090c4c0b5fa750b64a0b2a905327a76
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334106"
---
# <a name="update-contact"></a><span data-ttu-id="c042f-103">Обновление контакта</span><span class="sxs-lookup"><span data-stu-id="c042f-103">Update contact</span></span>

> <span data-ttu-id="c042f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c042f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c042f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c042f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c042f-106">Обновляет свойства объекта контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-106">Update the properties of contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c042f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c042f-107">Permissions</span></span>
<span data-ttu-id="c042f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c042f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c042f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c042f-110">Permission type</span></span>      | <span data-ttu-id="c042f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c042f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c042f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c042f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c042f-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c042f-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c042f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c042f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c042f-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c042f-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c042f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c042f-116">Application</span></span> | <span data-ttu-id="c042f-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c042f-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c042f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c042f-118">HTTP request</span></span>
<span data-ttu-id="c042f-119"><!-- { "blockType": "ignored" } -->[Обратитесь](../resources/contact.md) в пользователя по умолчанию [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c042f-119"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="c042f-120">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="c042f-120">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="c042f-121">[Обратитесь](../resources/contact.md) в дочерней папкой [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c042f-121">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="c042f-122">В приведенном ниже примере показана один уровень вложения, но контакт может быть найдена в дочерних дочернего и т. д.</span><span class="sxs-lookup"><span data-stu-id="c042f-122">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c042f-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c042f-123">Request headers</span></span>
| <span data-ttu-id="c042f-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c042f-124">Header</span></span>       | <span data-ttu-id="c042f-125">Значение</span><span class="sxs-lookup"><span data-stu-id="c042f-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c042f-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c042f-126">Authorization</span></span>  | <span data-ttu-id="c042f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c042f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c042f-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c042f-129">Content-Type</span></span>  | <span data-ttu-id="c042f-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c042f-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c042f-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c042f-132">Request body</span></span>
<span data-ttu-id="c042f-p106">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c042f-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c042f-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="c042f-136">Property</span></span>     | <span data-ttu-id="c042f-137">Тип</span><span class="sxs-lookup"><span data-stu-id="c042f-137">Type</span></span>   |<span data-ttu-id="c042f-138">Описание</span><span class="sxs-lookup"><span data-stu-id="c042f-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c042f-139">assistantName</span><span class="sxs-lookup"><span data-stu-id="c042f-139">assistantName</span></span>|<span data-ttu-id="c042f-140">String</span><span class="sxs-lookup"><span data-stu-id="c042f-140">String</span></span>|<span data-ttu-id="c042f-141">Имя помощника контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-141">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="c042f-142">birthday</span><span class="sxs-lookup"><span data-stu-id="c042f-142">birthday</span></span>|<span data-ttu-id="c042f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c042f-143">DateTimeOffset</span></span>|<span data-ttu-id="c042f-144">Дата рождения контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-144">The contact's birthday.</span></span>|
|<span data-ttu-id="c042f-145">categories</span><span class="sxs-lookup"><span data-stu-id="c042f-145">categories</span></span>|<span data-ttu-id="c042f-146">String</span><span class="sxs-lookup"><span data-stu-id="c042f-146">String</span></span>|<span data-ttu-id="c042f-147">Категории, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="c042f-147">The categories associated with the contact.</span></span>|
|<span data-ttu-id="c042f-148">children</span><span class="sxs-lookup"><span data-stu-id="c042f-148">children</span></span>|<span data-ttu-id="c042f-149">String</span><span class="sxs-lookup"><span data-stu-id="c042f-149">String</span></span>||
|<span data-ttu-id="c042f-150">companyName</span><span class="sxs-lookup"><span data-stu-id="c042f-150">companyName</span></span>|<span data-ttu-id="c042f-151">String</span><span class="sxs-lookup"><span data-stu-id="c042f-151">String</span></span>|<span data-ttu-id="c042f-152">Название компании контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-152">The name of the contact's company.</span></span>|
|<span data-ttu-id="c042f-153">department</span><span class="sxs-lookup"><span data-stu-id="c042f-153">department</span></span>|<span data-ttu-id="c042f-154">String</span><span class="sxs-lookup"><span data-stu-id="c042f-154">String</span></span>|<span data-ttu-id="c042f-155">Отдел контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-155">The contact's department.</span></span>|
|<span data-ttu-id="c042f-156">displayName</span><span class="sxs-lookup"><span data-stu-id="c042f-156">displayName</span></span>|<span data-ttu-id="c042f-157">String</span><span class="sxs-lookup"><span data-stu-id="c042f-157">String</span></span>|<span data-ttu-id="c042f-158">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-158">The contact's display name.</span></span> <span data-ttu-id="c042f-159">Обратите внимание, что более поздние обновления для других свойств может стать причиной автоматически подставленное значение для перезаписи значение displayName, заданные.</span><span class="sxs-lookup"><span data-stu-id="c042f-159">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="c042f-160">Чтобы сохранить существующие значения, всегда включите его в качестве displayName в операции обновления.</span><span class="sxs-lookup"><span data-stu-id="c042f-160">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="c042f-161">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="c042f-161">emailAddresses</span></span>|<span data-ttu-id="c042f-162">[typedEmailAddress](../resources/typedemailaddress.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c042f-162">[typedEmailAddress](../resources/typedemailaddress.md) collection</span></span>|<span data-ttu-id="c042f-163">Электронные адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-163">The contact's email addresses.</span></span>|
|<span data-ttu-id="c042f-164">fileAs</span><span class="sxs-lookup"><span data-stu-id="c042f-164">fileAs</span></span>|<span data-ttu-id="c042f-165">String</span><span class="sxs-lookup"><span data-stu-id="c042f-165">String</span></span>|<span data-ttu-id="c042f-166">Имя, под которым хранится контакт.</span><span class="sxs-lookup"><span data-stu-id="c042f-166">The name the contact is filed under.</span></span>|
|<span data-ttu-id="c042f-167">gender</span><span class="sxs-lookup"><span data-stu-id="c042f-167">gender</span></span> |<span data-ttu-id="c042f-168">String.</span><span class="sxs-lookup"><span data-stu-id="c042f-168">String</span></span> |<span data-ttu-id="c042f-169">Пол контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-169">The contact's gender.</span></span> |
|<span data-ttu-id="c042f-170">generation</span><span class="sxs-lookup"><span data-stu-id="c042f-170">generation</span></span>|<span data-ttu-id="c042f-171">String</span><span class="sxs-lookup"><span data-stu-id="c042f-171">String</span></span>|<span data-ttu-id="c042f-172">Поколение контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-172">The contact's generation.</span></span>|
|<span data-ttu-id="c042f-173">givenName</span><span class="sxs-lookup"><span data-stu-id="c042f-173">givenName</span></span>|<span data-ttu-id="c042f-174">String</span><span class="sxs-lookup"><span data-stu-id="c042f-174">String</span></span>|<span data-ttu-id="c042f-175">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-175">The contact's given name.</span></span>|
|<span data-ttu-id="c042f-176">imAddresses</span><span class="sxs-lookup"><span data-stu-id="c042f-176">imAddresses</span></span>|<span data-ttu-id="c042f-177">String</span><span class="sxs-lookup"><span data-stu-id="c042f-177">String</span></span>|<span data-ttu-id="c042f-178">Адреса контакта для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="c042f-178">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="c042f-179">initials</span><span class="sxs-lookup"><span data-stu-id="c042f-179">initials</span></span>|<span data-ttu-id="c042f-180">String</span><span class="sxs-lookup"><span data-stu-id="c042f-180">String</span></span>|<span data-ttu-id="c042f-181">Инициалы контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-181">The contact's initials.</span></span>|
|<span data-ttu-id="c042f-182">jobTitle</span><span class="sxs-lookup"><span data-stu-id="c042f-182">jobTitle</span></span>|<span data-ttu-id="c042f-183">String</span><span class="sxs-lookup"><span data-stu-id="c042f-183">String</span></span>|<span data-ttu-id="c042f-184">Должность контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-184">The contact’s job title.</span></span>|
|<span data-ttu-id="c042f-185">manager</span><span class="sxs-lookup"><span data-stu-id="c042f-185">manager</span></span>|<span data-ttu-id="c042f-186">String</span><span class="sxs-lookup"><span data-stu-id="c042f-186">String</span></span>|<span data-ttu-id="c042f-187">Имя руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-187">The name of the contact's manager.</span></span>
|<span data-ttu-id="c042f-188">middleName</span><span class="sxs-lookup"><span data-stu-id="c042f-188">middleName</span></span>|<span data-ttu-id="c042f-189">String</span><span class="sxs-lookup"><span data-stu-id="c042f-189">String</span></span>|<span data-ttu-id="c042f-190">Отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-190">The contact's middle name.</span></span>|
|<span data-ttu-id="c042f-191">nickName</span><span class="sxs-lookup"><span data-stu-id="c042f-191">nickName</span></span>|<span data-ttu-id="c042f-192">String</span><span class="sxs-lookup"><span data-stu-id="c042f-192">String</span></span>|<span data-ttu-id="c042f-193">Псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-193">The contact's nickname.</span></span>|
|<span data-ttu-id="c042f-194">officeLocation</span><span class="sxs-lookup"><span data-stu-id="c042f-194">officeLocation</span></span>|<span data-ttu-id="c042f-195">String</span><span class="sxs-lookup"><span data-stu-id="c042f-195">String</span></span>|<span data-ttu-id="c042f-196">Расположение офиса контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-196">The location of the contact's office.</span></span>|
|<span data-ttu-id="c042f-197">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="c042f-197">parentFolderId</span></span>|<span data-ttu-id="c042f-198">String</span><span class="sxs-lookup"><span data-stu-id="c042f-198">String</span></span>|<span data-ttu-id="c042f-199">Идентификатор родительской папки контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-199">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="c042f-200">personalNotes</span><span class="sxs-lookup"><span data-stu-id="c042f-200">personalNotes</span></span>|<span data-ttu-id="c042f-201">String</span><span class="sxs-lookup"><span data-stu-id="c042f-201">String</span></span>|<span data-ttu-id="c042f-202">Заметки пользователя о контакте.</span><span class="sxs-lookup"><span data-stu-id="c042f-202">The user's notes about the contact.</span></span>|
|<span data-ttu-id="c042f-203">phones</span><span class="sxs-lookup"><span data-stu-id="c042f-203">phones</span></span> |<span data-ttu-id="c042f-204">Коллекция [phone](../resources/phone.md)</span><span class="sxs-lookup"><span data-stu-id="c042f-204">[phone](../resources/phone.md) collection</span></span> |<span data-ttu-id="c042f-205">Номера телефонов, связанный с этим контактом, например домашний, мобильный телефон и рабочий телефон.</span><span class="sxs-lookup"><span data-stu-id="c042f-205">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="c042f-206">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="c042f-206">postalAddresses</span></span> |<span data-ttu-id="c042f-207">[physicalAddress](../resources/physicaladdress.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c042f-207">[physicalAddress](../resources/physicaladdress.md) collection</span></span> |<span data-ttu-id="c042f-208">Адреса, связанные с этим контактом, например домашний адрес и рабочего адреса.</span><span class="sxs-lookup"><span data-stu-id="c042f-208">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="c042f-209">profession</span><span class="sxs-lookup"><span data-stu-id="c042f-209">profession</span></span>|<span data-ttu-id="c042f-210">String</span><span class="sxs-lookup"><span data-stu-id="c042f-210">String</span></span>|<span data-ttu-id="c042f-211">Профессия контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-211">The contact's profession.</span></span>|
|<span data-ttu-id="c042f-212">spouseName</span><span class="sxs-lookup"><span data-stu-id="c042f-212">spouseName</span></span>|<span data-ttu-id="c042f-213">String</span><span class="sxs-lookup"><span data-stu-id="c042f-213">String</span></span>|<span data-ttu-id="c042f-214">Имя супруга или супруги контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-214">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="c042f-215">surname</span><span class="sxs-lookup"><span data-stu-id="c042f-215">surname</span></span>|<span data-ttu-id="c042f-216">String</span><span class="sxs-lookup"><span data-stu-id="c042f-216">String</span></span>|<span data-ttu-id="c042f-217">Фамилия контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-217">The contact's surname.</span></span>|
|<span data-ttu-id="c042f-218">title</span><span class="sxs-lookup"><span data-stu-id="c042f-218">title</span></span>|<span data-ttu-id="c042f-219">String</span><span class="sxs-lookup"><span data-stu-id="c042f-219">String</span></span>|<span data-ttu-id="c042f-220">Звание контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-220">The contact's title.</span></span>|
|<span data-ttu-id="c042f-221">websites</span><span class="sxs-lookup"><span data-stu-id="c042f-221">websites</span></span> |<span data-ttu-id="c042f-222">Коллекция [website](../resources/website.md)</span><span class="sxs-lookup"><span data-stu-id="c042f-222">[website](../resources/website.md) collection</span></span>|<span data-ttu-id="c042f-223">Веб-сайты, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="c042f-223">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="c042f-224">weddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="c042f-224">weddingAnniversary</span></span> |<span data-ttu-id="c042f-225">Date</span><span class="sxs-lookup"><span data-stu-id="c042f-225">Date</span></span> |<span data-ttu-id="c042f-226">Годовщина свадьбы контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-226">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="c042f-227">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="c042f-227">yomiCompanyName</span></span>|<span data-ttu-id="c042f-228">String</span><span class="sxs-lookup"><span data-stu-id="c042f-228">String</span></span>|<span data-ttu-id="c042f-p108">Название компании контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c042f-p108">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="c042f-231">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="c042f-231">yomiGivenName</span></span>|<span data-ttu-id="c042f-232">String</span><span class="sxs-lookup"><span data-stu-id="c042f-232">String</span></span>|<span data-ttu-id="c042f-p109">Имя контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c042f-p109">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="c042f-235">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="c042f-235">yomiSurname</span></span>|<span data-ttu-id="c042f-236">Строка</span><span class="sxs-lookup"><span data-stu-id="c042f-236">String</span></span>|<span data-ttu-id="c042f-p110">Фамилия контакта, записанная так, как она звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c042f-p110">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

<span data-ttu-id="c042f-239">Поскольку ресурсов **контактов** поддерживает [расширения](/graph/extensibility-overview), можно использовать `PATCH` операции для добавления, обновления или удаления данных конкретного приложения в настраиваемых свойств расширения в существующий экземпляр **контактов** .</span><span class="sxs-lookup"><span data-stu-id="c042f-239">Since the **contact** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **contact** instance.</span></span>

## <a name="response"></a><span data-ttu-id="c042f-240">Ответ</span><span class="sxs-lookup"><span data-stu-id="c042f-240">Response</span></span>

<span data-ttu-id="c042f-241">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные, [обратитесь в](../resources/contact.md) объект в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c042f-241">If successful, this method returns a `200 OK` response code and updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c042f-242">Пример</span><span class="sxs-lookup"><span data-stu-id="c042f-242">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c042f-243">Запрос</span><span class="sxs-lookup"><span data-stu-id="c042f-243">Request</span></span>
<span data-ttu-id="c042f-244">В следующем примере обновляются адрес электронной почты личного указанного контакта.</span><span class="sxs-lookup"><span data-stu-id="c042f-244">The following example updates the personal email address of the specified contact.</span></span>
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
##### <a name="response"></a><span data-ttu-id="c042f-245">Ответ</span><span class="sxs-lookup"><span data-stu-id="c042f-245">Response</span></span>
<span data-ttu-id="c042f-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c042f-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="c042f-249">См. также</span><span class="sxs-lookup"><span data-stu-id="c042f-249">See also</span></span>

- [<span data-ttu-id="c042f-250">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="c042f-250">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c042f-251">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="c042f-251">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->