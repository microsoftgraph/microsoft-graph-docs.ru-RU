---
title: 'servicePrincipal: delta'
description: Получать только что созданные, обновленные или удаленные основные службы, не выполняя полное чтение всей коллекции ресурсов. См. подробные сведения об использовании запроса delta.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 316ad5f18336cd269bcab8bbd773c9957654b240
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133338"
---
# <a name="serviceprincipal-delta"></a><span data-ttu-id="4fc2e-104">servicePrincipal: delta</span><span class="sxs-lookup"><span data-stu-id="4fc2e-104">servicePrincipal: delta</span></span>

<span data-ttu-id="4fc2e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fc2e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fc2e-106">Получать только что созданные, обновленные или удаленные основные службы, не выполняя полное чтение всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-106">Get newly created, updated, or deleted service principals without having to perform a full read of the entire resource collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fc2e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4fc2e-107">Permissions</span></span>

<span data-ttu-id="4fc2e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fc2e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4fc2e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fc2e-110">Permission type</span></span>      | <span data-ttu-id="4fc2e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fc2e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4fc2e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fc2e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4fc2e-113">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4fc2e-113">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4fc2e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fc2e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fc2e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-115">Not supported.</span></span>    |
|<span data-ttu-id="4fc2e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fc2e-116">Application</span></span> | <span data-ttu-id="4fc2e-117">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fc2e-117">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fc2e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fc2e-118">HTTP request</span></span>

<span data-ttu-id="4fc2e-119">Чтобы начать отслеживание изменений, необходимо внести запрос, включив функцию delta для ресурса servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-119">To begin tracking changes, you make a request including the delta function on the servicePrincipal resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

### <a name="query-parameters"></a><span data-ttu-id="4fc2e-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="4fc2e-120">Query parameters</span></span>

<span data-ttu-id="4fc2e-121">Отслеживание изменений вызывает один или несколько вызовов **функции delta.**</span><span class="sxs-lookup"><span data-stu-id="4fc2e-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="4fc2e-122">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="4fc2e-123">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="4fc2e-124">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="4fc2e-125">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="4fc2e-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="4fc2e-126">Query parameter</span></span>      | <span data-ttu-id="4fc2e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4fc2e-127">Type</span></span>   |<span data-ttu-id="4fc2e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4fc2e-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4fc2e-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="4fc2e-129">$deltatoken</span></span> | <span data-ttu-id="4fc2e-130">string</span><span class="sxs-lookup"><span data-stu-id="4fc2e-130">string</span></span> | <span data-ttu-id="4fc2e-131">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адресе предыдущего вызова функции delta для той же коллекции ресурсов, что указывает на завершение этого круга `deltaLink` отслеживания  изменений.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="4fc2e-132">Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="4fc2e-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="4fc2e-133">$skiptoken</span></span> | <span data-ttu-id="4fc2e-134">string</span><span class="sxs-lookup"><span data-stu-id="4fc2e-134">string</span></span> | <span data-ttu-id="4fc2e-135">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адресе предыдущего вызова функции delta, указывающий на то, что в той же коллекции ресурсов отслеживаются `nextLink` дополнительные  изменения.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="4fc2e-136">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4fc2e-136">Optional query parameters</span></span>

<span data-ttu-id="4fc2e-137">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-137">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="4fc2e-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="4fc2e-140">Имеется ограниченная поддержка параметра `$filter`:</span><span class="sxs-lookup"><span data-stu-id="4fc2e-140">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="4fc2e-141">Единственное поддерживаемые выражения для отслеживания изменений для `$filter` определенных ресурсов по их ид:  `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="4fc2e-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="4fc2e-142">Допустимые числа ид ограничены максимальной длиной URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-142">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="4fc2e-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4fc2e-143">Request headers</span></span>
| <span data-ttu-id="4fc2e-144">Имя</span><span class="sxs-lookup"><span data-stu-id="4fc2e-144">Name</span></span>       | <span data-ttu-id="4fc2e-145">Описание</span><span class="sxs-lookup"><span data-stu-id="4fc2e-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4fc2e-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fc2e-146">Authorization</span></span>  | <span data-ttu-id="4fc2e-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="4fc2e-147">Bearer &lt;token&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fc2e-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4fc2e-148">Request body</span></span>
<span data-ttu-id="4fc2e-149">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-149">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="4fc2e-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fc2e-150">Response</span></span>

<span data-ttu-id="4fc2e-151">В случае успеха этот метод возвращает код отклика и объект `200 OK` [коллекции servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-151">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) collection object in the response body.</span></span> <span data-ttu-id="4fc2e-152">Ответ также включает URL-адрес nextLink или URL-адрес deltaLink.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-152">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="4fc2e-153">Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-153">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="4fc2e-154">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-154">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="4fc2e-155">Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-155">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="4fc2e-156">Сохраните и используйте `deltaLink` URL-адрес, чтобы узнать об изменениях ресурса в будущем.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-156">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="4fc2e-157">См. следующее:</span><span class="sxs-lookup"><span data-stu-id="4fc2e-157">See:</span></span></br>
- <span data-ttu-id="4fc2e-158">[Дополнительные сведения](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="4fc2e-158">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="4fc2e-159">[Примеры запросов](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="4fc2e-159">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

## <a name="example"></a><span data-ttu-id="4fc2e-160">Пример</span><span class="sxs-lookup"><span data-stu-id="4fc2e-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="4fc2e-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fc2e-161">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4fc2e-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="4fc2e-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/delta
```
# <a name="c"></a>[<span data-ttu-id="4fc2e-163">C#</span><span class="sxs-lookup"><span data-stu-id="4fc2e-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4fc2e-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4fc2e-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4fc2e-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4fc2e-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4fc2e-166">Java</span><span class="sxs-lookup"><span data-stu-id="4fc2e-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4fc2e-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fc2e-167">Response</span></span>
><span data-ttu-id="4fc2e-168">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-168">Note: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4fc2e-169">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4fc2e-169">All the properties will be returned from an actual call.</span></span>
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



