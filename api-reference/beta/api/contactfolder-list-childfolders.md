---
title: Список childFolders
description: Получение коллекции дочерних папок для указанной папки с контактами.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2db187317a07202c13e22cd3c61800134f138134
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863269"
---
# <a name="list-childfolders"></a><span data-ttu-id="4bf0d-103">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="4bf0d-103">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bf0d-104">Получение коллекции дочерних папок для указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="4bf0d-104">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="4bf0d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4bf0d-105">Permissions</span></span>
<span data-ttu-id="4bf0d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bf0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bf0d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bf0d-108">Permission type</span></span>      | <span data-ttu-id="4bf0d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bf0d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bf0d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bf0d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4bf0d-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4bf0d-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4bf0d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bf0d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bf0d-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4bf0d-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4bf0d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bf0d-114">Application</span></span> | <span data-ttu-id="4bf0d-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4bf0d-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bf0d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bf0d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4bf0d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4bf0d-117">Optional query parameters</span></span>
<span data-ttu-id="4bf0d-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4bf0d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4bf0d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4bf0d-119">Request headers</span></span>
| <span data-ttu-id="4bf0d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4bf0d-120">Name</span></span>       | <span data-ttu-id="4bf0d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4bf0d-121">Type</span></span> | <span data-ttu-id="4bf0d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4bf0d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4bf0d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bf0d-123">Authorization</span></span>  | <span data-ttu-id="4bf0d-124">string</span><span class="sxs-lookup"><span data-stu-id="4bf0d-124">string</span></span>  | <span data-ttu-id="4bf0d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bf0d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bf0d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4bf0d-127">Request body</span></span>
<span data-ttu-id="4bf0d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4bf0d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bf0d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bf0d-129">Response</span></span>

<span data-ttu-id="4bf0d-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4bf0d-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4bf0d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4bf0d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4bf0d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bf0d-132">Request</span></span>
<span data-ttu-id="4bf0d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bf0d-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4bf0d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4bf0d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4bf0d-135">C#</span><span class="sxs-lookup"><span data-stu-id="4bf0d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4bf0d-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="4bf0d-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4bf0d-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4bf0d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4bf0d-138">Java</span><span class="sxs-lookup"><span data-stu-id="4bf0d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contactfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4bf0d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bf0d-139">Response</span></span>
<span data-ttu-id="4bf0d-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4bf0d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
