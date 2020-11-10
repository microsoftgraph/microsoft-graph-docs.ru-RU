---
title: Список приложений
description: Получение списка приложений в организации.
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7e8ccbf07bbc52e11b0aa98deb494e9469596666
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962086"
---
# <a name="list-applications"></a><span data-ttu-id="6cde2-103">Список приложений</span><span class="sxs-lookup"><span data-stu-id="6cde2-103">List applications</span></span>

<span data-ttu-id="6cde2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cde2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cde2-105">Получение списка [приложений](../resources/application.md) в организации.</span><span class="sxs-lookup"><span data-stu-id="6cde2-105">Get the list of [applications](../resources/application.md) in this organization.</span></span>

> [!NOTE]
> <span data-ttu-id="6cde2-106">При вызове этого API с использованием маркеров, выпущенных для личной учетной записи Майкрософт, возвращаются приложения, принадлежащие личной учетной записи Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="6cde2-106">When calling this API using tokens issued for a personal Microsoft account, it will return the apps owned by the personal Microsoft account.</span></span> <span data-ttu-id="6cde2-107">Для личных учетных записей Майкрософт не существует понятия организаций.</span><span class="sxs-lookup"><span data-stu-id="6cde2-107">The notion of organizations doesn't exist for personal Microsoft accounts.</span></span> <span data-ttu-id="6cde2-108">Чтобы составить список приложений, принадлежащих определенным личным учетным записям Майкрософт, для этого API помимо Application.Read.All или Application.ReadWrite.All требуется разрешение User.Read.</span><span class="sxs-lookup"><span data-stu-id="6cde2-108">In order to list applications owned by specific personal Microsoft accounts, this API requires User.Read permission in addition to Application.Read.All or Application.ReadWrite.All.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="6cde2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6cde2-109">Permissions</span></span>

<span data-ttu-id="6cde2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cde2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6cde2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cde2-112">Permission type</span></span> | <span data-ttu-id="6cde2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cde2-113">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="6cde2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cde2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6cde2-115">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6cde2-115">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="6cde2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cde2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cde2-117">Application.Read.All и User.Read, Application.ReadWrite.All и User.Read</span><span class="sxs-lookup"><span data-stu-id="6cde2-117">Application.Read.All and User.Read, Application.ReadWrite.All and User.Read</span></span>  |
| <span data-ttu-id="6cde2-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="6cde2-118">Application</span></span> | <span data-ttu-id="6cde2-119">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cde2-119">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cde2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cde2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6cde2-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6cde2-121">Optional query parameters</span></span>

<span data-ttu-id="6cde2-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="6cde2-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="6cde2-123">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="6cde2-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="6cde2-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="6cde2-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="6cde2-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="6cde2-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cde2-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6cde2-126">Request headers</span></span>

| <span data-ttu-id="6cde2-127">Имя</span><span class="sxs-lookup"><span data-stu-id="6cde2-127">Name</span></span> | <span data-ttu-id="6cde2-128">Описание</span><span class="sxs-lookup"><span data-stu-id="6cde2-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="6cde2-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6cde2-129">Authorization</span></span>  | <span data-ttu-id="6cde2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6cde2-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6cde2-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="6cde2-132">ConsistencyLevel</span></span> | <span data-ttu-id="6cde2-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="6cde2-133">eventual.</span></span> <span data-ttu-id="6cde2-134">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="6cde2-134">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="6cde2-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="6cde2-135">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6cde2-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6cde2-136">Request body</span></span>

<span data-ttu-id="6cde2-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6cde2-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cde2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cde2-138">Response</span></span>

<span data-ttu-id="6cde2-139">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6cde2-139">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6cde2-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="6cde2-140">Examples</span></span>

### <a name="example-1-get-the-list-of-applications"></a><span data-ttu-id="6cde2-141">Пример 1: получение списка приложений</span><span class="sxs-lookup"><span data-stu-id="6cde2-141">Example 1: Get the list of applications</span></span>

#### <a name="request"></a><span data-ttu-id="6cde2-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cde2-142">Request</span></span>

<span data-ttu-id="6cde2-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cde2-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6cde2-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cde2-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications
```
# <a name="c"></a>[<span data-ttu-id="6cde2-145">C#</span><span class="sxs-lookup"><span data-stu-id="6cde2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6cde2-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cde2-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cde2-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cde2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6cde2-148">Java</span><span class="sxs-lookup"><span data-stu-id="6cde2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6cde2-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cde2-149">Response</span></span>

<span data-ttu-id="6cde2-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6cde2-150">Here is an example of the response.</span></span>
> <span data-ttu-id="6cde2-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6cde2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-applications"></a><span data-ttu-id="6cde2-153">Пример 2: получение только количества приложений</span><span class="sxs-lookup"><span data-stu-id="6cde2-153">Example 2: Get only a count of applications</span></span>

#### <a name="request"></a><span data-ttu-id="6cde2-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cde2-154">Request</span></span>

<span data-ttu-id="6cde2-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cde2-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6cde2-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cde2-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="6cde2-157">C#</span><span class="sxs-lookup"><span data-stu-id="6cde2-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6cde2-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cde2-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cde2-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cde2-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6cde2-160">Java</span><span class="sxs-lookup"><span data-stu-id="6cde2-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6cde2-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cde2-161">Response</span></span>

<span data-ttu-id="6cde2-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6cde2-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="6cde2-163">893</span><span class="sxs-lookup"><span data-stu-id="6cde2-163">893</span></span>


### <a name="example-3-use-filter-and-top-to-get-one-application-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="6cde2-164">Пример 3: использование параметров $filter и $top для получения одного приложения с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="6cde2-164">Example 3: Use $filter and $top to get one application with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6cde2-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cde2-165">Request</span></span>

<span data-ttu-id="6cde2-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cde2-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6cde2-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cde2-167">Response</span></span>

<span data-ttu-id="6cde2-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6cde2-168">The following is an example of the response.</span></span>
><span data-ttu-id="6cde2-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6cde2-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-search-to-get-applications-with-display-names-that-contain-the-letters-web-including-a-count-of-returned-objects"></a><span data-ttu-id="6cde2-171">Пример 4: использование параметра $search для получения приложений с отображаемыми именами, содержащими буквы "Web", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="6cde2-171">Example 4: Use $search to get applications with display names that contain the letters 'Web' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6cde2-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cde2-172">Request</span></span>

<span data-ttu-id="6cde2-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cde2-173">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6cde2-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cde2-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_web_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications?$search="displayName:Web"&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="6cde2-175">C#</span><span class="sxs-lookup"><span data-stu-id="6cde2-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-web-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6cde2-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cde2-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-web-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cde2-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cde2-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-web-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6cde2-178">Java</span><span class="sxs-lookup"><span data-stu-id="6cde2-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-web-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6cde2-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cde2-179">Response</span></span>

<span data-ttu-id="6cde2-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6cde2-180">The following is an example of the response.</span></span>
><span data-ttu-id="6cde2-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6cde2-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


