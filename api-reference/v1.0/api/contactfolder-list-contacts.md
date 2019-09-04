---
title: Список контактов
description: Получение коллекции контактов из стандартной папки с контактами для пользователя, выполнившего вход (`.../me/contacts`), или из указанной папки с контактами.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2140bcb2f7dada9a83d5754ba9cdcefc635c7522
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727161"
---
# <a name="list-contacts"></a><span data-ttu-id="a6359-103">Список контактов</span><span class="sxs-lookup"><span data-stu-id="a6359-103">List contacts</span></span>

<span data-ttu-id="a6359-104">Получение коллекции контактов из стандартной папки с контактами для пользователя, выполнившего вход (`.../me/contacts`), или из указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="a6359-104">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="a6359-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6359-105">Permissions</span></span>
<span data-ttu-id="a6359-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6359-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6359-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6359-108">Permission type</span></span>      | <span data-ttu-id="a6359-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6359-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6359-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6359-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a6359-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6359-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a6359-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6359-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6359-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6359-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a6359-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6359-114">Application</span></span> | <span data-ttu-id="a6359-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6359-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6359-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6359-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a6359-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a6359-117">Optional query parameters</span></span>
<span data-ttu-id="a6359-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a6359-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a6359-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6359-119">Request headers</span></span>
| <span data-ttu-id="a6359-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a6359-120">Name</span></span>       | <span data-ttu-id="a6359-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a6359-121">Type</span></span> | <span data-ttu-id="a6359-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a6359-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a6359-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6359-123">Authorization</span></span>  | <span data-ttu-id="a6359-124">string</span><span class="sxs-lookup"><span data-stu-id="a6359-124">string</span></span>  | <span data-ttu-id="a6359-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6359-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6359-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a6359-127">Request body</span></span>
<span data-ttu-id="a6359-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a6359-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6359-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6359-129">Response</span></span>

<span data-ttu-id="a6359-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a6359-130">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a6359-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a6359-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6359-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6359-132">Request</span></span>
<span data-ttu-id="a6359-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6359-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a6359-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6359-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a6359-135">C#</span><span class="sxs-lookup"><span data-stu-id="a6359-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a6359-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6359-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a6359-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a6359-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a6359-138">Java</span><span class="sxs-lookup"><span data-stu-id="a6359-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contactfolder-get-contacts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a6359-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6359-139">Response</span></span>
<span data-ttu-id="a6359-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6359-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
