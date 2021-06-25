---
title: 'directoryRole: delta'
description: Создайте новые, обновленные или удаленные роли каталога, не выполняя полное чтение всей коллекции ресурсов. Подробные сведения см. в материале Использование запроса Delta.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 177c875f204a4019884fb025a2f06dc365e4a63b
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118653"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="a4a30-104">directoryRole: delta</span><span class="sxs-lookup"><span data-stu-id="a4a30-104">directoryRole: delta</span></span>

<span data-ttu-id="a4a30-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4a30-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a4a30-106">Создайте новые, обновленные или удаленные роли каталога, не выполняя полное чтение всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a4a30-106">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="a4a30-107">Подробные [сведения см. в материале Использование запроса Delta.](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="a4a30-107">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4a30-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4a30-108">Permissions</span></span>

<span data-ttu-id="a4a30-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4a30-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a4a30-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4a30-111">Permission type</span></span>      | <span data-ttu-id="a4a30-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4a30-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4a30-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4a30-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a4a30-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a4a30-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a4a30-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4a30-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4a30-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4a30-116">Not supported.</span></span>    |
|<span data-ttu-id="a4a30-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a4a30-117">Application</span></span> | <span data-ttu-id="a4a30-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4a30-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4a30-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4a30-119">HTTP request</span></span>

<span data-ttu-id="a4a30-120">Чтобы начать отслеживание изменений, необходимо сделать запрос, включив функцию **дельты** на [ресурсе directoryRole.](../resources/directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="a4a30-120">To begin tracking changes, you make a request including the **delta** function on the [directoryRole](../resources/directoryrole.md) resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

## <a name="query-parameters"></a><span data-ttu-id="a4a30-121">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="a4a30-121">Query parameters</span></span>

<span data-ttu-id="a4a30-122">Отслеживание изменений вызывает один или несколько вызовов функции **дельты.**</span><span class="sxs-lookup"><span data-stu-id="a4a30-122">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="a4a30-123">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="a4a30-123">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="a4a30-124">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="a4a30-124">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="a4a30-125">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="a4a30-125">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="a4a30-126">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="a4a30-126">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="a4a30-127">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="a4a30-127">Query parameter</span></span>      | <span data-ttu-id="a4a30-128">Тип</span><span class="sxs-lookup"><span data-stu-id="a4a30-128">Type</span></span>   |<span data-ttu-id="a4a30-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a4a30-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a4a30-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="a4a30-130">$deltatoken</span></span> | <span data-ttu-id="a4a30-131">string</span><span class="sxs-lookup"><span data-stu-id="a4a30-131">string</span></span> | <span data-ttu-id="a4a30-132">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущей функции дельты, вызываем для того же собрания ресурсов, что указывает на завершение этого раунда отслеживания `deltaLink` изменений. </span><span class="sxs-lookup"><span data-stu-id="a4a30-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="a4a30-133">Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="a4a30-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="a4a30-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="a4a30-134">$skiptoken</span></span> | <span data-ttu-id="a4a30-135">string</span><span class="sxs-lookup"><span data-stu-id="a4a30-135">string</span></span> | <span data-ttu-id="a4a30-136">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущего вызова функции дельты, указывает на то, что в том же собрании ресурсов необходимо отслеживать дальнейшие `nextLink` изменения. </span><span class="sxs-lookup"><span data-stu-id="a4a30-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="a4a30-137">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="a4a30-137">OData query parameters</span></span>

<span data-ttu-id="a4a30-138">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a4a30-138">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="a4a30-p106">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="a4a30-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span>

- <span data-ttu-id="a4a30-141">Имеется ограниченная поддержка параметра `$filter`:</span><span class="sxs-lookup"><span data-stu-id="a4a30-141">There is limited support for `$filter`:</span></span>

  - <span data-ttu-id="a4a30-142">Единственным `$filter` поддерживаемым выражением является отслеживание изменений для определенных ресурсов по их id:  `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="a4a30-142">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="a4a30-143">Количество ids, которые можно указать, ограничено максимальной длиной URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="a4a30-143">The number of ids you can specify is limited by the maximum URL length.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4a30-144">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4a30-144">Request headers</span></span>

| <span data-ttu-id="a4a30-145">Имя</span><span class="sxs-lookup"><span data-stu-id="a4a30-145">Name</span></span>       | <span data-ttu-id="a4a30-146">Описание</span><span class="sxs-lookup"><span data-stu-id="a4a30-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a4a30-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4a30-147">Authorization</span></span>  | <span data-ttu-id="a4a30-148">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="a4a30-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="a4a30-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4a30-149">Content-Type</span></span>  | <span data-ttu-id="a4a30-150">application/json</span><span class="sxs-lookup"><span data-stu-id="a4a30-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4a30-151">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4a30-151">Request body</span></span>

<span data-ttu-id="a4a30-152">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4a30-152">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="a4a30-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4a30-153">Response</span></span>

<span data-ttu-id="a4a30-154">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект коллекции directoryRole](../resources/directoryrole.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a4a30-154">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="a4a30-155">Отклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="a4a30-155">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="a4a30-156">Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="a4a30-156">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="a4a30-157">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="a4a30-157">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="a4a30-158">Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="a4a30-158">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="a4a30-159">Сохраните URL-адрес и примените его в следующем вызове delta, чтобы узнать об изменениях `deltaLink` в ресурсе в будущем. </span><span class="sxs-lookup"><span data-stu-id="a4a30-159">Save `deltaLink` URL and apply it in the next **delta** call to learn about changes to the resource in the future.</span></span>

### <a name="example"></a><span data-ttu-id="a4a30-160">Пример</span><span class="sxs-lookup"><span data-stu-id="a4a30-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a4a30-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4a30-161">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a4a30-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4a30-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/delta
```
# <a name="c"></a>[<span data-ttu-id="a4a30-163">C#</span><span class="sxs-lookup"><span data-stu-id="a4a30-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryrole-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4a30-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4a30-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryrole-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4a30-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4a30-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryrole-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4a30-166">Java</span><span class="sxs-lookup"><span data-stu-id="a4a30-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryrole-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a4a30-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4a30-167">Response</span></span>

><span data-ttu-id="a4a30-168">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a4a30-168">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryRoles",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/directoryRoles/delta?$skiptoken=pkXMyA5aFCIMmH1Kk1XEAnf2X-fodqXKXF03gYPQknSHRxogVsxvSq_26nhos-O2-shortened",
  "value": [
    {
      "description": "Device Administrators",
      "displayName": "Azure AD Joined Device Local Administrator",
      "roleTemplateId": "9f06204d-73c1-4d4c-880a-6edb90606fd8",
      "id": "f8e85ed8-f66f-4058-b170-3efae8b9c6e5",
      "members@delta": [
        {
          "@odata.type": "#microsoft.graph.user",
          "id": "bb165b45-151c-4cf6-9911-cd7188912848",
          "@removed": {
            "reason": "deleted"
          }
        }
      ]
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="a4a30-169">См. также</span><span class="sxs-lookup"><span data-stu-id="a4a30-169">See also</span></span>

- <span data-ttu-id="a4a30-170">[Дополнительные сведения можно получить](/graph/delta-query-overview) с помощью запроса delta для отслеживания изменений в Graph microsoft Graph данных</span><span class="sxs-lookup"><span data-stu-id="a4a30-170">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview) for more details</span></span>
- <span data-ttu-id="a4a30-171">[Примеры запросов](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="a4a30-171">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

