---
title: 'message: delta'
description: Получение списка сообщений, которые были добавлены в указанную папку, обновлены в ней или удалены из нее.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: dd17762c32a20b07a7c68c58d37f4db103123bc0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275028"
---
# <a name="message-delta"></a><span data-ttu-id="c25bc-103">message: delta</span><span class="sxs-lookup"><span data-stu-id="c25bc-103">message: delta</span></span>

<span data-ttu-id="c25bc-104">Получение списка сообщений, которые были добавлены в указанную папку, обновлены в ней или удалены из нее.</span><span class="sxs-lookup"><span data-stu-id="c25bc-104">Get a set of messages that have been added, deleted, or updated in a specified folder.</span></span>

<span data-ttu-id="c25bc-p101">Вызов функции **delta** для сообщений в папке похож на запрос GET, однако, правильно применяя [токены состояния](/graph/delta-query-overview) в этих вызовах, можно [запрашивать изменения в сообщениях папки](/graph/delta-query-messages). Это позволяет синхронизировать локальное хранилище сообщений пользователя, не загружая каждый раз весь набор сообщений с сервера.</span><span class="sxs-lookup"><span data-stu-id="c25bc-p101">A **delta** function call for messages in a folder is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can [query for incremental changes in the messages in that folder](/graph/delta-query-messages). This allows you to maintain and synchronize a local store of a user's messages without having to fetch the entire set of messages from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="c25bc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c25bc-107">Permissions</span></span>
<span data-ttu-id="c25bc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c25bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c25bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c25bc-110">Permission type</span></span>      | <span data-ttu-id="c25bc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c25bc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c25bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c25bc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c25bc-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c25bc-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c25bc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c25bc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c25bc-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c25bc-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c25bc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c25bc-116">Application</span></span> | <span data-ttu-id="c25bc-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c25bc-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c25bc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c25bc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/delta
GET /users/{id}/mailFolders/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="c25bc-119">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="c25bc-119">Query parameters</span></span>

<span data-ttu-id="c25bc-p103">Отслеживание изменений в сообщениях — это цикл из одного или нескольких вызовов функции **delta**. Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в первом запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в токене, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в ответ. Параметры запроса нужно указать только один раз в первом запросе. Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="c25bc-p103">Tracking changes in messages incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="c25bc-125">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="c25bc-125">Query parameter</span></span>      | <span data-ttu-id="c25bc-126">Тип</span><span class="sxs-lookup"><span data-stu-id="c25bc-126">Type</span></span>   |<span data-ttu-id="c25bc-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c25bc-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c25bc-128">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="c25bc-128">$deltatoken</span></span> | <span data-ttu-id="c25bc-129">string</span><span class="sxs-lookup"><span data-stu-id="c25bc-129">string</span></span> | <span data-ttu-id="c25bc-p104">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции сообщений и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="c25bc-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same message collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="c25bc-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="c25bc-132">$skiptoken</span></span> | <span data-ttu-id="c25bc-133">строка</span><span class="sxs-lookup"><span data-stu-id="c25bc-133">string</span></span> | <span data-ttu-id="c25bc-134">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что из коллекции сообщений получены не все изменения.</span><span class="sxs-lookup"><span data-stu-id="c25bc-134">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same message collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="c25bc-135">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="c25bc-135">OData query parameters</span></span>

