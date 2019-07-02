---
title: Список childFolders
description: 'Получение коллекции папок в указанной папке. Вы можете использовать короткий путь `.../me/MailFolders` для получения верхнего уровня '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 275f7bcd771db43f5d091848d9be8c50c6ddb124
ms.sourcegitcommit: ee710ff556f4a7907181df5c323e345f52808ce2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35417733"
---
# <a name="list-childfolders"></a><span data-ttu-id="bd83d-104">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="bd83d-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd83d-p102">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/mailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="bd83d-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd83d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd83d-107">Permissions</span></span>

<span data-ttu-id="bd83d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd83d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd83d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd83d-110">Permission type</span></span>                        | <span data-ttu-id="bd83d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd83d-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="bd83d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd83d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd83d-113">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd83d-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="bd83d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd83d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd83d-115">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd83d-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="bd83d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd83d-116">Application</span></span>                            | <span data-ttu-id="bd83d-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd83d-117">Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="bd83d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd83d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd83d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bd83d-119">Optional query parameters</span></span>

<span data-ttu-id="bd83d-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bd83d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd83d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd83d-121">Request headers</span></span>

| <span data-ttu-id="bd83d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="bd83d-122">Name</span></span>          | <span data-ttu-id="bd83d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="bd83d-123">Type</span></span>   | <span data-ttu-id="bd83d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="bd83d-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="bd83d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd83d-125">Authorization</span></span> | <span data-ttu-id="bd83d-126">string</span><span class="sxs-lookup"><span data-stu-id="bd83d-126">string</span></span> | <span data-ttu-id="bd83d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd83d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd83d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd83d-129">Request body</span></span>

<span data-ttu-id="bd83d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd83d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd83d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd83d-131">Response</span></span>

<span data-ttu-id="bd83d-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd83d-132">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd83d-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="bd83d-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="bd83d-134">Пример 1: список почтовых папок</span><span class="sxs-lookup"><span data-stu-id="bd83d-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="bd83d-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd83d-135">Request</span></span>

<span data-ttu-id="bd83d-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd83d-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="bd83d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd83d-137">Response</span></span>

<span data-ttu-id="bd83d-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd83d-138">The following is an example of the response.</span></span>

> <span data-ttu-id="bd83d-139">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bd83d-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bd83d-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd83d-140">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="bd83d-141">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="bd83d-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bd83d-142">C#</span><span class="sxs-lookup"><span data-stu-id="bd83d-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_childfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd83d-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="bd83d-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_childfolders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bd83d-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bd83d-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_childfolders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="bd83d-145">Пример 2: список папок поиска почты</span><span class="sxs-lookup"><span data-stu-id="bd83d-145">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="bd83d-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd83d-146">Request</span></span>

<span data-ttu-id="bd83d-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd83d-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response"></a><span data-ttu-id="bd83d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd83d-148">Response</span></span>

<span data-ttu-id="bd83d-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd83d-149">The following is an example of the response.</span></span>

> <span data-ttu-id="bd83d-150">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bd83d-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bd83d-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd83d-151">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="bd83d-152">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="bd83d-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bd83d-153">C#</span><span class="sxs-lookup"><span data-stu-id="bd83d-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_childfolders_of_searchfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd83d-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="bd83d-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_childfolders_of_searchfolders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bd83d-155">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bd83d-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_childfolders_of_searchfolders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
