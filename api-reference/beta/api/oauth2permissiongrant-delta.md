---
title: 'oauth2permissiongrant: дельта'
description: Получить заново созданные, обновленные или удаленные oauth2permissiongrants без выполнения полного чтения всей коллекции ресурсов.
localization_priority: Normal
author: psignoret
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e4a4568dc143148597729e5b0981bda606649e27
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442392"
---
# <a name="oauth2permissiongrant-delta"></a><span data-ttu-id="2bde6-103">oauth2permissiongrant: дельта</span><span class="sxs-lookup"><span data-stu-id="2bde6-103">oauth2permissiongrant: delta</span></span>

<span data-ttu-id="2bde6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bde6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bde6-105">Получить вновь созданные, обновленные или удаленные **объекты oauth2permissiongrant** без полного чтения всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2bde6-105">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span> <span data-ttu-id="2bde6-106">Подробные сведения см. в [материале Использование запроса delta.](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="2bde6-106">For details, see [Using delta query](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="2bde6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2bde6-107">Permissions</span></span>

<span data-ttu-id="2bde6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bde6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2bde6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2bde6-110">Permission type</span></span>      | <span data-ttu-id="2bde6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2bde6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bde6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2bde6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2bde6-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2bde6-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2bde6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2bde6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bde6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bde6-115">Not supported.</span></span>    |
|<span data-ttu-id="2bde6-116">oauth2permissiongrant</span><span class="sxs-lookup"><span data-stu-id="2bde6-116">oauth2permissiongrant</span></span> | <span data-ttu-id="2bde6-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bde6-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2bde6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2bde6-118">HTTP request</span></span>

<span data-ttu-id="2bde6-119">Чтобы начать отслеживать изменения, необходимо сделать запрос, включив функцию дельты на **ресурсе oauth2permissiongrant.**</span><span class="sxs-lookup"><span data-stu-id="2bde6-119">To begin tracking changes, you make a request including the delta function on the **oauth2permissiongrant** resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants/delta
```

## <a name="query-parameters"></a><span data-ttu-id="2bde6-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="2bde6-120">Query parameters</span></span>

<span data-ttu-id="2bde6-121">Отслеживание изменений вызывает один или несколько вызовов функции **дельты.**</span><span class="sxs-lookup"><span data-stu-id="2bde6-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="2bde6-122">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="2bde6-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="2bde6-123">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="2bde6-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="2bde6-124">Необходимо указать параметры запроса только один раз.</span><span class="sxs-lookup"><span data-stu-id="2bde6-124">You only need to specify any query parameters once up front.</span></span> <span data-ttu-id="2bde6-125">В последующих запросах скопируйте и примените `nextLink` `deltaLink` URL-адрес из предыдущего ответа.</span><span class="sxs-lookup"><span data-stu-id="2bde6-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="2bde6-126">Этот URL-адрес уже содержит закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="2bde6-126">That URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="2bde6-127">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="2bde6-127">Query parameter</span></span>      | <span data-ttu-id="2bde6-128">Тип</span><span class="sxs-lookup"><span data-stu-id="2bde6-128">Type</span></span>   |<span data-ttu-id="2bde6-129">Описание</span><span class="sxs-lookup"><span data-stu-id="2bde6-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2bde6-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="2bde6-130">$deltatoken</span></span> | <span data-ttu-id="2bde6-131">string</span><span class="sxs-lookup"><span data-stu-id="2bde6-131">string</span></span> | <span data-ttu-id="2bde6-132">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущей функции дельты, вызываем для того же собрания ресурсов, что указывает на завершение этого раунда отслеживания `deltaLink` изменений. </span><span class="sxs-lookup"><span data-stu-id="2bde6-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="2bde6-133">Сохраните и примените весь URL-адрес, включая этот маркер, в первом запросе следующего раунда отслеживания `deltaLink` изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="2bde6-133">Save and apply the entire `deltaLink` URL, including this token, in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="2bde6-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="2bde6-134">$skiptoken</span></span> | <span data-ttu-id="2bde6-135">string</span><span class="sxs-lookup"><span data-stu-id="2bde6-135">string</span></span> | <span data-ttu-id="2bde6-136">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущего вызова функции дельты, указывает на то, что в том же собрании ресурсов необходимо отслеживать дальнейшие `nextLink` изменения. </span><span class="sxs-lookup"><span data-stu-id="2bde6-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="optional-query-parameters"></a><span data-ttu-id="2bde6-137">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2bde6-137">Optional query parameters</span></span>

<span data-ttu-id="2bde6-138">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2bde6-138">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="2bde6-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство **id** возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="2bde6-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The **id** property is always returned.</span></span>
- <span data-ttu-id="2bde6-141">Имеется ограниченная поддержка параметра `$filter`:</span><span class="sxs-lookup"><span data-stu-id="2bde6-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="2bde6-142">Единственным `$filter` поддерживаемым выражением является отслеживание изменений для определенных ресурсов по их ID:  `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="2bde6-142">The only supported `$filter` expression is for tracking changes for specific resources, by their ID:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="2bde6-143">Количество url-адресов, которые можно указать, ограничено максимальной длиной URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="2bde6-143">The number of IDs you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="2bde6-144">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2bde6-144">Request headers</span></span>
| <span data-ttu-id="2bde6-145">Имя</span><span class="sxs-lookup"><span data-stu-id="2bde6-145">Name</span></span>       | <span data-ttu-id="2bde6-146">Описание</span><span class="sxs-lookup"><span data-stu-id="2bde6-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2bde6-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bde6-147">Authorization</span></span>  | <span data-ttu-id="2bde6-148">Носитель &lt;токен&gt;.</span><span class="sxs-lookup"><span data-stu-id="2bde6-148">Bearer &lt;token&gt;.</span></span> <span data-ttu-id="2bde6-149">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="2bde6-149">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bde6-150">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2bde6-150">Request body</span></span>
<span data-ttu-id="2bde6-151">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2bde6-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bde6-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bde6-152">Response</span></span>

