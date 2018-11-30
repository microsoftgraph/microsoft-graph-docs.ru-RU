---
title: Получение контакта
description: Извлечение свойств и связи контактного объекта.
ms.openlocfilehash: 41784971e4e74fe34c4d0f55b8b0139ce3356e79
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079478"
---
# <a name="get-contact"></a><span data-ttu-id="667b4-103">Получение контакта</span><span class="sxs-lookup"><span data-stu-id="667b4-103">Get contact</span></span>

> <span data-ttu-id="667b4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="667b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="667b4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="667b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="667b4-106">Извлечение свойств и связи контактного объекта.</span><span class="sxs-lookup"><span data-stu-id="667b4-106">Retrieve the properties and relationships of contact object.</span></span>

<span data-ttu-id="667b4-107">Существует два сценария, где приложения можно получить контакт в папке контактов другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="667b4-107">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="667b4-108">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="667b4-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="667b4-109">Если приложение имеет соответствующей делегированных [разрешений](#permissions) от одного пользователя, и другой пользователь общей папке контактов с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="667b4-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="667b4-110">В разделе [сведения и примеры](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="667b4-110">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="667b4-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="667b4-111">Permissions</span></span>
<span data-ttu-id="667b4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="667b4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="667b4-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="667b4-114">Permission type</span></span>      | <span data-ttu-id="667b4-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="667b4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="667b4-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="667b4-116">Delegated (work or school account)</span></span> | <span data-ttu-id="667b4-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="667b4-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="667b4-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="667b4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="667b4-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="667b4-119">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="667b4-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="667b4-120">Application</span></span> | <span data-ttu-id="667b4-121">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="667b4-121">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="667b4-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="667b4-122">HTTP request</span></span>
<span data-ttu-id="667b4-123"><!-- { "blockType": "ignored" } -->[Обратитесь](../resources/contact.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="667b4-123"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) in the user's mailbox.</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="667b4-124">[Обратитесь](../resources/contact.md) в верхнего уровня [contactFolder](../resources/contactfolder.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="667b4-124">A [contact](../resources/contact.md) from a top level [contactFolder](../resources/contactfolder.md) of the user's.</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="667b4-125">[Обратитесь](../resources/contact.md) в дочерней папкой [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="667b4-125">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="667b4-126">В приведенном ниже примере показана один уровень вложения, но контакт может быть найдена в дочерних дочернего и т. д.</span><span class="sxs-lookup"><span data-stu-id="667b4-126">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="667b4-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="667b4-127">Optional query parameters</span></span>
|<span data-ttu-id="667b4-128">Имя</span><span class="sxs-lookup"><span data-stu-id="667b4-128">Name</span></span>|<span data-ttu-id="667b4-129">Значение</span><span class="sxs-lookup"><span data-stu-id="667b4-129">Value</span></span>|<span data-ttu-id="667b4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="667b4-130">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="667b4-131">$expand</span><span class="sxs-lookup"><span data-stu-id="667b4-131">$expand</span></span>|<span data-ttu-id="667b4-132">string</span><span class="sxs-lookup"><span data-stu-id="667b4-132">string</span></span>|<span data-ttu-id="667b4-133">Список отношений, развертываемых и включаемых в ответ (разделитель — запятая).</span><span class="sxs-lookup"><span data-stu-id="667b4-133">Comma-separated list of relationships to expand and include in the response.</span></span> <span data-ttu-id="667b4-134">В разделе таблицы связей объекта [контактов](../resources/contact.md) для поддерживаемых имен.</span><span class="sxs-lookup"><span data-stu-id="667b4-134">See relationships table of [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="667b4-135">$select</span><span class="sxs-lookup"><span data-stu-id="667b4-135">$select</span></span>|<span data-ttu-id="667b4-136">string</span><span class="sxs-lookup"><span data-stu-id="667b4-136">string</span></span>|<span data-ttu-id="667b4-137">Разделенный запятыми список свойств, включаемых в ответ.</span><span class="sxs-lookup"><span data-stu-id="667b4-137">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="667b4-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="667b4-138">Request headers</span></span>
| <span data-ttu-id="667b4-139">Заголовок</span><span class="sxs-lookup"><span data-stu-id="667b4-139">Header</span></span>       | <span data-ttu-id="667b4-140">Значение</span><span class="sxs-lookup"><span data-stu-id="667b4-140">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="667b4-141">Авторизация</span><span class="sxs-lookup"><span data-stu-id="667b4-141">Authorization</span></span>  | <span data-ttu-id="667b4-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="667b4-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="667b4-144">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="667b4-144">Request body</span></span>
<span data-ttu-id="667b4-145">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="667b4-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="667b4-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="667b4-146">Response</span></span>

<span data-ttu-id="667b4-147">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="667b4-147">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="667b4-148">Пример</span><span class="sxs-lookup"><span data-stu-id="667b4-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="667b4-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="667b4-149">Request</span></span>
<span data-ttu-id="667b4-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="667b4-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts/AAMkAGI2THk0AAA=
```
##### <a name="response"></a><span data-ttu-id="667b4-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="667b4-151">Response</span></span>
<span data-ttu-id="667b4-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="667b4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="667b4-155">См. также</span><span class="sxs-lookup"><span data-stu-id="667b4-155">See also</span></span>

- [<span data-ttu-id="667b4-156">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="667b4-156">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="667b4-157">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="667b4-157">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->