---
title: 'directoryRole: Delta'
description: Получение только что созданных, обновленных или удаленных ролей каталогов без выполнения полного чтения всей коллекции ресурсов. Сведения об использовании запроса изменений см.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1a8c755fbdadca7926c9f7bce9179e4ce74953e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517960"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="277f9-104">directoryRole: Delta</span><span class="sxs-lookup"><span data-stu-id="277f9-104">directoryRole: delta</span></span>

<span data-ttu-id="277f9-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="277f9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="277f9-106">Получение только что созданных, обновленных или удаленных ролей каталогов без выполнения полного чтения всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="277f9-106">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="277f9-107">Сведения об [использовании запроса изменений](/graph/delta-query-overview) см.</span><span class="sxs-lookup"><span data-stu-id="277f9-107">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="277f9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="277f9-108">Permissions</span></span>

<span data-ttu-id="277f9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="277f9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="277f9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="277f9-111">Permission type</span></span>      | <span data-ttu-id="277f9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="277f9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="277f9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="277f9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="277f9-114">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="277f9-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="277f9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="277f9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="277f9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="277f9-116">Not supported.</span></span>    |
|<span data-ttu-id="277f9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="277f9-117">Application</span></span> | <span data-ttu-id="277f9-118">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="277f9-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="277f9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="277f9-119">HTTP request</span></span>

<span data-ttu-id="277f9-120">Чтобы начать отслеживание изменений, создайте запрос, включающий функцию **Delta** в ресурсе [directoryRole](../resources/directoryrole.md) .</span><span class="sxs-lookup"><span data-stu-id="277f9-120">To begin tracking changes, you make a request including the **delta** function on the [directoryRole](../resources/directoryrole.md) resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

## <a name="query-parameters"></a><span data-ttu-id="277f9-121">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="277f9-121">Query parameters</span></span>

<span data-ttu-id="277f9-122">Отслеживание изменений приводит к округлению одного или нескольких вызовов функции **Delta** .</span><span class="sxs-lookup"><span data-stu-id="277f9-122">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="277f9-123">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="277f9-123">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="277f9-124">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="277f9-124">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="277f9-125">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="277f9-125">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="277f9-126">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="277f9-126">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="277f9-127">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="277f9-127">Query parameter</span></span>      | <span data-ttu-id="277f9-128">Тип</span><span class="sxs-lookup"><span data-stu-id="277f9-128">Type</span></span>   |<span data-ttu-id="277f9-129">Описание</span><span class="sxs-lookup"><span data-stu-id="277f9-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="277f9-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="277f9-130">$deltatoken</span></span> | <span data-ttu-id="277f9-131">string</span><span class="sxs-lookup"><span data-stu-id="277f9-131">string</span></span> | <span data-ttu-id="277f9-132">[Токен состояния](/graph/delta-query-overview) возвращается в `deltaLink` URL-адресе предыдущего вызова функции **Delta** для той же коллекции ресурсов, что указывает на завершение этого круга отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="277f9-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="277f9-133">Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="277f9-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="277f9-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="277f9-134">$skiptoken</span></span> | <span data-ttu-id="277f9-135">string</span><span class="sxs-lookup"><span data-stu-id="277f9-135">string</span></span> | <span data-ttu-id="277f9-136">[Токен состояния](/graph/delta-query-overview) возвращается в `nextLink` URL-адресе предыдущего вызова функции **Delta** , указывая, что в коллекции ресурсов отслеживаются другие изменения.</span><span class="sxs-lookup"><span data-stu-id="277f9-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="277f9-137">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="277f9-137">OData query parameters</span></span>

<span data-ttu-id="277f9-138">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="277f9-138">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="277f9-p106">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="277f9-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span>

- <span data-ttu-id="277f9-141">Имеется ограниченная поддержка параметра `$filter`:</span><span class="sxs-lookup"><span data-stu-id="277f9-141">There is limited support for `$filter`:</span></span>

  - <span data-ttu-id="277f9-142">Единственное поддерживаемое `$filter` выражение предназначено для отслеживания изменений для определенных ресурсов по их идентификаторам: `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="277f9-142">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="277f9-143">Количество идентификаторов, которые можно указать, ограничено максимальной длиной URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="277f9-143">The number of ids you can specify is limited by the maximum URL length.</span></span>

## <a name="request-headers"></a><span data-ttu-id="277f9-144">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="277f9-144">Request headers</span></span>

| <span data-ttu-id="277f9-145">Имя</span><span class="sxs-lookup"><span data-stu-id="277f9-145">Name</span></span>       | <span data-ttu-id="277f9-146">Описание</span><span class="sxs-lookup"><span data-stu-id="277f9-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="277f9-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="277f9-147">Authorization</span></span>  | <span data-ttu-id="277f9-148">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="277f9-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="277f9-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="277f9-149">Content-Type</span></span>  | <span data-ttu-id="277f9-150">application/json</span><span class="sxs-lookup"><span data-stu-id="277f9-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="277f9-151">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="277f9-151">Request body</span></span>

<span data-ttu-id="277f9-152">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="277f9-152">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="277f9-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="277f9-153">Response</span></span>

<span data-ttu-id="277f9-154">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект коллекции [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="277f9-154">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="277f9-155">Отклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="277f9-155">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="277f9-156">Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="277f9-156">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="277f9-157">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="277f9-157">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="277f9-158">Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="277f9-158">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="277f9-159">Сохраните `deltaLink` URL-адрес и примените его в следующем **Дельта** -вызове, чтобы узнать об изменениях в ресурсе в будущем.</span><span class="sxs-lookup"><span data-stu-id="277f9-159">Save `deltaLink` URL and apply it in the next **delta** call to learn about changes to the resource in the future.</span></span>

### <a name="example"></a><span data-ttu-id="277f9-160">Пример</span><span class="sxs-lookup"><span data-stu-id="277f9-160">Example</span></span>

##### <a name="request"></a><span data-ttu-id="277f9-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="277f9-161">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="277f9-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="277f9-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/delta
```
# <a name="c"></a>[<span data-ttu-id="277f9-163">C#</span><span class="sxs-lookup"><span data-stu-id="277f9-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryrole-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="277f9-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="277f9-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryrole-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="277f9-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="277f9-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryrole-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="277f9-166">Java</span><span class="sxs-lookup"><span data-stu-id="277f9-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryrole-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="277f9-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="277f9-167">Response</span></span>

<span data-ttu-id="277f9-p111">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="277f9-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryRoles",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/directoryRoles/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
      {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="277f9-170">См. также</span><span class="sxs-lookup"><span data-stu-id="277f9-170">See also</span></span>

- <span data-ttu-id="277f9-171">[Использование запроса изменений для отслеживания изменений в данных Microsoft Graph](/graph/delta-query-overview) для получения дополнительных сведений</span><span class="sxs-lookup"><span data-stu-id="277f9-171">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview) for more details</span></span>
- <span data-ttu-id="277f9-172">[Примеры запросов](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="277f9-172">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span>

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
