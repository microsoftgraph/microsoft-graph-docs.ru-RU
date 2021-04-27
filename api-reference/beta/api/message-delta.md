---
title: 'message: delta'
description: Получение списка сообщений, которые были добавлены в указанную папку, обновлены в ней или удалены из нее.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 105c8bdbc14293e66f96bd8a69895da2c5e53790
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052154"
---
# <a name="message-delta"></a><span data-ttu-id="56422-103">message: delta</span><span class="sxs-lookup"><span data-stu-id="56422-103">message: delta</span></span>

<span data-ttu-id="56422-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56422-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56422-105">Получение списка сообщений, которые были добавлены в указанную папку, обновлены в ней или удалены из нее.</span><span class="sxs-lookup"><span data-stu-id="56422-105">Get a set of messages that have been added, deleted, or updated in a specified folder.</span></span>

<span data-ttu-id="56422-p101">Вызов функции **delta** для сообщений в папке похож на запрос GET, однако, правильно применяя [токены состояния](/graph/delta-query-overview) в этих вызовах, можно [запрашивать изменения в сообщениях папки](/graph/delta-query-messages). Это позволяет синхронизировать локальное хранилище сообщений пользователя, не загружая каждый раз весь набор сообщений с сервера.</span><span class="sxs-lookup"><span data-stu-id="56422-p101">A **delta** function call for messages in a folder is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can [query for incremental changes in the messages in that folder](/graph/delta-query-messages). This allows you to maintain and synchronize a local store of a user's messages without having to fetch the entire set of messages from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="56422-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56422-108">Permissions</span></span>
<span data-ttu-id="56422-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56422-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56422-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56422-111">Permission type</span></span>      | <span data-ttu-id="56422-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56422-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56422-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56422-113">Delegated (work or school account)</span></span> | <span data-ttu-id="56422-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56422-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="56422-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56422-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56422-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56422-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="56422-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="56422-117">Application</span></span> | <span data-ttu-id="56422-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56422-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="56422-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56422-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/delta
GET /users/{id}/mailFolders/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="56422-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="56422-120">Query parameters</span></span>

<span data-ttu-id="56422-p103">Отслеживание изменений в сообщениях — это цикл из одного или нескольких вызовов функции **delta**. Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в первом запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в токене, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в ответ. Параметры запроса нужно указать только один раз в первом запросе. Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="56422-p103">Tracking changes in messages incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="56422-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="56422-126">Query parameter</span></span>      | <span data-ttu-id="56422-127">Тип</span><span class="sxs-lookup"><span data-stu-id="56422-127">Type</span></span>   |<span data-ttu-id="56422-128">Описание</span><span class="sxs-lookup"><span data-stu-id="56422-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="56422-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="56422-129">$deltatoken</span></span> | <span data-ttu-id="56422-130">string</span><span class="sxs-lookup"><span data-stu-id="56422-130">string</span></span> | <span data-ttu-id="56422-p104">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции сообщений и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="56422-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same message collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="56422-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="56422-133">$skiptoken</span></span> | <span data-ttu-id="56422-134">строка</span><span class="sxs-lookup"><span data-stu-id="56422-134">string</span></span> | <span data-ttu-id="56422-135">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что из коллекции сообщений получены не все изменения.</span><span class="sxs-lookup"><span data-stu-id="56422-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same message collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="56422-136">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="56422-136">OData query parameters</span></span>

