---
title: Список childFolders
description: Получение коллекции дочерних папок для указанной папки с контактами.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 93cb60dff296db767664c784c91395940f12e219
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003177"
---
# <a name="list-childfolders"></a><span data-ttu-id="d092f-103">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="d092f-103">List childFolders</span></span>

<span data-ttu-id="d092f-104">Получение коллекции дочерних папок для указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="d092f-104">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="d092f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d092f-105">Permissions</span></span>
<span data-ttu-id="d092f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d092f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d092f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d092f-108">Permission type</span></span>      | <span data-ttu-id="d092f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d092f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d092f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d092f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d092f-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d092f-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d092f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d092f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d092f-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d092f-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d092f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d092f-114">Application</span></span> | <span data-ttu-id="d092f-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d092f-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d092f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d092f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d092f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d092f-117">Optional query parameters</span></span>
<span data-ttu-id="d092f-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d092f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d092f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d092f-119">Request headers</span></span>
| <span data-ttu-id="d092f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d092f-120">Name</span></span>       | <span data-ttu-id="d092f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d092f-121">Type</span></span> | <span data-ttu-id="d092f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d092f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d092f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d092f-123">Authorization</span></span>  | <span data-ttu-id="d092f-124">string</span><span class="sxs-lookup"><span data-stu-id="d092f-124">string</span></span>  | <span data-ttu-id="d092f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d092f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d092f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d092f-127">Request body</span></span>
<span data-ttu-id="d092f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d092f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d092f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d092f-129">Response</span></span>

<span data-ttu-id="d092f-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d092f-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d092f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d092f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d092f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d092f-132">Request</span></span>
<span data-ttu-id="d092f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d092f-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d092f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d092f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d092f-135">C#</span><span class="sxs-lookup"><span data-stu-id="d092f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d092f-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="d092f-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d092f-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d092f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d092f-138">Java</span><span class="sxs-lookup"><span data-stu-id="d092f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contactfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d092f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d092f-139">Response</span></span>
<span data-ttu-id="d092f-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d092f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
