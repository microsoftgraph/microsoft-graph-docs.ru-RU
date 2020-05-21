---
title: Список приложений
description: Получение списка приложений в организации.
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c8a837e3290ad273c58e5d407e9c6d26a1c53b74
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333245"
---
# <a name="list-applications"></a><span data-ttu-id="53c51-103">Список приложений</span><span class="sxs-lookup"><span data-stu-id="53c51-103">List applications</span></span>

<span data-ttu-id="53c51-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53c51-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53c51-105">Получение списка [приложений](../resources/application.md) в организации.</span><span class="sxs-lookup"><span data-stu-id="53c51-105">Get the list of [applications](../resources/application.md) in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="53c51-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53c51-106">Permissions</span></span>

<span data-ttu-id="53c51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53c51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53c51-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53c51-109">Permission type</span></span> | <span data-ttu-id="53c51-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53c51-110">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="53c51-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53c51-111">Delegated (work or school account)</span></span> | <span data-ttu-id="53c51-112">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="53c51-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="53c51-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53c51-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53c51-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53c51-114">Not supported.</span></span> |
| <span data-ttu-id="53c51-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53c51-115">Application</span></span> | <span data-ttu-id="53c51-116">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="53c51-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53c51-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53c51-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="53c51-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="53c51-118">Optional query parameters</span></span>

<span data-ttu-id="53c51-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, включая `$search` , `$count` и `$filter` .</span><span class="sxs-lookup"><span data-stu-id="53c51-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="53c51-120">Можно использовать `$search` свойство **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="53c51-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="53c51-121">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="53c51-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="53c51-122">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="53c51-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53c51-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53c51-123">Request headers</span></span>

| <span data-ttu-id="53c51-124">Имя</span><span class="sxs-lookup"><span data-stu-id="53c51-124">Name</span></span> | <span data-ttu-id="53c51-125">Описание</span><span class="sxs-lookup"><span data-stu-id="53c51-125">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="53c51-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53c51-126">Authorization</span></span>  | <span data-ttu-id="53c51-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53c51-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="53c51-129">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="53c51-129">ConsistencyLevel</span></span> | <span data-ttu-id="53c51-130">закончить.</span><span class="sxs-lookup"><span data-stu-id="53c51-130">eventual.</span></span> <span data-ttu-id="53c51-131">Этот заголовок и `$count` обязательные при использовании `$search` `$filter` с `$orderby` параметром Query.</span><span class="sxs-lookup"><span data-stu-id="53c51-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="53c51-132">Он использует индекс, который может быть не последним в актуальном изменении объекта.</span><span class="sxs-lookup"><span data-stu-id="53c51-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53c51-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="53c51-133">Request body</span></span>

<span data-ttu-id="53c51-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53c51-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53c51-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="53c51-135">Response</span></span>

<span data-ttu-id="53c51-136">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53c51-136">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53c51-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="53c51-137">Examples</span></span>

### <a name="example-1-get-the-list-of-applications"></a><span data-ttu-id="53c51-138">Пример 1: получение списка приложений</span><span class="sxs-lookup"><span data-stu-id="53c51-138">Example 1: Get the list of applications</span></span>

#### <a name="request"></a><span data-ttu-id="53c51-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="53c51-139">Request</span></span>

<span data-ttu-id="53c51-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53c51-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53c51-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="53c51-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications
```
# <a name="c"></a>[<span data-ttu-id="53c51-142">C#</span><span class="sxs-lookup"><span data-stu-id="53c51-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53c51-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53c51-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53c51-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53c51-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="53c51-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="53c51-145">Response</span></span>

<span data-ttu-id="53c51-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="53c51-146">Here is an example of the response.</span></span>
> <span data-ttu-id="53c51-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53c51-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications",
  "value": [
    {
      "appId": "00000000-0000-0000-0000-000000000000",
      "identifierUris": [ "http://contoso/" ],
      "displayName": "My app",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-applications"></a><span data-ttu-id="53c51-149">Пример 2: получение только количества приложений</span><span class="sxs-lookup"><span data-stu-id="53c51-149">Example 2: Get only a count of applications</span></span>

#### <a name="request"></a><span data-ttu-id="53c51-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="53c51-150">Request</span></span>

<span data-ttu-id="53c51-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53c51-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="53c51-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="53c51-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="53c51-153">C#</span><span class="sxs-lookup"><span data-stu-id="53c51-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53c51-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53c51-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53c51-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53c51-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="53c51-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="53c51-156">Response</span></span>

<span data-ttu-id="53c51-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="53c51-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="53c51-158">893</span><span class="sxs-lookup"><span data-stu-id="53c51-158">893</span></span>


### <a name="example-3-use-filter-and-top-to-get-one-application-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="53c51-159">Пример 3: используйте $filter и $top, чтобы получить одно приложение с отображаемым именем, начинающимся с "a", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="53c51-159">Example 3: Use $filter and $top to get one application with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="53c51-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="53c51-160">Request</span></span>

<span data-ttu-id="53c51-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53c51-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="53c51-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="53c51-162">Response</span></span>

<span data-ttu-id="53c51-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="53c51-163">The following is an example of the response.</span></span>
><span data-ttu-id="53c51-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53c51-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#applications",
  "@odata.count":1,
  "value":[
    {
      "appId": "00000000-0000-0000-0000-000000000000",
      "identifierUris": [ "http://contoso/" ],
      "displayName":"a",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-applications-with-display-names-that-contain-the-letters-web-including-a-count-of-returned-objects"></a><span data-ttu-id="53c51-166">Пример 4: использование $search для получения приложений с отображаемыми именами, содержащими "Web", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="53c51-166">Example 4: Use $search to get applications with display names that contain the letters 'Web' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="53c51-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="53c51-167">Request</span></span>

<span data-ttu-id="53c51-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53c51-168">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="53c51-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="53c51-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_web_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications?$search="displayName:Web"&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="53c51-170">C#</span><span class="sxs-lookup"><span data-stu-id="53c51-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-web-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53c51-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53c51-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-web-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53c51-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53c51-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-web-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="53c51-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="53c51-173">Response</span></span>

<span data-ttu-id="53c51-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="53c51-174">The following is an example of the response.</span></span>
><span data-ttu-id="53c51-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53c51-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#applications",
  "@odata.count":1396,
  "value":[
    {
      "appId": "00000000-0000-0000-0000-000000000000",
      "identifierUris": [ "http://contoso/" ],
      "displayName":"'DotNetWeb-App' ",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
