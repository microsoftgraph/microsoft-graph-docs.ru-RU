---
title: 'servicePrincipal: delta'
description: Создайте заново созданные, обновленные или удаленные принципы службы, не выполняя полное чтение всей коллекции ресурсов. Подробные сведения см. в материале Использование запроса Delta.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: a878e82a591f287712231c68022874b5967cbd1b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051944"
---
# <a name="serviceprincipal-delta"></a><span data-ttu-id="66766-104">servicePrincipal: delta</span><span class="sxs-lookup"><span data-stu-id="66766-104">servicePrincipal: delta</span></span>

<span data-ttu-id="66766-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66766-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66766-106">Создайте заново созданные, обновленные или удаленные принципы службы, не выполняя полное чтение всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="66766-106">Get newly created, updated, or deleted service principals without having to perform a full read of the entire resource collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="66766-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66766-107">Permissions</span></span>

<span data-ttu-id="66766-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66766-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="66766-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66766-110">Permission type</span></span>      | <span data-ttu-id="66766-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66766-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66766-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66766-112">Delegated (work or school account)</span></span> | <span data-ttu-id="66766-113">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="66766-113">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="66766-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66766-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66766-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66766-115">Not supported.</span></span>    |
|<span data-ttu-id="66766-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66766-116">Application</span></span> | <span data-ttu-id="66766-117">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66766-117">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66766-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66766-118">HTTP request</span></span>

<span data-ttu-id="66766-119">Чтобы начать отслеживание изменений, необходимо сделать запрос, включив функцию delta на ресурсе servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="66766-119">To begin tracking changes, you make a request including the delta function on the servicePrincipal resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

### <a name="query-parameters"></a><span data-ttu-id="66766-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="66766-120">Query parameters</span></span>

<span data-ttu-id="66766-121">Отслеживание изменений вызывает один или несколько вызовов функции **дельты.**</span><span class="sxs-lookup"><span data-stu-id="66766-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="66766-122">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="66766-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="66766-123">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="66766-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="66766-124">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="66766-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="66766-125">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="66766-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="66766-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="66766-126">Query parameter</span></span>      | <span data-ttu-id="66766-127">Тип</span><span class="sxs-lookup"><span data-stu-id="66766-127">Type</span></span>   |<span data-ttu-id="66766-128">Описание</span><span class="sxs-lookup"><span data-stu-id="66766-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="66766-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="66766-129">$deltatoken</span></span> | <span data-ttu-id="66766-130">string</span><span class="sxs-lookup"><span data-stu-id="66766-130">string</span></span> | <span data-ttu-id="66766-131">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущей функции дельты, вызываем для того же собрания ресурсов, что указывает на завершение этого раунда отслеживания `deltaLink` изменений. </span><span class="sxs-lookup"><span data-stu-id="66766-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="66766-132">Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="66766-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="66766-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="66766-133">$skiptoken</span></span> | <span data-ttu-id="66766-134">string</span><span class="sxs-lookup"><span data-stu-id="66766-134">string</span></span> | <span data-ttu-id="66766-135">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущего вызова функции дельты, указывает на то, что в том же собрании ресурсов необходимо отслеживать дальнейшие `nextLink` изменения. </span><span class="sxs-lookup"><span data-stu-id="66766-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="66766-136">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="66766-136">Optional query parameters</span></span>

<span data-ttu-id="66766-137">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="66766-137">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="66766-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="66766-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="66766-140">Имеется ограниченная поддержка параметра `$filter`:</span><span class="sxs-lookup"><span data-stu-id="66766-140">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="66766-141">Единственным `$filter` поддерживаемым выражением является отслеживание изменений для определенных ресурсов по их id:  `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="66766-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="66766-142">Количество ids, которые можно указать, ограничено максимальной длиной URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="66766-142">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="66766-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66766-143">Request headers</span></span>
| <span data-ttu-id="66766-144">Имя</span><span class="sxs-lookup"><span data-stu-id="66766-144">Name</span></span>       | <span data-ttu-id="66766-145">Описание</span><span class="sxs-lookup"><span data-stu-id="66766-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="66766-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="66766-146">Authorization</span></span>  | <span data-ttu-id="66766-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="66766-147">Bearer &lt;token&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="66766-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66766-148">Request body</span></span>
<span data-ttu-id="66766-149">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="66766-149">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="66766-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="66766-150">Response</span></span>

<span data-ttu-id="66766-151">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект коллекции servicePrincipal](../resources/serviceprincipal.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="66766-151">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) collection object in the response body.</span></span> <span data-ttu-id="66766-152">Ответ также включает URL-адрес nextLink или URL-адрес deltaLink.</span><span class="sxs-lookup"><span data-stu-id="66766-152">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="66766-153">Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="66766-153">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="66766-154">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="66766-154">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="66766-155">Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="66766-155">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="66766-156">Сохраните и используйте `deltaLink` URL-адрес, чтобы узнать об изменениях в ресурсе в будущем.</span><span class="sxs-lookup"><span data-stu-id="66766-156">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="66766-157">См. следующее:</span><span class="sxs-lookup"><span data-stu-id="66766-157">See:</span></span></br>
- <span data-ttu-id="66766-158">[Дополнительные сведения](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="66766-158">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="66766-159">[Примеры запросов](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="66766-159">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

## <a name="example"></a><span data-ttu-id="66766-160">Пример</span><span class="sxs-lookup"><span data-stu-id="66766-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="66766-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="66766-161">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="66766-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="66766-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/delta
```
# <a name="c"></a>[<span data-ttu-id="66766-163">C#</span><span class="sxs-lookup"><span data-stu-id="66766-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66766-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66766-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66766-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66766-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66766-166">Java</span><span class="sxs-lookup"><span data-stu-id="66766-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="66766-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="66766-167">Response</span></span>
><span data-ttu-id="66766-168">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="66766-168">Note: The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrincipals",
  "@odata.nextLink":"https://graph.microsoft.com/beta/servicePrincipals/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
     {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



