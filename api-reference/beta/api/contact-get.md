---
title: Получение контакта
description: Извлечение свойств и связей контактного объекта.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: accc9f8f8b089a5c4dc8a46bd3129806a9795bd8
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472540"
---
# <a name="get-contact"></a><span data-ttu-id="a16f4-103">Вывод контакта</span><span class="sxs-lookup"><span data-stu-id="a16f4-103">Get contact</span></span>

<span data-ttu-id="a16f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a16f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a16f4-105">Извлечение свойств и связей контактного объекта.</span><span class="sxs-lookup"><span data-stu-id="a16f4-105">Retrieve the properties and relationships of contact object.</span></span>

<span data-ttu-id="a16f4-106">Существует два сценария, в которых приложение может получить контакт в папке контактов другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="a16f4-106">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="a16f4-107">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="a16f4-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="a16f4-108">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой контактов или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="a16f4-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="a16f4-109">См. [подробные сведения и пример](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="a16f4-109">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="a16f4-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a16f4-110">Permissions</span></span>
<span data-ttu-id="a16f4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a16f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a16f4-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a16f4-113">Permission type</span></span>      | <span data-ttu-id="a16f4-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a16f4-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a16f4-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a16f4-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a16f4-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a16f4-116">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a16f4-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a16f4-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a16f4-118">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a16f4-118">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a16f4-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a16f4-119">Application</span></span> | <span data-ttu-id="a16f4-120">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a16f4-120">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a16f4-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a16f4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a16f4-122">Контакт [в](../resources/contact.md) почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="a16f4-122">A [contact](../resources/contact.md) in the user's mailbox.</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="a16f4-123">Контакт [с](../resources/contact.md) верхнего уровня [contactFolder](../resources/contactfolder.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="a16f4-123">A [contact](../resources/contact.md) from a top level [contactFolder](../resources/contactfolder.md) of the user's.</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="a16f4-124">Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a16f4-124">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="a16f4-125">Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="a16f4-125">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a16f4-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a16f4-126">Optional query parameters</span></span>
|<span data-ttu-id="a16f4-127">Имя</span><span class="sxs-lookup"><span data-stu-id="a16f4-127">Name</span></span>|<span data-ttu-id="a16f4-128">Значение</span><span class="sxs-lookup"><span data-stu-id="a16f4-128">Value</span></span>|<span data-ttu-id="a16f4-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a16f4-129">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="a16f4-130">$expand</span><span class="sxs-lookup"><span data-stu-id="a16f4-130">$expand</span></span>|<span data-ttu-id="a16f4-131">string</span><span class="sxs-lookup"><span data-stu-id="a16f4-131">string</span></span>|<span data-ttu-id="a16f4-132">Список отношений, развертываемых и включаемых в ответ (разделитель — запятая).</span><span class="sxs-lookup"><span data-stu-id="a16f4-132">Comma-separated list of relationships to expand and include in the response.</span></span> <span data-ttu-id="a16f4-133">См. таблицу [связей контактного](../resources/contact.md) объекта для поддерживаемых имен.</span><span class="sxs-lookup"><span data-stu-id="a16f4-133">See relationships table of [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="a16f4-134">$select</span><span class="sxs-lookup"><span data-stu-id="a16f4-134">$select</span></span>|<span data-ttu-id="a16f4-135">string</span><span class="sxs-lookup"><span data-stu-id="a16f4-135">string</span></span>|<span data-ttu-id="a16f4-136">Разделенный запятыми список свойств, включаемых в ответ.</span><span class="sxs-lookup"><span data-stu-id="a16f4-136">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="a16f4-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a16f4-137">Request headers</span></span>
| <span data-ttu-id="a16f4-138">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a16f4-138">Header</span></span>       | <span data-ttu-id="a16f4-139">Значение</span><span class="sxs-lookup"><span data-stu-id="a16f4-139">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a16f4-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a16f4-140">Authorization</span></span>  | <span data-ttu-id="a16f4-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a16f4-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a16f4-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a16f4-143">Request body</span></span>
<span data-ttu-id="a16f4-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a16f4-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a16f4-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a16f4-145">Response</span></span>

<span data-ttu-id="a16f4-146">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a16f4-146">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a16f4-147">Пример</span><span class="sxs-lookup"><span data-stu-id="a16f4-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a16f4-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="a16f4-148">Request</span></span>
<span data-ttu-id="a16f4-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a16f4-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a16f4-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="a16f4-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contacts/AAMkAGI2THk0AAA=
```
# <a name="c"></a>[<span data-ttu-id="a16f4-151">C#</span><span class="sxs-lookup"><span data-stu-id="a16f4-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a16f4-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a16f4-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a16f4-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a16f4-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a16f4-154">Java</span><span class="sxs-lookup"><span data-stu-id="a16f4-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a16f4-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="a16f4-155">Response</span></span>
<span data-ttu-id="a16f4-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a16f4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com",
      "type": "unknown"
    },
    {
      "name": "Garth",
      "address": "garth@contoso.onmicrosoft.com",
      "type": "personal"
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
  "assistantName": null,
  "manager": null,
  "phones": [{
    "type": "business",
    "number": "+1 918 555 0101"
  }],
  "postalAddresses": [{
    "type": "business",
    "postOfficeBox": "P.O. Box 100",
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "countryOrRegion": "USA",
    "postalCode": "98121"
  }],
  "spouseName": null,
  "personalNotes": null,
  "children": [], 
  "gender": null,
  "websites": [{
      "type": "work",
      "address": "https://www.contoso.com",
      "name": "Contoso"
  }],
  "weddingAnniversary": null
}
```

## <a name="see-also"></a><span data-ttu-id="a16f4-159">См. также</span><span class="sxs-lookup"><span data-stu-id="a16f4-159">See also</span></span>

- [<span data-ttu-id="a16f4-160">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="a16f4-160">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a16f4-161">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="a16f4-161">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