- <span data-ttu-id="c25bc-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="c25bc-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="c25bc-138">Запросы изменений поддерживают параметры `$select`, `$top` и `$expand` для сообщений.</span><span class="sxs-lookup"><span data-stu-id="c25bc-138">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="c25bc-139">Имеется ограниченная поддержка параметров `$filter` и `$orderby`:</span><span class="sxs-lookup"><span data-stu-id="c25bc-139">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="c25bc-140">Для параметра `$filter` поддерживаются только выражения `$filter=receivedDateTime+ge+{value}` и `$filter=receivedDateTime+gt+{value}`.</span><span class="sxs-lookup"><span data-stu-id="c25bc-140">The only supported `$filter` expresssions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  * <span data-ttu-id="c25bc-p106">Для параметра `$orderby` поддерживается только выражение `$orderby=receivedDateTime+desc`. Если выражение `$orderby` не указано, результаты будут возвращаться в непредсказуемом порядке.</span><span class="sxs-lookup"><span data-stu-id="c25bc-p106">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="c25bc-143">Параметр `$search` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c25bc-143">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c25bc-144">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c25bc-144">Request headers</span></span>
| <span data-ttu-id="c25bc-145">Имя</span><span class="sxs-lookup"><span data-stu-id="c25bc-145">Name</span></span>       | <span data-ttu-id="c25bc-146">Тип</span><span class="sxs-lookup"><span data-stu-id="c25bc-146">Type</span></span> | <span data-ttu-id="c25bc-147">Описание</span><span class="sxs-lookup"><span data-stu-id="c25bc-147">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="c25bc-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="c25bc-148">Authorization</span></span>  | <span data-ttu-id="c25bc-149">string</span><span class="sxs-lookup"><span data-stu-id="c25bc-149">string</span></span>  | <span data-ttu-id="c25bc-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c25bc-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c25bc-152">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c25bc-152">Content-Type</span></span>  | <span data-ttu-id="c25bc-153">string</span><span class="sxs-lookup"><span data-stu-id="c25bc-153">string</span></span>  | <span data-ttu-id="c25bc-p108">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c25bc-p108">application/json. Required.</span></span> |
| <span data-ttu-id="c25bc-156">Prefer</span><span class="sxs-lookup"><span data-stu-id="c25bc-156">Prefer</span></span> | <span data-ttu-id="c25bc-157">string</span><span class="sxs-lookup"><span data-stu-id="c25bc-157">string</span></span>  | <span data-ttu-id="c25bc-p109">odata.maxpagesize={x}. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c25bc-p109">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c25bc-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="c25bc-160">Response</span></span>

<span data-ttu-id="c25bc-161">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [message](../resources/message.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c25bc-161">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c25bc-162">Пример</span><span class="sxs-lookup"><span data-stu-id="c25bc-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c25bc-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="c25bc-163">Request</span></span>
<span data-ttu-id="c25bc-164">В следующем примере показано, как выполнить один вызов функции **delta** и ограничить максимальное количество сообщений в тексте ответа до 2.</span><span class="sxs-lookup"><span data-stu-id="c25bc-164">The following example shows how to make a single **delta** function call, and limit the maximum number of messages in the response body to 2.</span></span>

<span data-ttu-id="c25bc-p110">Чтобы отследить изменения в сообщениях папки, выполните один или несколько вызовов функции **delta**, чтобы получить набор изменений с момента последнего запроса. Пример, в котором показан цикл запросов изменений: [Получение добавочных изменений для сообщений в папке](/graph/delta-query-messages).</span><span class="sxs-lookup"><span data-stu-id="c25bc-p110">To track changes in the messages in a folder, you would make one or more **delta** function calls to get the set of incremental changes since the last delta query. For an example that shows a round of delta query calls, see [Get incremental changes to messages in a folder](/graph/delta-query-messages).</span></span>
 
<!-- {
  "blockType": "request",
  "name": "message_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta
Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="c25bc-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="c25bc-167">Response</span></span>
<span data-ttu-id="c25bc-168">В случае успешного выполнения запроса отклик будет содержать маркер состояния — _skipToken_</span><span class="sxs-lookup"><span data-stu-id="c25bc-168">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="c25bc-p111">или _deltaToken_. Первый включен в заголовок отклика _@odata.nextLink_, второй — в заголовок отклика _@odata.deltaLink_. Первый указывает на необходимость продолжать цикл, второй — на наличие всех изменений для определенного цикла.</span><span class="sxs-lookup"><span data-stu-id="c25bc-p111">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="c25bc-171">Ниже показан отклик с маркером состояния _skipToken_ в заголовке отклика _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="c25bc-171">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="c25bc-p112">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c25bc-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 337

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders('{id}')/messages/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "internetMessageId": "internetMessageId-value",
      "subject": "subject-value",
      "body": {
        "contentType": "contentType-value",
        "content": "content-value"
      }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c25bc-174">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c25bc-174">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c25bc-175">C#</span><span class="sxs-lookup"><span data-stu-id="c25bc-175">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_delta-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c25bc-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c25bc-176">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_delta-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c25bc-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c25bc-177">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_delta-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="see-also"></a><span data-ttu-id="c25bc-178">См. также</span><span class="sxs-lookup"><span data-stu-id="c25bc-178">See also</span></span>

- [<span data-ttu-id="c25bc-179">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="c25bc-179">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="c25bc-180">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="c25bc-180">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-delta.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-delta.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-delta.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
