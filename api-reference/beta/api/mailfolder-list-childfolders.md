---
title: Список childFolders
description: 'Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете перейти к верхнему уровню '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c42d214e9c099c8d732eb73b93d16b5392801138
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665268"
---
# <a name="list-childfolders"></a><span data-ttu-id="bd489-104">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="bd489-104">List childFolders</span></span>

<span data-ttu-id="bd489-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd489-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd489-p102">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/mailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="bd489-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

<span data-ttu-id="bd489-108">По умолчанию эта операция не возвращает скрытые папки.</span><span class="sxs-lookup"><span data-stu-id="bd489-108">By default, this operation does not return hidden folders.</span></span> <span data-ttu-id="bd489-109">Используйте параметр запроса _includeHiddenFolders_, чтобы включить их в отклик.</span><span class="sxs-lookup"><span data-stu-id="bd489-109">Use a query parameter _includeHiddenFolders_ to include them in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd489-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd489-110">Permissions</span></span>

<span data-ttu-id="bd489-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd489-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd489-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd489-113">Permission type</span></span>                        | <span data-ttu-id="bd489-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd489-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="bd489-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd489-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd489-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd489-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="bd489-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd489-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd489-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd489-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="bd489-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="bd489-119">Application</span></span>                            | <span data-ttu-id="bd489-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd489-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="bd489-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd489-121">HTTP request</span></span>

<span data-ttu-id="bd489-122">Чтобы получить все дочерние папки в указанной папке, за исключением скрытых:</span><span class="sxs-lookup"><span data-stu-id="bd489-122">To get all the child folders under the specified folder, excluding those that are hidden:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="bd489-123">Чтобы включить _скрытые_ дочерние папки в отклик:</span><span class="sxs-lookup"><span data-stu-id="bd489-123">To include _hidden_ child folders in the response:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders?includeHiddenFolders=true
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders?includeHiddenFolders=true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd489-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bd489-124">Optional query parameters</span></span>
<span data-ttu-id="bd489-125">Чтобы вернуть список всех объектов childFolder, включая скрытые (их свойство **isHidden** имеет значение true), в URL-адресе запроса укажите параметр запроса `includeHiddenFolders` как `true`, как показано в разделе [HTTP-запрос](#http-request).</span><span class="sxs-lookup"><span data-stu-id="bd489-125">To return a list of all childFolders including those that are hidden (their **isHidden** property is true), in the request URL, specify the `includeHiddenFolders` query parameter as `true`, as shown in the [HTTP request](#http-request) section.</span></span>

<span data-ttu-id="bd489-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bd489-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd489-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd489-127">Request headers</span></span>

| <span data-ttu-id="bd489-128">Имя</span><span class="sxs-lookup"><span data-stu-id="bd489-128">Name</span></span>          | <span data-ttu-id="bd489-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bd489-129">Type</span></span>   | <span data-ttu-id="bd489-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bd489-130">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="bd489-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd489-131">Authorization</span></span> | <span data-ttu-id="bd489-132">string</span><span class="sxs-lookup"><span data-stu-id="bd489-132">string</span></span> | <span data-ttu-id="bd489-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd489-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd489-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd489-135">Request body</span></span>

<span data-ttu-id="bd489-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd489-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd489-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd489-137">Response</span></span>

<span data-ttu-id="bd489-138">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd489-138">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd489-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="bd489-139">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="bd489-140">Пример 1. Перечисление папок почты</span><span class="sxs-lookup"><span data-stu-id="bd489-140">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="bd489-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd489-141">Request</span></span>

<span data-ttu-id="bd489-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd489-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bd489-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd489-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```
# <a name="c"></a>[<span data-ttu-id="bd489-144">C#</span><span class="sxs-lookup"><span data-stu-id="bd489-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd489-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd489-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd489-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd489-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd489-147">Java</span><span class="sxs-lookup"><span data-stu-id="bd489-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="bd489-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd489-148">Response</span></span>

<span data-ttu-id="bd489-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd489-149">The following is an example of the response.</span></span>

> <span data-ttu-id="bd489-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bd489-150">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "wellKnownName": null,
      "isHidden": false
    },
    {
      "id": "AAMkAGVmMDEzB",
      "displayName": "Project Falcon",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 5,
      "totalItemCount": 5,
      "wellKnownName": null,
      "isHidden": false
    },
    {
      "id": "AAMkAGVmMDEzMA",
      "displayName": "Finder",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 4,
      "unreadItemCount": 0,
      "totalItemCount": 0,
      "wellKnownName": "searchfolders",
      "isHidden": false
    }
  ]
}
```

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="bd489-151">Пример 2. Список папок поиска почты</span><span class="sxs-lookup"><span data-stu-id="bd489-151">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="bd489-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd489-152">Request</span></span>

<span data-ttu-id="bd489-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd489-153">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bd489-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd489-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```
# <a name="c"></a>[<span data-ttu-id="bd489-155">C#</span><span class="sxs-lookup"><span data-stu-id="bd489-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-of-searchfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd489-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd489-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-of-searchfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd489-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd489-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-of-searchfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd489-158">Java</span><span class="sxs-lookup"><span data-stu-id="bd489-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-childfolders-of-searchfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bd489-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd489-159">Response</span></span>

