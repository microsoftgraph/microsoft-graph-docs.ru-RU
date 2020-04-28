---
title: 'servicePrincipal: Delta'
description: Получите только что созданных, обновленных или удаленных субъектов-служб, не требуя полного считывания всей коллекции ресурсов. Сведения об использовании запроса изменений см.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 1489b31e6523c1bcd3b456aa3fef567ac2d3754c
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43216710"
---
# <a name="serviceprincipal-delta"></a><span data-ttu-id="7ae33-104">servicePrincipal: Delta</span><span class="sxs-lookup"><span data-stu-id="7ae33-104">servicePrincipal: delta</span></span>

<span data-ttu-id="7ae33-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ae33-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ae33-106">Получите только что созданных, обновленных или удаленных субъектов-служб, не требуя полного считывания всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="7ae33-106">Get newly created, updated, or deleted service principals without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="7ae33-107">Сведения об [использовании запроса изменений](/graph/delta-query-overview) см.</span><span class="sxs-lookup"><span data-stu-id="7ae33-107">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ae33-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ae33-108">Permissions</span></span>

<span data-ttu-id="7ae33-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ae33-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7ae33-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ae33-111">Permission type</span></span>      | <span data-ttu-id="7ae33-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ae33-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ae33-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ae33-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7ae33-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7ae33-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7ae33-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ae33-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ae33-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ae33-116">Not supported.</span></span>    |
|<span data-ttu-id="7ae33-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ae33-117">Application</span></span> | <span data-ttu-id="7ae33-118">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ae33-118">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ae33-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ae33-119">HTTP request</span></span>

<span data-ttu-id="7ae33-120">Чтобы начать отслеживание изменений, создайте запрос, включающий функцию Delta в ресурсе servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="7ae33-120">To begin tracking changes, you make a request including the delta function on the servicePrincipal resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

### <a name="query-parameters"></a><span data-ttu-id="7ae33-121">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="7ae33-121">Query parameters</span></span>

<span data-ttu-id="7ae33-122">Отслеживание изменений приводит к округлению одного или нескольких вызовов функции **Delta** .</span><span class="sxs-lookup"><span data-stu-id="7ae33-122">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="7ae33-123">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="7ae33-123">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="7ae33-124">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="7ae33-124">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="7ae33-125">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="7ae33-125">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="7ae33-126">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="7ae33-126">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="7ae33-127">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="7ae33-127">Query parameter</span></span>      | <span data-ttu-id="7ae33-128">Тип</span><span class="sxs-lookup"><span data-stu-id="7ae33-128">Type</span></span>   |<span data-ttu-id="7ae33-129">Описание</span><span class="sxs-lookup"><span data-stu-id="7ae33-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7ae33-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="7ae33-130">$deltatoken</span></span> | <span data-ttu-id="7ae33-131">string</span><span class="sxs-lookup"><span data-stu-id="7ae33-131">string</span></span> | <span data-ttu-id="7ae33-132">[Токен состояния](/graph/delta-query-overview) возвращается в `deltaLink` URL-адресе предыдущего вызова функции **Delta** для той же коллекции ресурсов, что указывает на завершение этого круга отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="7ae33-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="7ae33-133">Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="7ae33-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="7ae33-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="7ae33-134">$skiptoken</span></span> | <span data-ttu-id="7ae33-135">string</span><span class="sxs-lookup"><span data-stu-id="7ae33-135">string</span></span> | <span data-ttu-id="7ae33-136">[Токен состояния](/graph/delta-query-overview) возвращается в `nextLink` URL-адресе предыдущего вызова функции **Delta** , указывая, что в коллекции ресурсов отслеживаются другие изменения.</span><span class="sxs-lookup"><span data-stu-id="7ae33-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="7ae33-137">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7ae33-137">Optional query parameters</span></span>

<span data-ttu-id="7ae33-138">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7ae33-138">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="7ae33-p106">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="7ae33-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="7ae33-141">Имеется ограниченная поддержка параметра `$filter`:</span><span class="sxs-lookup"><span data-stu-id="7ae33-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="7ae33-142">Единственное поддерживаемое `$filter` выражение предназначено для отслеживания изменений для определенных ресурсов по их идентификаторам: `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="7ae33-142">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="7ae33-143">Количество идентификаторов, которые можно указать, ограничено максимальной длиной URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="7ae33-143">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="7ae33-144">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ae33-144">Request headers</span></span>
| <span data-ttu-id="7ae33-145">Имя</span><span class="sxs-lookup"><span data-stu-id="7ae33-145">Name</span></span>       | <span data-ttu-id="7ae33-146">Описание</span><span class="sxs-lookup"><span data-stu-id="7ae33-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7ae33-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ae33-147">Authorization</span></span>  | <span data-ttu-id="7ae33-148">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="7ae33-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="7ae33-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ae33-149">Content-Type</span></span>  | <span data-ttu-id="7ae33-150">application/json</span><span class="sxs-lookup"><span data-stu-id="7ae33-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ae33-151">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ae33-151">Request body</span></span>
<span data-ttu-id="7ae33-152">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ae33-152">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="7ae33-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ae33-153">Response</span></span>

<span data-ttu-id="7ae33-154">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект коллекции [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7ae33-154">If successful, this method returns `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) collection object in the response body.</span></span> <span data-ttu-id="7ae33-155">Ответ также включает URL-адрес nextLink или URL-адрес deltaLink.</span><span class="sxs-lookup"><span data-stu-id="7ae33-155">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="7ae33-156">Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="7ae33-156">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="7ae33-157">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="7ae33-157">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="7ae33-158">Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="7ae33-158">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="7ae33-159">Следует оставить и использовать `deltaLink` URL-адрес для получения сведений об изменениях в ресурсе в будущем.</span><span class="sxs-lookup"><span data-stu-id="7ae33-159">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="7ae33-160">См. следующее:</span><span class="sxs-lookup"><span data-stu-id="7ae33-160">See:</span></span></br>
- <span data-ttu-id="7ae33-161">[Дополнительные сведения](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="7ae33-161">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="7ae33-162">[Примеры запросов](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="7ae33-162">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="7ae33-163">Пример</span><span class="sxs-lookup"><span data-stu-id="7ae33-163">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ae33-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ae33-164">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7ae33-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ae33-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/delta
```
# <a name="c"></a>[<span data-ttu-id="7ae33-166">C#</span><span class="sxs-lookup"><span data-stu-id="7ae33-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ae33-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ae33-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ae33-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ae33-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7ae33-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ae33-169">Response</span></span>
<span data-ttu-id="7ae33-p111">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ae33-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