- <span data-ttu-id="56422-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="56422-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="56422-139">Запросы изменений поддерживают параметры `$select`, `$top` и `$expand` для сообщений.</span><span class="sxs-lookup"><span data-stu-id="56422-139">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="56422-140">Имеется ограниченная поддержка параметров `$filter` и `$orderby`:</span><span class="sxs-lookup"><span data-stu-id="56422-140">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="56422-141">Для параметра `$filter` поддерживаются только выражения `$filter=receivedDateTime+ge+{value}` и `$filter=receivedDateTime+gt+{value}`.</span><span class="sxs-lookup"><span data-stu-id="56422-141">The only supported `$filter` expresssions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  * <span data-ttu-id="56422-p106">Для параметра `$orderby` поддерживается только выражение `$orderby=receivedDateTime+desc`. Если выражение `$orderby` не указано, результаты будут возвращаться в непредсказуемом порядке.</span><span class="sxs-lookup"><span data-stu-id="56422-p106">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="56422-144">Параметр `$search` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56422-144">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56422-145">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56422-145">Request headers</span></span>
| <span data-ttu-id="56422-146">Имя</span><span class="sxs-lookup"><span data-stu-id="56422-146">Name</span></span>       | <span data-ttu-id="56422-147">Тип</span><span class="sxs-lookup"><span data-stu-id="56422-147">Type</span></span> | <span data-ttu-id="56422-148">Описание</span><span class="sxs-lookup"><span data-stu-id="56422-148">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="56422-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="56422-149">Authorization</span></span>  | <span data-ttu-id="56422-150">string</span><span class="sxs-lookup"><span data-stu-id="56422-150">string</span></span>  | <span data-ttu-id="56422-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56422-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56422-153">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56422-153">Content-Type</span></span>  | <span data-ttu-id="56422-154">string</span><span class="sxs-lookup"><span data-stu-id="56422-154">string</span></span>  | <span data-ttu-id="56422-p108">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56422-p108">application/json. Required.</span></span> |
| <span data-ttu-id="56422-157">Prefer</span><span class="sxs-lookup"><span data-stu-id="56422-157">Prefer</span></span> | <span data-ttu-id="56422-158">string</span><span class="sxs-lookup"><span data-stu-id="56422-158">string</span></span>  | <span data-ttu-id="56422-p109">odata.maxpagesize={x}. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="56422-p109">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="56422-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="56422-161">Response</span></span>

<span data-ttu-id="56422-162">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [message](../resources/message.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="56422-162">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56422-163">Пример</span><span class="sxs-lookup"><span data-stu-id="56422-163">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56422-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="56422-164">Request</span></span>
<span data-ttu-id="56422-165">В следующем примере показано, как выполнить один вызов функции **delta** и ограничить максимальное количество сообщений в тексте ответа до 2.</span><span class="sxs-lookup"><span data-stu-id="56422-165">The following example shows how to make a single **delta** function call, and limit the maximum number of messages in the response body to 2.</span></span>

<span data-ttu-id="56422-p110">Чтобы отследить изменения в сообщениях папки, выполните один или несколько вызовов функции **delta**, чтобы получить набор изменений с момента последнего запроса. Пример, в котором показан цикл запросов изменений: [Получение добавочных изменений для сообщений в папке](/graph/delta-query-messages).</span><span class="sxs-lookup"><span data-stu-id="56422-p110">To track changes in the messages in a folder, you would make one or more **delta** function calls to get the set of incremental changes since the last delta query. For an example that shows a round of delta query calls, see [Get incremental changes to messages in a folder](/graph/delta-query-messages).</span></span>
 

# <a name="http"></a>[<span data-ttu-id="56422-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="56422-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/{id}/messages/delta

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="56422-169">C#</span><span class="sxs-lookup"><span data-stu-id="56422-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56422-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56422-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56422-171">Java</span><span class="sxs-lookup"><span data-stu-id="56422-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="56422-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="56422-172">Response</span></span>
<span data-ttu-id="56422-173">В случае успешного выполнения запроса отклик будет содержать маркер состояния — _skipToken_</span><span class="sxs-lookup"><span data-stu-id="56422-173">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="56422-p111">или _deltaToken_. Первый включен в заголовок отклика _@odata.nextLink_, второй — в заголовок отклика _@odata.deltaLink_. Первый указывает на необходимость продолжать цикл, второй — на наличие всех изменений для определенного цикла.</span><span class="sxs-lookup"><span data-stu-id="56422-p111">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="56422-176">Ниже показан отклик с маркером состояния _skipToken_ в заголовке отклика _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="56422-176">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="56422-177">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="56422-177">Note: The response object shown here might be shortened for readability.</span></span>
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
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/mailfolders/{id}/messages/delta?$skiptoken={_skipToken_}",
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

### <a name="see-also"></a><span data-ttu-id="56422-178">См. также</span><span class="sxs-lookup"><span data-stu-id="56422-178">See also</span></span>

- [<span data-ttu-id="56422-179">Запрос изменений Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="56422-179">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="56422-180">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="56422-180">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


