---
title: Список контактов
description: Получение всех контактов в почтовом ящике вошедшего пользователя (. ../ме/контактс) или из указанной папки контактов.
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fa660186ea9cdb34ba6586a1e932f740d51e5d26
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002935"
---
# <a name="list-contacts"></a><span data-ttu-id="116ad-103">Список контактов</span><span class="sxs-lookup"><span data-stu-id="116ad-103">List contacts</span></span>

<span data-ttu-id="116ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="116ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="116ad-105">Получение всех контактов в почтовом ящике вошедшего пользователя (. ../ме/контактс) или из указанной папки контактов.</span><span class="sxs-lookup"><span data-stu-id="116ad-105">Get all the contacts in the signed-in user's mailbox (.../me/contacts), or from the specified contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="116ad-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="116ad-106">Permissions</span></span>
<span data-ttu-id="116ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="116ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="116ad-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="116ad-109">Permission type</span></span>      | <span data-ttu-id="116ad-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="116ad-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="116ad-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="116ad-111">Delegated (work or school account)</span></span> | <span data-ttu-id="116ad-112">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="116ad-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="116ad-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="116ad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="116ad-114">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="116ad-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="116ad-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="116ad-115">Application</span></span> | <span data-ttu-id="116ad-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="116ad-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="116ad-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="116ad-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="116ad-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="116ad-118">Optional query parameters</span></span>
<span data-ttu-id="116ad-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="116ad-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="116ad-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="116ad-120">Request headers</span></span>
| <span data-ttu-id="116ad-121">Имя</span><span class="sxs-lookup"><span data-stu-id="116ad-121">Name</span></span>       | <span data-ttu-id="116ad-122">Тип</span><span class="sxs-lookup"><span data-stu-id="116ad-122">Type</span></span> | <span data-ttu-id="116ad-123">Описание</span><span class="sxs-lookup"><span data-stu-id="116ad-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="116ad-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="116ad-124">Authorization</span></span>  | <span data-ttu-id="116ad-125">string</span><span class="sxs-lookup"><span data-stu-id="116ad-125">string</span></span>  | <span data-ttu-id="116ad-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="116ad-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="116ad-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="116ad-128">Request body</span></span>
<span data-ttu-id="116ad-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="116ad-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="116ad-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="116ad-130">Response</span></span>

<span data-ttu-id="116ad-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="116ad-131">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="116ad-132">Пример</span><span class="sxs-lookup"><span data-stu-id="116ad-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="116ad-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="116ad-133">Request</span></span>
<span data-ttu-id="116ad-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="116ad-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="116ad-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="116ad-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
```
# <a name="c"></a>[<span data-ttu-id="116ad-136">C#</span><span class="sxs-lookup"><span data-stu-id="116ad-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="116ad-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="116ad-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="116ad-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="116ad-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="116ad-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="116ad-139">Response</span></span>
<span data-ttu-id="116ad-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="116ad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "2016-10-19T10:37:00Z",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


