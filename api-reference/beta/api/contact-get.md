---
title: Получение контакта
description: Извлечение свойств и связи контактного объекта.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e758a088400168ca755aae755054fcd57c1d092a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530120"
---
# <a name="get-contact"></a><span data-ttu-id="aae86-103">Получение контакта</span><span class="sxs-lookup"><span data-stu-id="aae86-103">Get contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aae86-104">Извлечение свойств и связи контактного объекта.</span><span class="sxs-lookup"><span data-stu-id="aae86-104">Retrieve the properties and relationships of contact object.</span></span>

<span data-ttu-id="aae86-105">Существует два сценария, где приложения можно получить контакт в папке контактов другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="aae86-105">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="aae86-106">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="aae86-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="aae86-107">Если приложение имеет соответствующей делегированных [разрешений](#permissions) от одного пользователя, и другой пользователь общей папке контактов с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="aae86-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="aae86-108">В разделе [сведения и примеры](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="aae86-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="aae86-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aae86-109">Permissions</span></span>
<span data-ttu-id="aae86-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aae86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aae86-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aae86-112">Permission type</span></span>      | <span data-ttu-id="aae86-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aae86-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aae86-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aae86-114">Delegated (work or school account)</span></span> | <span data-ttu-id="aae86-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aae86-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="aae86-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aae86-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aae86-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aae86-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="aae86-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aae86-118">Application</span></span> | <span data-ttu-id="aae86-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aae86-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="aae86-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aae86-120">HTTP request</span></span>
<span data-ttu-id="aae86-121"><!-- { "blockType": "ignored" } -->[Обратитесь](../resources/contact.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="aae86-121"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) in the user's mailbox.</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="aae86-122">[Обратитесь](../resources/contact.md) в верхнего уровня [contactFolder](../resources/contactfolder.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="aae86-122">A [contact](../resources/contact.md) from a top level [contactFolder](../resources/contactfolder.md) of the user's.</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="aae86-p103">[Контакт](../resources/contact.md), содержащийся в дочерней папке объекта [contactFolder](../resources/mailfolder.md). В приведенном ниже примере показан один уровень вложенности, но контакт может храниться в папке, вложенной в дочернюю папку и т. д.</span><span class="sxs-lookup"><span data-stu-id="aae86-p103">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aae86-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aae86-125">Optional query parameters</span></span>
|<span data-ttu-id="aae86-126">Имя</span><span class="sxs-lookup"><span data-stu-id="aae86-126">Name</span></span>|<span data-ttu-id="aae86-127">Значение</span><span class="sxs-lookup"><span data-stu-id="aae86-127">Value</span></span>|<span data-ttu-id="aae86-128">Описание</span><span class="sxs-lookup"><span data-stu-id="aae86-128">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="aae86-129">$expand</span><span class="sxs-lookup"><span data-stu-id="aae86-129">$expand</span></span>|<span data-ttu-id="aae86-130">string</span><span class="sxs-lookup"><span data-stu-id="aae86-130">string</span></span>|<span data-ttu-id="aae86-131">Список отношений, развертываемых и включаемых в ответ (разделитель — запятая).</span><span class="sxs-lookup"><span data-stu-id="aae86-131">Comma-separated list of relationships to expand and include in the response.</span></span> <span data-ttu-id="aae86-132">В разделе таблицы связей объекта [контактов](../resources/contact.md) для поддерживаемых имен.</span><span class="sxs-lookup"><span data-stu-id="aae86-132">See relationships table of [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="aae86-133">$select</span><span class="sxs-lookup"><span data-stu-id="aae86-133">$select</span></span>|<span data-ttu-id="aae86-134">string</span><span class="sxs-lookup"><span data-stu-id="aae86-134">string</span></span>|<span data-ttu-id="aae86-135">Разделенный запятыми список свойств, включаемых в ответ.</span><span class="sxs-lookup"><span data-stu-id="aae86-135">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="aae86-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aae86-136">Request headers</span></span>
| <span data-ttu-id="aae86-137">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aae86-137">Header</span></span>       | <span data-ttu-id="aae86-138">Значение</span><span class="sxs-lookup"><span data-stu-id="aae86-138">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aae86-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aae86-139">Authorization</span></span>  | <span data-ttu-id="aae86-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aae86-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aae86-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aae86-142">Request body</span></span>
<span data-ttu-id="aae86-143">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aae86-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aae86-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="aae86-144">Response</span></span>

<span data-ttu-id="aae86-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aae86-145">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aae86-146">Пример</span><span class="sxs-lookup"><span data-stu-id="aae86-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aae86-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="aae86-147">Request</span></span>
<span data-ttu-id="aae86-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aae86-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts/AAMkAGI2THk0AAA=
```
##### <a name="response"></a><span data-ttu-id="aae86-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="aae86-149">Response</span></span>
<span data-ttu-id="aae86-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="aae86-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="aae86-153">См. также</span><span class="sxs-lookup"><span data-stu-id="aae86-153">See also</span></span>

- [<span data-ttu-id="aae86-154">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="aae86-154">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="aae86-155">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="aae86-155">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/contact-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
