---
title: 'chatMessages: delta'
description: Получение списка сообщений (без ответов) в канале команды. С помощью разностного запроса можно получить новые или обновленные сообщения в канале.
localization_priority: Priority
doc_type: apiPageType
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: e5f297dc236899f0fbd362c7ef369897b7bc7786
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719924"
---
# <a name="chatmessages-delta"></a><span data-ttu-id="c452a-104">chatMessages: delta</span><span class="sxs-lookup"><span data-stu-id="c452a-104">chatMessages: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c452a-105">Получение списка [сообщений](../resources/chatmessage.md) (без ответов) в [канале](../resources/channel.md) [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="c452a-105">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="c452a-106">С помощью разностного запроса можно получить новые или обновленные сообщения в канале.</span><span class="sxs-lookup"><span data-stu-id="c452a-106">By using delta query, you can get new or updated messages in a channel.</span></span>

<span data-ttu-id="c452a-107">Запрос изменений поддерживает как полную синхронизацию с получением всех сообщений в определенном канале, так и добавочную синхронизацию с получением тех сообщений, которые были добавлены или изменены в канале с момента последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c452a-107">Delta query supports both full synchronization that retrieves all the events in the specified calendar view, and incremental synchronization that retrieves those events that have changed in the calendar view since the last synchronization.</span></span> <span data-ttu-id="c452a-108">Как правило, сначала выполняется полная синхронизация, а затем в представление календаря периодически добавляются изменения.</span><span class="sxs-lookup"><span data-stu-id="c452a-108">Typically, you would do an initial full synchronization, and subsequently, get incremental changes to that calendar view periodically.</span></span>

<span data-ttu-id="c452a-109">Чтобы получить ответы на сообщение, используйте операцию [перечисления ответов на сообщение](channel-get-messagereply.md) или [получения ответа на сообщение](channel-list-messagereplies.md).</span><span class="sxs-lookup"><span data-stu-id="c452a-109">To get the replies for a message, call the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) API.</span></span>

<span data-ttu-id="c452a-110">Запрос GET с функцией delta возвращает одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="c452a-110">A GET request with the delta function returns either:</span></span>

- <span data-ttu-id="c452a-111">ссылку `nextLink` (содержащую URL-адрес с вызовом функции **delta** и `skipToken`), или</span><span class="sxs-lookup"><span data-stu-id="c452a-111">A `nextLink` (that contains a URL with a **delta** function call and a `skipToken`), or</span></span>
- <span data-ttu-id="c452a-112">ссылку `deltaLink` (содержащую URL-адрес с вызовом функции **delta** и `deltaToken`).</span><span class="sxs-lookup"><span data-stu-id="c452a-112">A `deltaLink` (that contains a URL with a **delta** function call and `deltaToken`).</span></span>

<span data-ttu-id="c452a-113">Маркеры состояния полностью непрозрачны для клиента.</span><span class="sxs-lookup"><span data-stu-id="c452a-113">State tokens are completely opaque to the client.</span></span> <span data-ttu-id="c452a-114">Чтобы продолжить цикл отслеживания изменений, просто скопируйте и примените URL-адрес `nextLink` или `deltaLink`, возвращенный последним запросом GET, при следующем вызове функции delta для этого представления календаря.</span><span class="sxs-lookup"><span data-stu-id="c452a-114">To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next delta function call for that same calendar view.</span></span> <span data-ttu-id="c452a-115">Ссылка `deltaLink` в ответе означает, что текущий цикл отслеживания изменений завершен.</span><span class="sxs-lookup"><span data-stu-id="c452a-115">A `deltaLink` returned in a response signifies that the current round of change tracking is complete.</span></span> <span data-ttu-id="c452a-116">Вы можете сохранить и использовать URL-адрес `deltaLink` в начале следующего цикла.</span><span class="sxs-lookup"><span data-stu-id="c452a-116">You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="c452a-117">Дополнительные сведения см. в документации по [разностному запросу](/graph/delta-query-overview.md).</span><span class="sxs-lookup"><span data-stu-id="c452a-117">For more information, see the [delta query](/graph/delta-query-overview.md) documentation.</span></span>

