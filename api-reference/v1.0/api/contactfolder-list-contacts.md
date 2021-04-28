---
title: Список контактов
description: Получение коллекции контактов из стандартной папки с контактами для пользователя, выполнившего вход (`.../me/contacts`), или из указанной папки с контактами.
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 339f8ebcf4cac6cd29e582fca6b947c1b18d8d11
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051531"
---
# <a name="list-contacts"></a><span data-ttu-id="c5616-103">Список контактов</span><span class="sxs-lookup"><span data-stu-id="c5616-103">List contacts</span></span>

<span data-ttu-id="c5616-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5616-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c5616-105">Получение коллекции контактов из стандартной папки с контактами для пользователя, выполнившего вход (`.../me/contacts`), или из указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="c5616-105">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5616-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5616-106">Permissions</span></span>
<span data-ttu-id="c5616-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5616-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5616-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5616-109">Permission type</span></span>      | <span data-ttu-id="c5616-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5616-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5616-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5616-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c5616-112">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5616-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c5616-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5616-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5616-114">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5616-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c5616-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5616-115">Application</span></span> | <span data-ttu-id="c5616-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5616-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5616-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5616-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c5616-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c5616-118">Optional query parameters</span></span>
<span data-ttu-id="c5616-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c5616-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c5616-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5616-120">Request headers</span></span>
| <span data-ttu-id="c5616-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c5616-121">Name</span></span>       | <span data-ttu-id="c5616-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c5616-122">Type</span></span> | <span data-ttu-id="c5616-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c5616-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c5616-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5616-124">Authorization</span></span>  | <span data-ttu-id="c5616-125">string</span><span class="sxs-lookup"><span data-stu-id="c5616-125">string</span></span>  | <span data-ttu-id="c5616-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5616-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5616-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5616-128">Request body</span></span>
<span data-ttu-id="c5616-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5616-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5616-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5616-130">Response</span></span>

<span data-ttu-id="c5616-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5616-131">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5616-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c5616-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5616-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5616-133">Request</span></span>
<span data-ttu-id="c5616-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5616-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c5616-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5616-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
```
# <a name="c"></a>[<span data-ttu-id="c5616-136">C#</span><span class="sxs-lookup"><span data-stu-id="c5616-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5616-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5616-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5616-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5616-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5616-139">Java</span><span class="sxs-lookup"><span data-stu-id="c5616-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contactfolder-get-contacts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c5616-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5616-140">Response</span></span>
<span data-ttu-id="c5616-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c5616-141">Here is an example of the response.</span></span> <span data-ttu-id="c5616-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c5616-142">Note: The response object shown here might be shortened for readability.</span></span>
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
      "birthday": "datetime-value",
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
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
