---
title: 'servicePrincipal: delta'
description: Создайте заново созданные, обновленные или удаленные принципы службы, не выполняя полное чтение всей коллекции ресурсов. Подробные сведения см. в материале Использование запроса Delta.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: dcbc05093737862c025b337d102696da718ccf99
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054464"
---
# <a name="serviceprincipal-delta"></a><span data-ttu-id="c80f0-104">servicePrincipal: delta</span><span class="sxs-lookup"><span data-stu-id="c80f0-104">servicePrincipal: delta</span></span>

<span data-ttu-id="c80f0-105">Создайте заново созданные, обновленные или удаленные принципы службы, не выполняя полное чтение всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c80f0-105">Get newly created, updated, or deleted service principals without having to perform a full read of the entire resource collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="c80f0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c80f0-106">Permissions</span></span>

<span data-ttu-id="c80f0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c80f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c80f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c80f0-109">Permission type</span></span>      | <span data-ttu-id="c80f0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c80f0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c80f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c80f0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c80f0-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c80f0-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c80f0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c80f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c80f0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c80f0-114">Not supported.</span></span>    |
|<span data-ttu-id="c80f0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c80f0-115">Application</span></span> | <span data-ttu-id="c80f0-116">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c80f0-116">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c80f0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c80f0-117">HTTP request</span></span>

<span data-ttu-id="c80f0-118">Чтобы начать отслеживание изменений, необходимо сделать запрос, включив функцию delta на ресурсе servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="c80f0-118">To begin tracking changes, you make a request including the delta function on the servicePrincipal resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

## <a name="query-parameters"></a><span data-ttu-id="c80f0-119">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="c80f0-119">Query parameters</span></span>

<span data-ttu-id="c80f0-120">Отслеживание изменений вызывает один или несколько вызовов функции **дельты.**</span><span class="sxs-lookup"><span data-stu-id="c80f0-120">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="c80f0-121">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="c80f0-121">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="c80f0-122">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="c80f0-122">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="c80f0-123">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="c80f0-123">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="c80f0-124">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="c80f0-124">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="c80f0-125">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="c80f0-125">Query parameter</span></span>      | <span data-ttu-id="c80f0-126">Тип</span><span class="sxs-lookup"><span data-stu-id="c80f0-126">Type</span></span>   |<span data-ttu-id="c80f0-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c80f0-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c80f0-128">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="c80f0-128">$deltatoken</span></span> | <span data-ttu-id="c80f0-129">string</span><span class="sxs-lookup"><span data-stu-id="c80f0-129">string</span></span> | <span data-ttu-id="c80f0-130">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущей функции дельты, вызываем для того же собрания ресурсов, что указывает на завершение этого раунда отслеживания `deltaLink` изменений. </span><span class="sxs-lookup"><span data-stu-id="c80f0-130">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="c80f0-131">Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="c80f0-131">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="c80f0-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="c80f0-132">$skiptoken</span></span> | <span data-ttu-id="c80f0-133">string</span><span class="sxs-lookup"><span data-stu-id="c80f0-133">string</span></span> | <span data-ttu-id="c80f0-134">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущего вызова функции дельты, указывает на то, что в том же собрании ресурсов необходимо отслеживать дальнейшие `nextLink` изменения. </span><span class="sxs-lookup"><span data-stu-id="c80f0-134">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="optional-query-parameters"></a><span data-ttu-id="c80f0-135">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c80f0-135">Optional query parameters</span></span>

<span data-ttu-id="c80f0-136">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c80f0-136">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="c80f0-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="c80f0-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="c80f0-139">Имеется ограниченная поддержка параметра `$filter`:</span><span class="sxs-lookup"><span data-stu-id="c80f0-139">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="c80f0-140">Единственным `$filter` поддерживаемым выражением является отслеживание изменений для определенных ресурсов по их id:  `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="c80f0-140">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="c80f0-141">Количество ids, которые можно указать, ограничено максимальной длиной URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="c80f0-141">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="c80f0-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c80f0-142">Request headers</span></span>
| <span data-ttu-id="c80f0-143">Имя</span><span class="sxs-lookup"><span data-stu-id="c80f0-143">Name</span></span>       | <span data-ttu-id="c80f0-144">Описание</span><span class="sxs-lookup"><span data-stu-id="c80f0-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c80f0-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="c80f0-145">Authorization</span></span>  | <span data-ttu-id="c80f0-146">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="c80f0-146">Bearer &lt;token&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="c80f0-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c80f0-147">Request body</span></span>
<span data-ttu-id="c80f0-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c80f0-148">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="c80f0-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c80f0-149">Response</span></span>

<span data-ttu-id="c80f0-150">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект коллекции servicePrincipal](../resources/serviceprincipal.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c80f0-150">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) collection object in the response body.</span></span> <span data-ttu-id="c80f0-151">Ответ также включает URL-адрес nextLink или URL-адрес deltaLink.</span><span class="sxs-lookup"><span data-stu-id="c80f0-151">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="c80f0-152">Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="c80f0-152">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="c80f0-153">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="c80f0-153">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="c80f0-154">Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="c80f0-154">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="c80f0-155">Сохраните и используйте `deltaLink` URL-адрес, чтобы узнать об изменениях в ресурсе в будущем.</span><span class="sxs-lookup"><span data-stu-id="c80f0-155">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="c80f0-156">См. следующее:</span><span class="sxs-lookup"><span data-stu-id="c80f0-156">See:</span></span></br>
- <span data-ttu-id="c80f0-157">[Дополнительные сведения](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="c80f0-157">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="c80f0-158">[Примеры запросов](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="c80f0-158">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

## <a name="example"></a><span data-ttu-id="c80f0-159">Пример</span><span class="sxs-lookup"><span data-stu-id="c80f0-159">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c80f0-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="c80f0-160">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c80f0-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="c80f0-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/delta
```
# <a name="c"></a>[<span data-ttu-id="c80f0-162">C#</span><span class="sxs-lookup"><span data-stu-id="c80f0-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c80f0-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c80f0-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c80f0-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c80f0-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c80f0-165">Java</span><span class="sxs-lookup"><span data-stu-id="c80f0-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c80f0-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="c80f0-166">Response</span></span>
><span data-ttu-id="c80f0-167">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c80f0-167">Note: The response object shown here might be shortened for readability.</span></span>
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
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/servicePrincipals/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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