## <a name="permissions"></a><span data-ttu-id="c452a-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c452a-118">Permissions</span></span>

<span data-ttu-id="c452a-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c452a-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="c452a-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c452a-121">Permission Type</span></span>                        |<span data-ttu-id="c452a-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c452a-122">Permissions (from least to most privileged)</span></span>  |
|---------------------------------------|---------------------------------------------|
|<span data-ttu-id="c452a-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c452a-123">Delegated (work or school account)</span></span>     |<span data-ttu-id="c452a-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c452a-124">Group.Read.All, Group.ReadWrite.All</span></span>          |
|<span data-ttu-id="c452a-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c452a-125">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c452a-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c452a-126">Not Supported</span></span>                                |
|<span data-ttu-id="c452a-127">Приложение</span><span class="sxs-lookup"><span data-stu-id="c452a-127">Application</span></span>                            |<span data-ttu-id="c452a-128">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c452a-128">Group.Read.All, Group.ReadWrite.All</span></span>          |

## <a name="http-request"></a><span data-ttu-id="c452a-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c452a-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="c452a-130">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="c452a-130">Query parameters</span></span>

<span data-ttu-id="c452a-131">Отслеживание изменений в сообщениях в канале — это цикл из одного или нескольких вызовов функции **delta**.</span><span class="sxs-lookup"><span data-stu-id="c452a-131">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="c452a-132">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="c452a-132">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="c452a-133">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="c452a-133">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="c452a-134">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="c452a-134">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="c452a-135">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержатся закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="c452a-135">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="c452a-136">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="c452a-136">Query parameter</span></span>      | <span data-ttu-id="c452a-137">Тип</span><span class="sxs-lookup"><span data-stu-id="c452a-137">Type</span></span>   |<span data-ttu-id="c452a-138">Описание</span><span class="sxs-lookup"><span data-stu-id="c452a-138">Description</span></span>|
|:---------------|:--------|:----------|
| `$deltatoken` | <span data-ttu-id="c452a-139">string</span><span class="sxs-lookup"><span data-stu-id="c452a-139">string</span></span> | <span data-ttu-id="c452a-140">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` при предыдущем вызове функции **delta** и указывает на завершение этого цикла отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="c452a-140">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire  URL including this token in the first request of the next round of change tracking for that collection.</span></span> <span data-ttu-id="c452a-141">Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="c452a-141">A state token returned in the  URL of the previous delta function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| `$skiptoken` | <span data-ttu-id="c452a-142">string</span><span class="sxs-lookup"><span data-stu-id="c452a-142">string</span></span> | <span data-ttu-id="c452a-143">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` при предыдущем вызове функции **delta** и указывает на то, что  остаются не отслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="c452a-143">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="optional-odata-query-parameters"></a><span data-ttu-id="c452a-144">Необязательные параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="c452a-144">Optional OData query parameters</span></span>