<span data-ttu-id="bd489-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd489-160">The following is an example of the response.</span></span>

> <span data-ttu-id="bd489-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bd489-161">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "isHidden": false,
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
      "isHidden": false,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'ACTION REQUIRED')"
    }
  ]
}
```

### <a name="example-3-include-hidden-child-folders-under-a-specified-mail-folder"></a><span data-ttu-id="bd489-162">Пример 3. Включай скрытые детские папки в указанную папку почты</span><span class="sxs-lookup"><span data-stu-id="bd489-162">Example 3: Include hidden child folders under a specified mail folder</span></span>

<span data-ttu-id="bd489-163">В следующем примере параметр запроса `includeHiddenFolders` используется для получения списка дочерних папок в указанной почтовой папке, включая скрытые почтовые папки.</span><span class="sxs-lookup"><span data-stu-id="bd489-163">The next example uses the `includeHiddenFolders` query parameter to get a list of child folders under a specified mail folder including hidden mail folders.</span></span> <span data-ttu-id="bd489-164">Отклик включает папку "Несрочные", параметру **isHidden** которой присвоено значение true.</span><span class="sxs-lookup"><span data-stu-id="bd489-164">The response includes the "Clutters" folder that has the **isHidden** set to true.</span></span>

#### <a name="request"></a><span data-ttu-id="bd489-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd489-165">Request</span></span>

<span data-ttu-id="bd489-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd489-166">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="bd489-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd489-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_hiddenchildfolders"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders?includeHiddenFolders=true
```
# <a name="c"></a>[<span data-ttu-id="bd489-168">C#</span><span class="sxs-lookup"><span data-stu-id="bd489-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-hiddenchildfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd489-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd489-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-hiddenchildfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd489-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd489-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-hiddenchildfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd489-171">Java</span><span class="sxs-lookup"><span data-stu-id="bd489-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-hiddenchildfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bd489-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd489-172">Response</span></span>

<span data-ttu-id="bd489-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd489-173">The following is an example of the response.</span></span>

> <span data-ttu-id="bd489-174">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bd489-174">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "wellKnownName": null,
      "isHidden": false
    },
    {
      "id": "AAMkAGVmMDEzB",
      "displayName": "Clutters",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 5,
      "totalItemCount": 5,
      "wellKnownName": null,
      "isHidden": true
    },
    {
      "id": "AAMkAGVmMDEzMA",
      "displayName": "Finder",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 4,
      "unreadItemCount": 0,
      "totalItemCount": 0,
      "wellKnownName": "searchfolders",
      "isHidden": false
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