<span data-ttu-id="2bde6-153">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект коллекции oauth2permissiongrant](../resources/oauth2permissiongrant.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2bde6-153">If successful, this method returns a `200 OK` response code and an [oauth2permissiongrant](../resources/oauth2permissiongrant.md) collection object in the response body.</span></span> <span data-ttu-id="2bde6-154">Отклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="2bde6-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="2bde6-155">Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="2bde6-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="2bde6-156">**Oauth2permissiongrant** продолжает делать запросы с помощью URL-адреса до тех пор, пока URL-адрес не будет включен `nextLink` `deltaLink` в ответ.</span><span class="sxs-lookup"><span data-stu-id="2bde6-156">The **oauth2permissiongrant** continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="2bde6-157">Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="2bde6-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="2bde6-158">Сохраните и используйте `deltaLink` URL-адрес, чтобы узнать об изменениях в ресурсе в будущем.</span><span class="sxs-lookup"><span data-stu-id="2bde6-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="2bde6-159">Подробные сведения см. в [материале Использование запроса delta.](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="2bde6-159">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="2bde6-160">Например, запросы см. [в рублях Получить дополнительные изменения для пользователей.](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="2bde6-160">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="example"></a><span data-ttu-id="2bde6-161">Пример</span><span class="sxs-lookup"><span data-stu-id="2bde6-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="2bde6-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bde6-162">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2bde6-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="2bde6-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "oauth2permissiongrant_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants/delta
```
# <a name="c"></a>[<span data-ttu-id="2bde6-164">C#</span><span class="sxs-lookup"><span data-stu-id="2bde6-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/oauth2permissiongrant-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2bde6-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2bde6-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/oauth2permissiongrant-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2bde6-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2bde6-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/oauth2permissiongrant-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2bde6-167">Java</span><span class="sxs-lookup"><span data-stu-id="2bde6-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/oauth2permissiongrant-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2bde6-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bde6-168">Response</span></span>
><span data-ttu-id="2bde6-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2bde6-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#oauth2permissiongrants",
  "@odata.nextLink":"https://graph.microsoft.com/beta/oauth2permissiongrants/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "clientId": "22a3c970-8ad4-4120-8127-300837f87f2c",
      "consentType": "Principal",
      "expiryTime": "2017-08-13T21:41:23.3929007Z",
      "principalId": "c2e8df37-c6a7-4d88-89b1-feb4f1fda7c5",
      "resourceId": "98dc9d95-49b6-405a-b3c0-834e969a708b",
      "scope": "User.Read Directory.AccessAsUser.All",
      "startTime": "0001-01-01T00:00:00Z",
      "id": "cMmjItSKIEGBJzAIN_h_LJWd3Ji2SVpAs8CDTpaacIs33-jCp8aITYmx_rTx_afF"
    }
  ]
}
```

<!-- uuid: ba679d55-d10e-4518-b733-6f3e9576afb1
2020-04-09 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oauth2permissiongrant: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