<span data-ttu-id="c452a-145">Этим API поддерживаются указанные ниже [параметры запросов OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c452a-145">The following [OData query parameters](/graph/query-parameters) are supported by this API:</span></span>
- <span data-ttu-id="c452a-146">`$top`, указывает максимальное количество сообщений, которое нужно получить в результате вызова.</span><span class="sxs-lookup"><span data-stu-id="c452a-146">`$top`, represents maximum number of messages to fetch in a call.</span></span> <span data-ttu-id="c452a-147">Верхний предел – **50**.</span><span class="sxs-lookup"><span data-stu-id="c452a-147">The upper limit is **50**.</span></span>
- <span data-ttu-id="c452a-148">`$skip`, указывает, сколько сообщений нужно пропустить в начале списка.</span><span class="sxs-lookup"><span data-stu-id="c452a-148">`$skip`, represents how many messages to skip at the beginning of the list.</span></span>
- <span data-ttu-id="c452a-149">`$filter` поддерживает возврат сообщений, удовлетворяющих определенным условиям.</span><span class="sxs-lookup"><span data-stu-id="c452a-149">`$filter` allows returning messages that meet a certain criteria.</span></span> <span data-ttu-id="c452a-150">Единственное свойство, поддерживающее фильтрацию, – это `lastModifiedDateTime`, при этом поддерживаются только операторы **gt** и **ge**.</span><span class="sxs-lookup"><span data-stu-id="c452a-150">The only property that supports filtering is `lastModifiedDateTime`, and only the **gt** and **ge** operators are supported.</span></span> <span data-ttu-id="c452a-151">Например, `../messages/delta?$filter=lastModifiedDateTime ge 2019-02-27T07:13:28.000z` будет получать любые сообщения, созданные или измененные после указанной даты и времени.</span><span class="sxs-lookup"><span data-stu-id="c452a-151">For example, `../messages/delta?$filter=lastModifiedDateTime ge 2019-02-27T07:13:28.000z` will fetch any messages created or changed after the specified date time.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c452a-152">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c452a-152">Request headers</span></span>
| <span data-ttu-id="c452a-153">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c452a-153">Header</span></span>        | <span data-ttu-id="c452a-154">Значение</span><span class="sxs-lookup"><span data-stu-id="c452a-154">Value</span></span>                     |
|---------------|---------------------------|
| <span data-ttu-id="c452a-155">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c452a-155">Authorization</span></span> | <span data-ttu-id="c452a-p110">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c452a-p110">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c452a-158">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c452a-158">Content-Type</span></span>  | <span data-ttu-id="c452a-159">application/json</span><span class="sxs-lookup"><span data-stu-id="c452a-159">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="c452a-160">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c452a-160">Request Body</span></span>

<span data-ttu-id="c452a-161">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c452a-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c452a-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="c452a-162">Response</span></span>

<span data-ttu-id="c452a-163">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](https://docs.microsoft.com/ru-RU/graph/api/resources/chatmessage?view=graph-rest-beta) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c452a-163">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](https://docs.microsoft.com/en-us/graph/api/resources/chatmessage?view=graph-rest-beta) objects in the response body.</span></span> <span data-ttu-id="c452a-164">Отклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="c452a-164">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

## <a name="examples"></a><span data-ttu-id="c452a-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="c452a-165">Examples</span></span>

### <a name="example-1-initial-synchronization"></a><span data-ttu-id="c452a-166">Пример 1: Первоначальная синхронизация</span><span class="sxs-lookup"><span data-stu-id="c452a-166">Example 1: Initial synchronization</span></span>

<span data-ttu-id="c452a-167">В приведенном ниже примере показана серия из трех запросов для синхронизации сообщений в заданном канале.</span><span class="sxs-lookup"><span data-stu-id="c452a-167">The following example shows a series of three requests to synchronize the messages in the given channel.</span></span> <span data-ttu-id="c452a-168">В канале пять сообщений.</span><span class="sxs-lookup"><span data-stu-id="c452a-168">There are five messages in the channel.</span></span>

- <span data-ttu-id="c452a-169">Шаг 1. [Пример исходного запроса](#initial-request) и [ответ](#initial-request-response).</span><span class="sxs-lookup"><span data-stu-id="c452a-169">[Step 1: sample initial request](#initial-request) and [response](#initial-request-response)</span></span>
- <span data-ttu-id="c452a-170">Шаг 2. [Пример второго запроса](#second-request) и [ответ](#second-request-response).</span><span class="sxs-lookup"><span data-stu-id="c452a-170">[Step 2: sample second request](#second-request) and [response](#second-request-response)</span></span>
- <span data-ttu-id="c452a-171">Шаг 3. [Пример третьего запроса](#third-request) и [последний ответ](#third-request-response).</span><span class="sxs-lookup"><span data-stu-id="c452a-171">[Step 3: sample third request](#third-request) and [final response](#third-request-response)</span></span>

<span data-ttu-id="c452a-p113">В примерах показаны только некоторые свойства события. При фактическом вызове возвращается большинство свойств события.</span><span class="sxs-lookup"><span data-stu-id="c452a-p113">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span>

<span data-ttu-id="c452a-174">См. также, что можно сделать в [следующем цикле](#example-2-retrieving-additional-changes).</span><span class="sxs-lookup"><span data-stu-id="c452a-174">See also what you'll do in the [next round](#example-2-retrieving-additional-changes).</span></span>

#### <a name="initial-request"></a><span data-ttu-id="c452a-175">Исходный запрос</span><span class="sxs-lookup"><span data-stu-id="c452a-175">Initial request</span></span>

<span data-ttu-id="c452a-176">В этом примере сообщения канала синхронизируются впервые, поэтому исходный запрос на синхронизацию не содержит маркер состояния.</span><span class="sxs-lookup"><span data-stu-id="c452a-176">In this example, the specified folder is being synchronized for the first time, so the initial sync request does not include any state token.</span></span> <span data-ttu-id="c452a-177">В этом цикле возвращаются все события в представлении календаря.</span><span class="sxs-lookup"><span data-stu-id="c452a-177">This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="c452a-178">В запросе указывается необязательный заголовок запроса, odata.top, возвращающий 2 события одновременно.</span><span class="sxs-lookup"><span data-stu-id="c452a-178">The optional request header, odata.maxpagesize, returning 2 events at a time.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c452a-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="c452a-179">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_1"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$top=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c452a-180">C#</span><span class="sxs-lookup"><span data-stu-id="c452a-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c452a-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c452a-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c452a-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c452a-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="initial-request-response"></a><span data-ttu-id="c452a-183">Ответ на исходный запрос</span><span class="sxs-lookup"><span data-stu-id="c452a-183">Initial request and response</span></span>

<span data-ttu-id="c452a-184">Ответ включает два сообщения и заголовок ответа `@odata.nextLink` с маркером `skipToken`.</span><span class="sxs-lookup"><span data-stu-id="c452a-184">The response includes two events and a `@odata.nextLink` response header with a `skipToken`.</span></span> <span data-ttu-id="c452a-185">URL-адрес `nextLink` указывает, что в канале еще остались сообщения.</span><span class="sxs-lookup"><span data-stu-id="c452a-185">The `nextLink` URL indicates there are more messages in the folder to get.</span></span>

><span data-ttu-id="c452a-186">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c452a-186">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c452a-187">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c452a-187">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.nextLink": "/teams('id')/channels('id')/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T07:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T07:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        },
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T08:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T08:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        }
    ]
}
```

#### <a name="second-request"></a><span data-ttu-id="c452a-188">Второй запрос</span><span class="sxs-lookup"><span data-stu-id="c452a-188">Second request</span></span>

<span data-ttu-id="c452a-189">Второй запрос указывает URL-адрес `nextLink`, полученный из предыдущего ответа.</span><span class="sxs-lookup"><span data-stu-id="c452a-189">The second request specifies the `nextLink` URL returned from the previous response.</span></span> <span data-ttu-id="c452a-190">Обратите внимание, что в нем больше не требуется указывать те же основные параметры, что и в исходном запросе, так как маркер `skipToken` в URL-адресе `nextLink` включает их в закодированном виде.</span><span class="sxs-lookup"><span data-stu-id="c452a-190">Notice that it no longer has to specify the same startDateTime and endDateTime parameters as in the initial request, as the  in the  URL encodes and includes them.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c452a-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="c452a-191">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_2"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c452a-192">C#</span><span class="sxs-lookup"><span data-stu-id="c452a-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c452a-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c452a-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c452a-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c452a-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="second-request-response"></a><span data-ttu-id="c452a-195">Ответ на второй запрос</span><span class="sxs-lookup"><span data-stu-id="c452a-195">Second request response</span></span>

<span data-ttu-id="c452a-196">Второй ответ содержит следующие 2 сообщения в папке и заголовок ответа `@odata.nextLink` с `skipToken`, и указывает, что в канале еще остались сообщения.</span><span class="sxs-lookup"><span data-stu-id="c452a-196">The second response returns the next 2 messages and a `@odata.nextLink` response header with a `skipToken`, indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="c452a-197">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c452a-197">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c452a-198">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c452a-198">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.nextLink": "/teams('id')/channels('id')/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T09:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T09:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        },
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T09:50:20.152Z",
            "lastModifiedDateTime": "2019-03-06T09:50:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        }
    ]
}
```

#### <a name="third-request"></a><span data-ttu-id="c452a-199">Третий запрос</span><span class="sxs-lookup"><span data-stu-id="c452a-199">Third sync request</span></span>

<span data-ttu-id="c452a-200">Третий запрос продолжает использовать маркер `nextLink`, полученный из последнего запроса на синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="c452a-200">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c452a-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="c452a-201">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_3"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c452a-202">C#</span><span class="sxs-lookup"><span data-stu-id="c452a-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c452a-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c452a-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c452a-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c452a-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="third-request-response"></a><span data-ttu-id="c452a-205">Ответ на третий запрос</span><span class="sxs-lookup"><span data-stu-id="c452a-205">Third request response</span></span>

<span data-ttu-id="c452a-206">Третий ответ содержит только оставшиеся сообщения в канале и заголовок ответа `@odata.deltaLink` с `deltaToken`, что указывает на то, что все сообщения в канале считаны.</span><span class="sxs-lookup"><span data-stu-id="c452a-206">The third response returns the only remaining messages in the channel and a `@odata.deltaLink` response header with a `deltaToken` which indicates that all messages in the channel have been read.</span></span> <span data-ttu-id="c452a-207">Сохраните и используйте URL-адрес `deltaLink` для запроса любых новых сообщений, начиная с этого момента в следующем цикле.</span><span class="sxs-lookup"><span data-stu-id="c452a-207">Save and use the `deltaLink` URL to query for any new messages starting from this point in the next round.</span></span>

><span data-ttu-id="c452a-208">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c452a-208">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c452a-209">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c452a-209">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.deltaLink": "/teams('id')/channels('id')/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T10:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T10:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        }
    ]
}
```

### <a name="example-2-retrieving-additional-changes"></a><span data-ttu-id="c452a-210">Пример 2. Извлечение дополнительных изменений</span><span class="sxs-lookup"><span data-stu-id="c452a-210">Example 2: Retrieving additional changes</span></span>

<span data-ttu-id="c452a-211">С помощью ссылки `deltaLink` из последнего цикла прошлого запроса вы сможете получить только те сообщения, которые изменились (путем добавления или обновления) в этом канале с момента последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c452a-211">Using the `deltaLink` from the last request in the last round, you will be able to get only those messages that have changed (by being added, deleted, or updated) in that folder since then.</span></span> <span data-ttu-id="c452a-212">При условии, что вы не хотите менять максимальный размер страницы ответа, ваш запрос будет выглядеть следующим образом:</span><span class="sxs-lookup"><span data-stu-id="c452a-212">Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

#### <a name="request"></a><span data-ttu-id="c452a-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="c452a-213">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c452a-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="c452a-214">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_4"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c452a-215">C#</span><span class="sxs-lookup"><span data-stu-id="c452a-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c452a-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c452a-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c452a-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c452a-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c452a-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="c452a-218">Response</span></span>

><span data-ttu-id="c452a-p122">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c452a-p122">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.deltaLink": "/teams('id')/channels('id')/messages/delta?$deltatoken=c3RhcnRUaW1l5Ti1NTEyODc1ODB0OTAyXGFdZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T10:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T10:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Channel messages: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    ]
}
-->
