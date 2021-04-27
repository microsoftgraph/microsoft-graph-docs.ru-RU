---
title: 'приложение: дельта'
description: Получение новых, обновленных или удаленных приложений без выполнения полного чтения всей коллекции ресурсов. Подробные сведения см. в материале Использование запроса Delta.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: c3bfedbfdd8aa13e27b3daa1aaf6da3c67c645b5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048129"
---
# <a name="application-delta"></a><span data-ttu-id="549a0-104">приложение: дельта</span><span class="sxs-lookup"><span data-stu-id="549a0-104">application: delta</span></span>

<span data-ttu-id="549a0-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="549a0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="549a0-106">Получение новых, обновленных или удаленных приложений без выполнения полного чтения всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="549a0-106">Get newly created, updated, or deleted applications without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="549a0-107">Подробные [сведения см. в материале Использование запроса Delta.](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="549a0-107">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="549a0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="549a0-108">Permissions</span></span>

<span data-ttu-id="549a0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="549a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="549a0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="549a0-111">Permission type</span></span>      | <span data-ttu-id="549a0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="549a0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="549a0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="549a0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="549a0-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="549a0-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="549a0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="549a0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="549a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="549a0-116">Not supported.</span></span>    |
|<span data-ttu-id="549a0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="549a0-117">Application</span></span> | <span data-ttu-id="549a0-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="549a0-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="549a0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="549a0-119">HTTP request</span></span>

<span data-ttu-id="549a0-120">Чтобы начать отслеживание изменений, необходимо сделать запрос, включив функцию delta на ресурсе приложения.</span><span class="sxs-lookup"><span data-stu-id="549a0-120">To begin tracking changes, you make a request including the delta function on the application resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /applications/delta
```

### <a name="query-parameters"></a><span data-ttu-id="549a0-121">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="549a0-121">Query parameters</span></span>

<span data-ttu-id="549a0-122">Отслеживание изменений вызывает один или несколько вызовов функции **дельты.**</span><span class="sxs-lookup"><span data-stu-id="549a0-122">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="549a0-123">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="549a0-123">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="549a0-124">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="549a0-124">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="549a0-125">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="549a0-125">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="549a0-126">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="549a0-126">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="549a0-127">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="549a0-127">Query parameter</span></span>      | <span data-ttu-id="549a0-128">Тип</span><span class="sxs-lookup"><span data-stu-id="549a0-128">Type</span></span>   |<span data-ttu-id="549a0-129">Описание</span><span class="sxs-lookup"><span data-stu-id="549a0-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="549a0-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="549a0-130">$deltatoken</span></span> | <span data-ttu-id="549a0-131">string</span><span class="sxs-lookup"><span data-stu-id="549a0-131">string</span></span> | <span data-ttu-id="549a0-132">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущей функции дельты, вызываем для того же собрания ресурсов, что указывает на завершение этого раунда отслеживания `deltaLink` изменений. </span><span class="sxs-lookup"><span data-stu-id="549a0-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="549a0-133">Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="549a0-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="549a0-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="549a0-134">$skiptoken</span></span> | <span data-ttu-id="549a0-135">string</span><span class="sxs-lookup"><span data-stu-id="549a0-135">string</span></span> | <span data-ttu-id="549a0-136">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущего вызова функции дельты, указывает на то, что в том же собрании ресурсов необходимо отслеживать дальнейшие `nextLink` изменения. </span><span class="sxs-lookup"><span data-stu-id="549a0-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="549a0-137">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="549a0-137">Optional query parameters</span></span>

<span data-ttu-id="549a0-138">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="549a0-138">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="549a0-p106">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="549a0-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="549a0-141">Имеется ограниченная поддержка параметра `$filter`:</span><span class="sxs-lookup"><span data-stu-id="549a0-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="549a0-142">Единственным `$filter` поддерживаемым выражением является отслеживание изменений для определенных ресурсов по их id:  `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="549a0-142">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="549a0-143">Количество ids, которые можно указать, ограничено максимальной длиной URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="549a0-143">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="549a0-144">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="549a0-144">Request headers</span></span>
| <span data-ttu-id="549a0-145">Имя</span><span class="sxs-lookup"><span data-stu-id="549a0-145">Name</span></span>       | <span data-ttu-id="549a0-146">Описание</span><span class="sxs-lookup"><span data-stu-id="549a0-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="549a0-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="549a0-147">Authorization</span></span>  | <span data-ttu-id="549a0-148">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="549a0-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="549a0-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="549a0-149">Content-Type</span></span>  | <span data-ttu-id="549a0-150">application/json</span><span class="sxs-lookup"><span data-stu-id="549a0-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="549a0-151">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="549a0-151">Request body</span></span>
<span data-ttu-id="549a0-152">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="549a0-152">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="549a0-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="549a0-153">Response</span></span>

<span data-ttu-id="549a0-154">В случае успешного применения этот метод возвращает объект кода отклика и коллекции `200 OK` приложений в тексте отклика. [](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="549a0-154">If successful, this method returns `200 OK` response code and [application](../resources/application.md) collection object in the response body.</span></span> <span data-ttu-id="549a0-155">Ответ также включает URL-адрес nextLink или URL-адрес deltaLink.</span><span class="sxs-lookup"><span data-stu-id="549a0-155">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="549a0-156">Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="549a0-156">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="549a0-157">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="549a0-157">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="549a0-158">Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="549a0-158">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="549a0-159">Сохраните и используйте `deltaLink` URL-адрес, чтобы узнать об изменениях в ресурсе в будущем.</span><span class="sxs-lookup"><span data-stu-id="549a0-159">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="549a0-160">См. следующее:</span><span class="sxs-lookup"><span data-stu-id="549a0-160">See:</span></span></br>
- <span data-ttu-id="549a0-161">[Дополнительные сведения](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="549a0-161">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="549a0-162">[Примеры запросов](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="549a0-162">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="549a0-163">Пример</span><span class="sxs-lookup"><span data-stu-id="549a0-163">Example</span></span>
##### <a name="request"></a><span data-ttu-id="549a0-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="549a0-164">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="549a0-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="549a0-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/delta
```
# <a name="c"></a>[<span data-ttu-id="549a0-166">C#</span><span class="sxs-lookup"><span data-stu-id="549a0-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="549a0-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="549a0-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="549a0-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="549a0-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="549a0-169">Java</span><span class="sxs-lookup"><span data-stu-id="549a0-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="549a0-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="549a0-170">Response</span></span>
<span data-ttu-id="549a0-171">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="549a0-171">Note: The response object shown here might be shortened for readability.</span></span>
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
  "@odata.nextLink":"https://graph.microsoft.com/beta/applications/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "application: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



