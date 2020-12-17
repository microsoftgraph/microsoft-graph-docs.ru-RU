---
title: Перечисление servicePrincipals
description: Получение списка объектов servicePrincipal.
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ea7596d1c94c110916fbb6e9bd407397d6029203
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082234"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="82af5-103">Перечисление servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="82af5-103">List servicePrincipals</span></span>

<span data-ttu-id="82af5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82af5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="82af5-105">Получение списка объектов [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="82af5-105">Retrieve a list of [servicePrincipal](../resources/serviceprincipal.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="82af5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82af5-106">Permissions</span></span>

<span data-ttu-id="82af5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82af5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82af5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82af5-109">Permission type</span></span>      | <span data-ttu-id="82af5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82af5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82af5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82af5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="82af5-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="82af5-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="82af5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82af5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82af5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82af5-114">Not supported.</span></span>    |
|<span data-ttu-id="82af5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82af5-115">Application</span></span> | <span data-ttu-id="82af5-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="82af5-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82af5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82af5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="82af5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="82af5-118">Optional query parameters</span></span>

<span data-ttu-id="82af5-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="82af5-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="82af5-120">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="82af5-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="82af5-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="82af5-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="82af5-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="82af5-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82af5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82af5-123">Request headers</span></span>
| <span data-ttu-id="82af5-124">Имя</span><span class="sxs-lookup"><span data-stu-id="82af5-124">Name</span></span>           | <span data-ttu-id="82af5-125">Описание</span><span class="sxs-lookup"><span data-stu-id="82af5-125">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="82af5-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82af5-126">Authorization</span></span>  | <span data-ttu-id="82af5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82af5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="82af5-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="82af5-129">ConsistencyLevel</span></span> | <span data-ttu-id="82af5-130">необязательный.</span><span class="sxs-lookup"><span data-stu-id="82af5-130">eventual.</span></span> <span data-ttu-id="82af5-131">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="82af5-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="82af5-132">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="82af5-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82af5-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82af5-133">Request body</span></span>

<span data-ttu-id="82af5-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82af5-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82af5-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="82af5-135">Response</span></span>

<span data-ttu-id="82af5-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82af5-136">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="82af5-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="82af5-137">Examples</span></span>

### <a name="example-1-get-a-list-of-service-principals"></a><span data-ttu-id="82af5-138">Пример 1. Получение списка субъект-служб</span><span class="sxs-lookup"><span data-stu-id="82af5-138">Example 1: Get a list of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="82af5-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="82af5-139">Request</span></span>

<span data-ttu-id="82af5-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82af5-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="82af5-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="82af5-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals
```
# <a name="c"></a>[<span data-ttu-id="82af5-142">C#</span><span class="sxs-lookup"><span data-stu-id="82af5-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82af5-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82af5-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82af5-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82af5-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="82af5-145">Java</span><span class="sxs-lookup"><span data-stu-id="82af5-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="82af5-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="82af5-146">Response</span></span>

<span data-ttu-id="82af5-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="82af5-147">The following is an example of the response.</span></span>

><span data-ttu-id="82af5-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82af5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":true,
      "displayName":"amasf",
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-service-principals"></a><span data-ttu-id="82af5-150">Пример 2. Получение только количества субъект-служб</span><span class="sxs-lookup"><span data-stu-id="82af5-150">Example 2: Get only a count of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="82af5-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="82af5-151">Request</span></span>

<span data-ttu-id="82af5-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82af5-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="82af5-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="82af5-153">Response</span></span>

<span data-ttu-id="82af5-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="82af5-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-filter-and-top-to-get-one-service-principal-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="82af5-155">Пример 3. Использование параметров $filter и $top для получения субъект-службы с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="82af5-155">Example 3: Use $filter and $top to get one service principal with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="82af5-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="82af5-156">Request</span></span>

<span data-ttu-id="82af5-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82af5-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="82af5-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="82af5-158">Response</span></span>

<span data-ttu-id="82af5-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="82af5-159">The following is an example of the response.</span></span>

><span data-ttu-id="82af5-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82af5-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#servicePrinciples",
  "@odata.count":1,
  "value":[
    {
      "accountEnabled":true,
      "displayName":"a",
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-service-principals-with-display-names-that-contain-the-letters-team-including-a-count-of-returned-objects"></a><span data-ttu-id="82af5-162">Пример 4. Использование параметра $search для получения субъект-служб с отображаемыми именами, содержащими буквы "Team", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="82af5-162">Example 4: Use $search to get service principals with display names that contain the letters 'Team' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="82af5-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="82af5-163">Request</span></span>

<span data-ttu-id="82af5-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82af5-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals?$search="displayName:Team"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="82af5-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="82af5-165">Response</span></span>

<span data-ttu-id="82af5-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="82af5-166">The following is an example of the response.</span></span>

><span data-ttu-id="82af5-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82af5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#servicePrincipals",
  "@odata.count":1396,
  "value":[
    {
      "accountEnabled":true,
      "displayName":"myContosoTeam",
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
