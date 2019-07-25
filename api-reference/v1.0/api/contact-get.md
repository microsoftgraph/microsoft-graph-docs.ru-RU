---
title: Получение контакта
description: Получение свойств и связей объекта contact.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2f5b146d6fa47ed643a4ac1dc1a4a2e2650dcc8b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885143"
---
# <a name="get-contact"></a><span data-ttu-id="411d2-103">Получение контакта</span><span class="sxs-lookup"><span data-stu-id="411d2-103">Get contact</span></span>

<span data-ttu-id="411d2-104">Получение свойств и связей объекта contact.</span><span class="sxs-lookup"><span data-stu-id="411d2-104">Retrieve the properties and relationships of a contact object.</span></span>

<span data-ttu-id="411d2-105">Существует два сценария, в которых приложение может получить контакт в папке контактов другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="411d2-105">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="411d2-106">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="411d2-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="411d2-107">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой контактов или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="411d2-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="411d2-108">См. [подробные сведения и пример](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="411d2-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="411d2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="411d2-109">Permissions</span></span>
<span data-ttu-id="411d2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="411d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="411d2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="411d2-112">Permission type</span></span>      | <span data-ttu-id="411d2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="411d2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="411d2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="411d2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="411d2-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="411d2-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="411d2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="411d2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="411d2-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="411d2-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="411d2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="411d2-118">Application</span></span> | <span data-ttu-id="411d2-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="411d2-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="411d2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="411d2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="411d2-121">Объект [contact](../resources/contact.md) из стандартной пользовательской папки [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="411d2-121">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="411d2-122">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="411d2-122">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="411d2-p103">[Контакт](../resources/contact.md), содержащийся в дочерней папке объекта [contactFolder](../resources/mailfolder.md). В приведенном ниже примере показан один уровень вложенности, но контакт может храниться в папке, вложенной в дочернюю папку и т. д.</span><span class="sxs-lookup"><span data-stu-id="411d2-p103">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="411d2-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="411d2-125">Optional query parameters</span></span>
|<span data-ttu-id="411d2-126">Имя</span><span class="sxs-lookup"><span data-stu-id="411d2-126">Name</span></span>|<span data-ttu-id="411d2-127">Значение</span><span class="sxs-lookup"><span data-stu-id="411d2-127">Value</span></span>|<span data-ttu-id="411d2-128">Описание</span><span class="sxs-lookup"><span data-stu-id="411d2-128">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="411d2-129">$expand</span><span class="sxs-lookup"><span data-stu-id="411d2-129">$expand</span></span>|<span data-ttu-id="411d2-130">string</span><span class="sxs-lookup"><span data-stu-id="411d2-130">string</span></span>|<span data-ttu-id="411d2-p104">Разделенный запятыми список связей, развертываемых и включаемых в ответ. Поддерживаемые имена представлены в таблице связей объекта [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="411d2-p104">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="411d2-133">$select</span><span class="sxs-lookup"><span data-stu-id="411d2-133">$select</span></span>|<span data-ttu-id="411d2-134">string</span><span class="sxs-lookup"><span data-stu-id="411d2-134">string</span></span>|<span data-ttu-id="411d2-135">Разделенный запятыми список свойств, включаемых в ответ.</span><span class="sxs-lookup"><span data-stu-id="411d2-135">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="411d2-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="411d2-136">Request headers</span></span>
| <span data-ttu-id="411d2-137">Заголовок</span><span class="sxs-lookup"><span data-stu-id="411d2-137">Header</span></span>       | <span data-ttu-id="411d2-138">Значение</span><span class="sxs-lookup"><span data-stu-id="411d2-138">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="411d2-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="411d2-139">Authorization</span></span>  | <span data-ttu-id="411d2-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="411d2-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="411d2-142">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="411d2-142">Request body</span></span>
<span data-ttu-id="411d2-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="411d2-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="411d2-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="411d2-144">Response</span></span>

<span data-ttu-id="411d2-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="411d2-145">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="411d2-146">Пример</span><span class="sxs-lookup"><span data-stu-id="411d2-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="411d2-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="411d2-147">Request</span></span>
<span data-ttu-id="411d2-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="411d2-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="411d2-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="411d2-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="411d2-150">C#</span><span class="sxs-lookup"><span data-stu-id="411d2-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="411d2-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="411d2-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="411d2-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="411d2-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="411d2-153">Java</span><span class="sxs-lookup"><span data-stu-id="411d2-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="411d2-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="411d2-154">Response</span></span>
<span data-ttu-id="411d2-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="411d2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "homeAddress": {},
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
  "description": "Get contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
