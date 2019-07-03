---
title: Список childFolders
description: 'Получение коллекции папок в указанной папке. Вы можете использовать короткий путь `.../me/MailFolders` для получения верхнего уровня '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 50b5a36d2529e295a4876e851cf89459cc386a77
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445298"
---
# <a name="list-childfolders"></a><span data-ttu-id="3c355-104">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="3c355-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c355-p102">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/mailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="3c355-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c355-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c355-107">Permissions</span></span>

<span data-ttu-id="3c355-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c355-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3c355-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c355-110">Permission type</span></span>                        | <span data-ttu-id="3c355-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c355-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="3c355-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c355-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c355-113">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c355-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="3c355-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c355-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c355-115">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c355-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="3c355-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c355-116">Application</span></span>                            | <span data-ttu-id="3c355-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c355-117">Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="3c355-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c355-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c355-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3c355-119">Optional query parameters</span></span>

<span data-ttu-id="3c355-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3c355-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c355-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c355-121">Request headers</span></span>

| <span data-ttu-id="3c355-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3c355-122">Name</span></span>          | <span data-ttu-id="3c355-123">Тип</span><span class="sxs-lookup"><span data-stu-id="3c355-123">Type</span></span>   | <span data-ttu-id="3c355-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3c355-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="3c355-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c355-125">Authorization</span></span> | <span data-ttu-id="3c355-126">string</span><span class="sxs-lookup"><span data-stu-id="3c355-126">string</span></span> | <span data-ttu-id="3c355-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c355-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c355-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c355-129">Request body</span></span>

<span data-ttu-id="3c355-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c355-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c355-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c355-131">Response</span></span>

<span data-ttu-id="3c355-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c355-132">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c355-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="3c355-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="3c355-134">Пример 1: список почтовых папок</span><span class="sxs-lookup"><span data-stu-id="3c355-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="3c355-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c355-135">Request</span></span>

<span data-ttu-id="3c355-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c355-136">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3c355-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c355-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c355-138">C#</span><span class="sxs-lookup"><span data-stu-id="3c355-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c355-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c355-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c355-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3c355-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="3c355-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c355-141">Response</span></span>

<span data-ttu-id="3c355-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3c355-142">The following is an example of the response.</span></span>

> <span data-ttu-id="3c355-143">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3c355-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3c355-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c355-144">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="3c355-145">Пример 2: список папок поиска почты</span><span class="sxs-lookup"><span data-stu-id="3c355-145">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="3c355-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c355-146">Request</span></span>

<span data-ttu-id="3c355-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c355-147">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3c355-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c355-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c355-149">C#</span><span class="sxs-lookup"><span data-stu-id="3c355-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-of-searchfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c355-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c355-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-of-searchfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c355-151">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3c355-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-of-searchfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3c355-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c355-152">Response</span></span>

<span data-ttu-id="3c355-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3c355-153">The following is an example of the response.</span></span>

> <span data-ttu-id="3c355-154">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3c355-154">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3c355-155">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c355-155">All the properties will be returned from an actual call.</span></span>

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
