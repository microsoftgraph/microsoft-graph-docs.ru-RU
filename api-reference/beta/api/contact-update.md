---
title: Обновление контакта
description: Обновление свойств объекта Contact.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e8e1bb9332ca6a5821e0c17d12060a9f4044a983
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863359"
---
# <a name="update-contact"></a><span data-ttu-id="5de96-103">Обновление контакта</span><span class="sxs-lookup"><span data-stu-id="5de96-103">Update contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5de96-104">Обновление свойств объекта Contact.</span><span class="sxs-lookup"><span data-stu-id="5de96-104">Update the properties of contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5de96-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5de96-105">Permissions</span></span>
<span data-ttu-id="5de96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5de96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5de96-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5de96-108">Permission type</span></span>      | <span data-ttu-id="5de96-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5de96-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5de96-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5de96-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5de96-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5de96-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5de96-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5de96-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5de96-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5de96-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5de96-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5de96-114">Application</span></span> | <span data-ttu-id="5de96-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5de96-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5de96-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5de96-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="5de96-117">[Контакт](../resources/contact.md) от [contactFolder](../resources/contactfolder.md)пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5de96-117">A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="5de96-118">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="5de96-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="5de96-119">Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="5de96-119">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="5de96-120">Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="5de96-120">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5de96-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5de96-121">Request headers</span></span>
| <span data-ttu-id="5de96-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5de96-122">Header</span></span>       | <span data-ttu-id="5de96-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5de96-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5de96-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5de96-124">Authorization</span></span>  | <span data-ttu-id="5de96-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5de96-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5de96-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5de96-127">Content-Type</span></span>  | <span data-ttu-id="5de96-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5de96-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5de96-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5de96-130">Request body</span></span>
<span data-ttu-id="5de96-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5de96-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5de96-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="5de96-134">Property</span></span>     | <span data-ttu-id="5de96-135">Тип</span><span class="sxs-lookup"><span data-stu-id="5de96-135">Type</span></span>   |<span data-ttu-id="5de96-136">Описание</span><span class="sxs-lookup"><span data-stu-id="5de96-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5de96-137">assistantName</span><span class="sxs-lookup"><span data-stu-id="5de96-137">assistantName</span></span>|<span data-ttu-id="5de96-138">String</span><span class="sxs-lookup"><span data-stu-id="5de96-138">String</span></span>|<span data-ttu-id="5de96-139">Имя помощника контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-139">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="5de96-140">birthday</span><span class="sxs-lookup"><span data-stu-id="5de96-140">birthday</span></span>|<span data-ttu-id="5de96-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5de96-141">DateTimeOffset</span></span>|<span data-ttu-id="5de96-142">Дата рождения контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-142">The contact's birthday.</span></span>|
|<span data-ttu-id="5de96-143">categories</span><span class="sxs-lookup"><span data-stu-id="5de96-143">categories</span></span>|<span data-ttu-id="5de96-144">String</span><span class="sxs-lookup"><span data-stu-id="5de96-144">String</span></span>|<span data-ttu-id="5de96-145">Категории, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="5de96-145">The categories associated with the contact.</span></span>|
|<span data-ttu-id="5de96-146">children</span><span class="sxs-lookup"><span data-stu-id="5de96-146">children</span></span>|<span data-ttu-id="5de96-147">String</span><span class="sxs-lookup"><span data-stu-id="5de96-147">String</span></span>||
|<span data-ttu-id="5de96-148">companyName</span><span class="sxs-lookup"><span data-stu-id="5de96-148">companyName</span></span>|<span data-ttu-id="5de96-149">String</span><span class="sxs-lookup"><span data-stu-id="5de96-149">String</span></span>|<span data-ttu-id="5de96-150">Название компании контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-150">The name of the contact's company.</span></span>|
|<span data-ttu-id="5de96-151">department</span><span class="sxs-lookup"><span data-stu-id="5de96-151">department</span></span>|<span data-ttu-id="5de96-152">String</span><span class="sxs-lookup"><span data-stu-id="5de96-152">String</span></span>|<span data-ttu-id="5de96-153">Отдел контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-153">The contact's department.</span></span>|
|<span data-ttu-id="5de96-154">displayName</span><span class="sxs-lookup"><span data-stu-id="5de96-154">displayName</span></span>|<span data-ttu-id="5de96-155">Строка</span><span class="sxs-lookup"><span data-stu-id="5de96-155">String</span></span>|<span data-ttu-id="5de96-156">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-156">The contact's display name.</span></span> <span data-ttu-id="5de96-157">Обратите внимание, что последующие обновления других свойств могут привести к тому, что автоматически созданное значение перезапишет указанное значение displayName.</span><span class="sxs-lookup"><span data-stu-id="5de96-157">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="5de96-158">Чтобы сохранить существующее значение, всегда добавляйте его как displayName в операцию обновления.</span><span class="sxs-lookup"><span data-stu-id="5de96-158">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="5de96-159">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="5de96-159">emailAddresses</span></span>|<span data-ttu-id="5de96-160">Коллекция [типедемаиладдресс](../resources/typedemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="5de96-160">[typedEmailAddress](../resources/typedemailaddress.md) collection</span></span>|<span data-ttu-id="5de96-161">Электронные адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-161">The contact's email addresses.</span></span>|
|<span data-ttu-id="5de96-162">fileAs</span><span class="sxs-lookup"><span data-stu-id="5de96-162">fileAs</span></span>|<span data-ttu-id="5de96-163">String</span><span class="sxs-lookup"><span data-stu-id="5de96-163">String</span></span>|<span data-ttu-id="5de96-164">Имя, под которым хранится контакт.</span><span class="sxs-lookup"><span data-stu-id="5de96-164">The name the contact is filed under.</span></span>|
|<span data-ttu-id="5de96-165">gender</span><span class="sxs-lookup"><span data-stu-id="5de96-165">gender</span></span> |<span data-ttu-id="5de96-166">String</span><span class="sxs-lookup"><span data-stu-id="5de96-166">String</span></span> |<span data-ttu-id="5de96-167">Пол контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-167">The contact's gender.</span></span> |
|<span data-ttu-id="5de96-168">generation</span><span class="sxs-lookup"><span data-stu-id="5de96-168">generation</span></span>|<span data-ttu-id="5de96-169">String</span><span class="sxs-lookup"><span data-stu-id="5de96-169">String</span></span>|<span data-ttu-id="5de96-170">Поколение контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-170">The contact's generation.</span></span>|
|<span data-ttu-id="5de96-171">givenName</span><span class="sxs-lookup"><span data-stu-id="5de96-171">givenName</span></span>|<span data-ttu-id="5de96-172">String</span><span class="sxs-lookup"><span data-stu-id="5de96-172">String</span></span>|<span data-ttu-id="5de96-173">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-173">The contact's given name.</span></span>|
|<span data-ttu-id="5de96-174">imAddresses</span><span class="sxs-lookup"><span data-stu-id="5de96-174">imAddresses</span></span>|<span data-ttu-id="5de96-175">String</span><span class="sxs-lookup"><span data-stu-id="5de96-175">String</span></span>|<span data-ttu-id="5de96-176">Адреса контакта для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="5de96-176">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="5de96-177">initials</span><span class="sxs-lookup"><span data-stu-id="5de96-177">initials</span></span>|<span data-ttu-id="5de96-178">String</span><span class="sxs-lookup"><span data-stu-id="5de96-178">String</span></span>|<span data-ttu-id="5de96-179">Инициалы контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-179">The contact's initials.</span></span>|
|<span data-ttu-id="5de96-180">jobTitle</span><span class="sxs-lookup"><span data-stu-id="5de96-180">jobTitle</span></span>|<span data-ttu-id="5de96-181">String</span><span class="sxs-lookup"><span data-stu-id="5de96-181">String</span></span>|<span data-ttu-id="5de96-182">Должность контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-182">The contact’s job title.</span></span>|
|<span data-ttu-id="5de96-183">manager</span><span class="sxs-lookup"><span data-stu-id="5de96-183">manager</span></span>|<span data-ttu-id="5de96-184">String</span><span class="sxs-lookup"><span data-stu-id="5de96-184">String</span></span>|<span data-ttu-id="5de96-185">Имя руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-185">The name of the contact's manager.</span></span>
|<span data-ttu-id="5de96-186">middleName</span><span class="sxs-lookup"><span data-stu-id="5de96-186">middleName</span></span>|<span data-ttu-id="5de96-187">String</span><span class="sxs-lookup"><span data-stu-id="5de96-187">String</span></span>|<span data-ttu-id="5de96-188">Отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-188">The contact's middle name.</span></span>|
|<span data-ttu-id="5de96-189">nickName</span><span class="sxs-lookup"><span data-stu-id="5de96-189">nickName</span></span>|<span data-ttu-id="5de96-190">String</span><span class="sxs-lookup"><span data-stu-id="5de96-190">String</span></span>|<span data-ttu-id="5de96-191">Псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-191">The contact's nickname.</span></span>|
|<span data-ttu-id="5de96-192">officeLocation</span><span class="sxs-lookup"><span data-stu-id="5de96-192">officeLocation</span></span>|<span data-ttu-id="5de96-193">String</span><span class="sxs-lookup"><span data-stu-id="5de96-193">String</span></span>|<span data-ttu-id="5de96-194">Расположение офиса контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-194">The location of the contact's office.</span></span>|
|<span data-ttu-id="5de96-195">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="5de96-195">parentFolderId</span></span>|<span data-ttu-id="5de96-196">Строка</span><span class="sxs-lookup"><span data-stu-id="5de96-196">String</span></span>|<span data-ttu-id="5de96-197">Идентификатор родительской папки контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-197">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="5de96-198">personalNotes</span><span class="sxs-lookup"><span data-stu-id="5de96-198">personalNotes</span></span>|<span data-ttu-id="5de96-199">String</span><span class="sxs-lookup"><span data-stu-id="5de96-199">String</span></span>|<span data-ttu-id="5de96-200">Заметки пользователя о контакте.</span><span class="sxs-lookup"><span data-stu-id="5de96-200">The user's notes about the contact.</span></span>|
|<span data-ttu-id="5de96-201">phones</span><span class="sxs-lookup"><span data-stu-id="5de96-201">phones</span></span> |<span data-ttu-id="5de96-202">Коллекция [phone](../resources/phone.md)</span><span class="sxs-lookup"><span data-stu-id="5de96-202">[phone](../resources/phone.md) collection</span></span> |<span data-ttu-id="5de96-203">Номера телефонов, связанные с контактом, например домашний телефон, мобильный телефон и служебный телефон.</span><span class="sxs-lookup"><span data-stu-id="5de96-203">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="5de96-204">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="5de96-204">postalAddresses</span></span> |<span data-ttu-id="5de96-205">Коллекция [physicalAddress](../resources/physicaladdress.md)</span><span class="sxs-lookup"><span data-stu-id="5de96-205">[physicalAddress](../resources/physicaladdress.md) collection</span></span> |<span data-ttu-id="5de96-206">Адреса, связанные с контактом, например домашний адрес и служебный адрес.</span><span class="sxs-lookup"><span data-stu-id="5de96-206">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="5de96-207">profession</span><span class="sxs-lookup"><span data-stu-id="5de96-207">profession</span></span>|<span data-ttu-id="5de96-208">String</span><span class="sxs-lookup"><span data-stu-id="5de96-208">String</span></span>|<span data-ttu-id="5de96-209">Профессия контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-209">The contact's profession.</span></span>|
|<span data-ttu-id="5de96-210">spouseName</span><span class="sxs-lookup"><span data-stu-id="5de96-210">spouseName</span></span>|<span data-ttu-id="5de96-211">String</span><span class="sxs-lookup"><span data-stu-id="5de96-211">String</span></span>|<span data-ttu-id="5de96-212">Имя супруга или супруги контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-212">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="5de96-213">surname</span><span class="sxs-lookup"><span data-stu-id="5de96-213">surname</span></span>|<span data-ttu-id="5de96-214">String</span><span class="sxs-lookup"><span data-stu-id="5de96-214">String</span></span>|<span data-ttu-id="5de96-215">Фамилия контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-215">The contact's surname.</span></span>|
|<span data-ttu-id="5de96-216">title</span><span class="sxs-lookup"><span data-stu-id="5de96-216">title</span></span>|<span data-ttu-id="5de96-217">String</span><span class="sxs-lookup"><span data-stu-id="5de96-217">String</span></span>|<span data-ttu-id="5de96-218">Звание контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-218">The contact's title.</span></span>|
|<span data-ttu-id="5de96-219">websites</span><span class="sxs-lookup"><span data-stu-id="5de96-219">websites</span></span> |<span data-ttu-id="5de96-220">Коллекция [website](../resources/website.md)</span><span class="sxs-lookup"><span data-stu-id="5de96-220">[website](../resources/website.md) collection</span></span>|<span data-ttu-id="5de96-221">Веб-сайты, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="5de96-221">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="5de96-222">Веддинганниверсари</span><span class="sxs-lookup"><span data-stu-id="5de96-222">weddingAnniversary</span></span> |<span data-ttu-id="5de96-223">Дата</span><span class="sxs-lookup"><span data-stu-id="5de96-223">Date</span></span> |<span data-ttu-id="5de96-224">Годовщина свадьбы контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-224">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="5de96-225">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="5de96-225">yomiCompanyName</span></span>|<span data-ttu-id="5de96-226">String</span><span class="sxs-lookup"><span data-stu-id="5de96-226">String</span></span>|<span data-ttu-id="5de96-p107">Название компании контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="5de96-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="5de96-229">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="5de96-229">yomiGivenName</span></span>|<span data-ttu-id="5de96-230">String</span><span class="sxs-lookup"><span data-stu-id="5de96-230">String</span></span>|<span data-ttu-id="5de96-p108">Имя контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="5de96-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="5de96-233">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="5de96-233">yomiSurname</span></span>|<span data-ttu-id="5de96-234">String</span><span class="sxs-lookup"><span data-stu-id="5de96-234">String</span></span>|<span data-ttu-id="5de96-p109">Фамилия контакта, записанная так, как она звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="5de96-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

