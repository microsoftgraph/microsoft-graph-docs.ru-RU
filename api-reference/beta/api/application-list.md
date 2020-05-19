---
title: Список приложений
description: Получение списка приложений в организации.
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1483e745f5db70c08e4b919363a09fb91c1f360b
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289322"
---
# <a name="list-applications"></a><span data-ttu-id="0a156-103">Список приложений</span><span class="sxs-lookup"><span data-stu-id="0a156-103">List applications</span></span>

<span data-ttu-id="0a156-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a156-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a156-105">Получение списка [приложений](../resources/application.md) в организации.</span><span class="sxs-lookup"><span data-stu-id="0a156-105">Get the list of [applications](../resources/application.md) in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a156-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a156-106">Permissions</span></span>

<span data-ttu-id="0a156-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a156-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a156-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a156-109">Permission type</span></span> | <span data-ttu-id="0a156-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a156-110">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="0a156-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a156-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0a156-112">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="0a156-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="0a156-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a156-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a156-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a156-114">Not supported.</span></span> |
| <span data-ttu-id="0a156-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a156-115">Application</span></span> | <span data-ttu-id="0a156-116">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="0a156-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a156-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a156-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0a156-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0a156-118">Optional query parameters</span></span>

<span data-ttu-id="0a156-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, включая `$search` , `$count` и `$filter` .</span><span class="sxs-lookup"><span data-stu-id="0a156-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="0a156-120">Можно использовать `$search` свойство **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="0a156-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="0a156-121">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="0a156-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="0a156-122">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="0a156-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a156-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a156-123">Request headers</span></span>

| <span data-ttu-id="0a156-124">Имя</span><span class="sxs-lookup"><span data-stu-id="0a156-124">Name</span></span> | <span data-ttu-id="0a156-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0a156-125">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="0a156-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a156-126">Authorization</span></span>  | <span data-ttu-id="0a156-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a156-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0a156-129">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="0a156-129">ConsistencyLevel</span></span> | <span data-ttu-id="0a156-130">закончить.</span><span class="sxs-lookup"><span data-stu-id="0a156-130">eventual.</span></span> <span data-ttu-id="0a156-131">Этот заголовок и `$count` обязательные при использовании `$search` `$filter` с `$orderby` параметром Query.</span><span class="sxs-lookup"><span data-stu-id="0a156-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="0a156-132">Он использует индекс, который может быть не последним в актуальном изменении объекта.</span><span class="sxs-lookup"><span data-stu-id="0a156-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a156-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0a156-133">Request body</span></span>

<span data-ttu-id="0a156-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a156-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a156-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a156-135">Response</span></span>

<span data-ttu-id="0a156-136">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0a156-136">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0a156-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="0a156-137">Examples</span></span>

### <a name="example-1-get-the-list-of-applications"></a><span data-ttu-id="0a156-138">Пример 1: получение списка приложений</span><span class="sxs-lookup"><span data-stu-id="0a156-138">Example 1: Get the list of applications</span></span>

#### <a name="request"></a><span data-ttu-id="0a156-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a156-139">Request</span></span>

<span data-ttu-id="0a156-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a156-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0a156-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a156-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications
```
# <a name="c"></a>[<span data-ttu-id="0a156-142">C#</span><span class="sxs-lookup"><span data-stu-id="0a156-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a156-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a156-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a156-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a156-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="0a156-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a156-145">Response</span></span>

<span data-ttu-id="0a156-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0a156-146">Here is an example of the response.</span></span>
> <span data-ttu-id="0a156-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a156-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-applications"></a><span data-ttu-id="0a156-149">Пример 2: получение только количества приложений</span><span class="sxs-lookup"><span data-stu-id="0a156-149">Example 2: Get only a count of applications</span></span>

#### <a name="request"></a><span data-ttu-id="0a156-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a156-150">Request</span></span>

<span data-ttu-id="0a156-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a156-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0a156-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a156-152">Response</span></span>

<span data-ttu-id="0a156-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0a156-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="0a156-154">893</span><span class="sxs-lookup"><span data-stu-id="0a156-154">893</span></span>


### <a name="example-3-use-filter-and-top-to-get-one-application-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="0a156-155">Пример 3: используйте $filter и $top, чтобы получить одно приложение с отображаемым именем, начинающимся с "a", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="0a156-155">Example 3: Use $filter and $top to get one application with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0a156-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a156-156">Request</span></span>

<span data-ttu-id="0a156-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a156-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0a156-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a156-158">Response</span></span>

<span data-ttu-id="0a156-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0a156-159">The following is an example of the response.</span></span>
><span data-ttu-id="0a156-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a156-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-search-to-get-applications-with-display-names-that-contain-the-letters-web-including-a-count-of-returned-objects"></a><span data-ttu-id="0a156-162">Пример 4: использование $search для получения приложений с отображаемыми именами, содержащими "Web", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="0a156-162">Example 4: Use $search to get applications with display names that contain the letters 'Web' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0a156-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a156-163">Request</span></span>

<span data-ttu-id="0a156-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a156-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_web_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications?$search="displayName:Web"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0a156-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a156-165">Response</span></span>

<span data-ttu-id="0a156-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0a156-166">The following is an example of the response.</span></span>
><span data-ttu-id="0a156-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a156-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
