---
title: Список childFolders
description: 'Получение коллекции папок в указанной папке. Вы можете использовать короткий путь `.../me/MailFolders` для получения верхнего уровня '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9cf1f5cd48a07cb6e240002b8715fc546b56136d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049277"
---
# <a name="list-childfolders"></a><span data-ttu-id="1cfe4-104">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="1cfe4-104">List childFolders</span></span>

<span data-ttu-id="1cfe4-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cfe4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cfe4-p102">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/mailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="1cfe4-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cfe4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1cfe4-108">Permissions</span></span>

<span data-ttu-id="1cfe4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cfe4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1cfe4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cfe4-111">Permission type</span></span>                        | <span data-ttu-id="1cfe4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cfe4-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="1cfe4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cfe4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1cfe4-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cfe4-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="1cfe4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cfe4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cfe4-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cfe4-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="1cfe4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1cfe4-117">Application</span></span>                            | <span data-ttu-id="1cfe4-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cfe4-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="1cfe4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cfe4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1cfe4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1cfe4-120">Optional query parameters</span></span>

<span data-ttu-id="1cfe4-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1cfe4-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1cfe4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1cfe4-122">Request headers</span></span>

| <span data-ttu-id="1cfe4-123">Имя</span><span class="sxs-lookup"><span data-stu-id="1cfe4-123">Name</span></span>          | <span data-ttu-id="1cfe4-124">Тип</span><span class="sxs-lookup"><span data-stu-id="1cfe4-124">Type</span></span>   | <span data-ttu-id="1cfe4-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1cfe4-125">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="1cfe4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cfe4-126">Authorization</span></span> | <span data-ttu-id="1cfe4-127">string</span><span class="sxs-lookup"><span data-stu-id="1cfe4-127">string</span></span> | <span data-ttu-id="1cfe4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cfe4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cfe4-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1cfe4-130">Request body</span></span>

<span data-ttu-id="1cfe4-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1cfe4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cfe4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cfe4-132">Response</span></span>

<span data-ttu-id="1cfe4-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1cfe4-133">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1cfe4-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="1cfe4-134">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="1cfe4-135">Пример 1. Список почтовых папок</span><span class="sxs-lookup"><span data-stu-id="1cfe4-135">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="1cfe4-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cfe4-136">Request</span></span>

<span data-ttu-id="1cfe4-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cfe4-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1cfe4-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cfe4-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```
# <a name="c"></a>[<span data-ttu-id="1cfe4-139">C#</span><span class="sxs-lookup"><span data-stu-id="1cfe4-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1cfe4-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cfe4-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1cfe4-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cfe4-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1cfe4-142">Java</span><span class="sxs-lookup"><span data-stu-id="1cfe4-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="1cfe4-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cfe4-143">Response</span></span>

<span data-ttu-id="1cfe4-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1cfe4-144">The following is an example of the response.</span></span>

> <span data-ttu-id="1cfe4-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1cfe4-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "AAMkAGVmMDEzA",
      "displayName": "Internal Screens",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 2,
      "totalItemCount": 2,
      "wellKnownName": null
    },
    {
      "id": "AAMkAGVmMDEzB",
      "displayName": "Project Falcon",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 5,
      "totalItemCount": 5,
      "wellKnownName": null
    },
    {
      "id": "AAMkAGVmMDEzMA",
      "displayName": "Finder",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 4,
      "unreadItemCount": 0,
      "totalItemCount": 0,
      "wellKnownName": "searchfolders"
    }
  ]
}
```

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="1cfe4-146">Пример 2. Список папок поиска почты</span><span class="sxs-lookup"><span data-stu-id="1cfe4-146">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="1cfe4-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cfe4-147">Request</span></span>

<span data-ttu-id="1cfe4-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cfe4-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1cfe4-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cfe4-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```
# <a name="c"></a>[<span data-ttu-id="1cfe4-150">C#</span><span class="sxs-lookup"><span data-stu-id="1cfe4-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-of-searchfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1cfe4-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cfe4-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-of-searchfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1cfe4-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cfe4-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-of-searchfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1cfe4-153">Java</span><span class="sxs-lookup"><span data-stu-id="1cfe4-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-childfolders-of-searchfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1cfe4-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cfe4-154">Response</span></span>

<span data-ttu-id="1cfe4-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1cfe4-155">The following is an example of the response.</span></span>

> <span data-ttu-id="1cfe4-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1cfe4-156">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailSearchFolder",
      "id": "AAMkAGE1NWMz",
      "displayName": "Get MyAnalytics",
      "parentFolderId": "AAMkAGE1NWMx",
      "childFolderCount": 0,
      "unreadItemCount": 6,
      "totalItemCount": 6,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'MyAnalytics')"
    },
    {
      "@odata.type": "#microsoft.graph.mailSearchFolder",
      "id": "AAMkAGE1NWMy",
      "displayName": "Action Required",
      "parentFolderId": "AAMkAGE1NWMx",
      "childFolderCount": 0,
      "unreadItemCount": 2,
      "totalItemCount": 4,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'ACTION REQUIRED')"
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