<span data-ttu-id="5de96-237">Так как **контактный** ресурс поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, относящиеся к приложению, в пользовательских свойствах расширения в существующем экземпляре **контакта** .</span><span class="sxs-lookup"><span data-stu-id="5de96-237">Since the **contact** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **contact** instance.</span></span>

## <a name="response"></a><span data-ttu-id="5de96-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="5de96-238">Response</span></span>

<span data-ttu-id="5de96-239">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5de96-239">If successful, this method returns a `200 OK` response code and updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5de96-240">Пример</span><span class="sxs-lookup"><span data-stu-id="5de96-240">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5de96-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="5de96-241">Request</span></span>
<span data-ttu-id="5de96-242">В следующем примере обновляется личный адрес электронной почты указанного контакта.</span><span class="sxs-lookup"><span data-stu-id="5de96-242">The following example updates the personal email address of the specified contact.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5de96-243">HTTP</span><span class="sxs-lookup"><span data-stu-id="5de96-243">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="5de96-244">C#</span><span class="sxs-lookup"><span data-stu-id="5de96-244">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5de96-245">Javascript</span><span class="sxs-lookup"><span data-stu-id="5de96-245">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5de96-246">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5de96-246">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5de96-247">Java</span><span class="sxs-lookup"><span data-stu-id="5de96-247">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5de96-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="5de96-248">Response</span></span>
<span data-ttu-id="5de96-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5de96-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="5de96-252">См. также</span><span class="sxs-lookup"><span data-stu-id="5de96-252">See also</span></span>

- [<span data-ttu-id="5de96-253">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="5de96-253">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5de96-254">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5de96-254">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
