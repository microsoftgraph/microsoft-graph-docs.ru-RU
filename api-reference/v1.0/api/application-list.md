---
title: Список приложений
description: Получение списка приложений в организации.
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fa6d2eaf1a9480976407d78c75152b8861d82297
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905604"
---
# <a name="list-applications"></a><span data-ttu-id="6067a-103">Список приложений</span><span class="sxs-lookup"><span data-stu-id="6067a-103">List applications</span></span>

<span data-ttu-id="6067a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6067a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6067a-105">Получение списка [приложений](../resources/application.md) в организации.</span><span class="sxs-lookup"><span data-stu-id="6067a-105">Get the list of [applications](../resources/application.md) in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="6067a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6067a-106">Permissions</span></span>
<span data-ttu-id="6067a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6067a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6067a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6067a-109">Permission type</span></span>      | <span data-ttu-id="6067a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6067a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6067a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6067a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6067a-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6067a-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6067a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6067a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6067a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6067a-114">Not supported.</span></span>    |
|<span data-ttu-id="6067a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6067a-115">Application</span></span> | <span data-ttu-id="6067a-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6067a-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6067a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6067a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6067a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6067a-118">Optional query parameters</span></span>

<span data-ttu-id="6067a-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="6067a-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="6067a-120">Вы можете использовать `$search` в свойствах **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="6067a-120">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="6067a-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="6067a-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="6067a-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="6067a-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6067a-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6067a-123">Request headers</span></span>

| <span data-ttu-id="6067a-124">Имя</span><span class="sxs-lookup"><span data-stu-id="6067a-124">Name</span></span>           | <span data-ttu-id="6067a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="6067a-125">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="6067a-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6067a-126">Authorization</span></span>  | <span data-ttu-id="6067a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6067a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6067a-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="6067a-129">ConsistencyLevel</span></span> | <span data-ttu-id="6067a-130">необязательный.</span><span class="sxs-lookup"><span data-stu-id="6067a-130">eventual.</span></span> <span data-ttu-id="6067a-131">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="6067a-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="6067a-132">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="6067a-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6067a-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6067a-133">Request body</span></span>
<span data-ttu-id="6067a-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6067a-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6067a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6067a-135">Response</span></span>

<span data-ttu-id="6067a-136">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6067a-136">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6067a-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="6067a-137">Examples</span></span>

### <a name="example-1-get-the-list-of-applications"></a><span data-ttu-id="6067a-138">Пример 1: получение списка приложений</span><span class="sxs-lookup"><span data-stu-id="6067a-138">Example 1: Get the list of applications</span></span>

#### <a name="request"></a><span data-ttu-id="6067a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6067a-139">Request</span></span>

<span data-ttu-id="6067a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6067a-140">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6067a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="6067a-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications
```
# <a name="c"></a>[<span data-ttu-id="6067a-142">C#</span><span class="sxs-lookup"><span data-stu-id="6067a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6067a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6067a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6067a-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6067a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6067a-145">Java</span><span class="sxs-lookup"><span data-stu-id="6067a-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6067a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="6067a-146">Response</span></span>

<span data-ttu-id="6067a-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6067a-147">Here is an example of the response.</span></span>

> <span data-ttu-id="6067a-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6067a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications",
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

### <a name="example-2-get-only-a-count-of-applications"></a><span data-ttu-id="6067a-150">Пример 2: получение только количества приложений</span><span class="sxs-lookup"><span data-stu-id="6067a-150">Example 2: Get only a count of applications</span></span>

#### <a name="request"></a><span data-ttu-id="6067a-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="6067a-151">Request</span></span>

<span data-ttu-id="6067a-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6067a-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6067a-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="6067a-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="6067a-154">C#</span><span class="sxs-lookup"><span data-stu-id="6067a-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6067a-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6067a-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6067a-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6067a-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6067a-157">Java</span><span class="sxs-lookup"><span data-stu-id="6067a-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6067a-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="6067a-158">Response</span></span>

<span data-ttu-id="6067a-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6067a-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-filter-and-top-to-get-one-application-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="6067a-160">Пример 3: использование параметров $filter и $top для получения одного приложения с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="6067a-160">Example 3: Use $filter and $top to get one application with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6067a-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="6067a-161">Request</span></span>

<span data-ttu-id="6067a-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6067a-162">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6067a-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="6067a-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="6067a-164">C#</span><span class="sxs-lookup"><span data-stu-id="6067a-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6067a-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6067a-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6067a-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6067a-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6067a-167">Java</span><span class="sxs-lookup"><span data-stu-id="6067a-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6067a-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="6067a-168">Response</span></span>

<span data-ttu-id="6067a-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6067a-169">The following is an example of the response.</span></span>

><span data-ttu-id="6067a-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6067a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#applications",
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

### <a name="example-4-use-search-to-get-applications-with-display-names-that-contain-the-letters-web-including-a-count-of-returned-objects"></a><span data-ttu-id="6067a-172">Пример 4: использование параметра $search для получения приложений с отображаемыми именами, содержащими буквы "Web", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="6067a-172">Example 4: Use $search to get applications with display names that contain the letters 'Web' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6067a-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="6067a-173">Request</span></span>

<span data-ttu-id="6067a-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6067a-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6067a-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="6067a-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_web_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications?$search="displayName:Web"&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="6067a-176">C#</span><span class="sxs-lookup"><span data-stu-id="6067a-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-web-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6067a-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6067a-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-web-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6067a-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6067a-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-web-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6067a-179">Java</span><span class="sxs-lookup"><span data-stu-id="6067a-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-web-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6067a-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="6067a-180">Response</span></span>

<span data-ttu-id="6067a-181">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6067a-181">The following is an example of the response.</span></span>

><span data-ttu-id="6067a-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6067a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#applications",
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
