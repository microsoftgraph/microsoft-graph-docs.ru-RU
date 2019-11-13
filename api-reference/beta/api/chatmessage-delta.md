---
title: 'chatMessages: delta'
description: Получение списка сообщений (без ответов) в канале команды. С помощью разностного запроса можно получить новые или обновленные сообщения в канале.
localization_priority: Priority
doc_type: apiPageType
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: bf4c0fa8333d05ad77397cb4d0bd8ad45e92539a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936799"
---
# <a name="chatmessages-delta"></a><span data-ttu-id="7e876-104">chatMessages: delta</span><span class="sxs-lookup"><span data-stu-id="7e876-104">chatMessages: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e876-105">Получение списка [сообщений](../resources/chatmessage.md) (без ответов) в [канале](../resources/channel.md) [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="7e876-105">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="7e876-106">С помощью разностного запроса можно получить новые или обновленные сообщения в канале.</span><span class="sxs-lookup"><span data-stu-id="7e876-106">By using delta query, you can get new or updated messages in a channel.</span></span>

<span data-ttu-id="7e876-107">Запрос изменений поддерживает как полную синхронизацию с получением всех сообщений в определенном канале, так и добавочную синхронизацию с получением тех сообщений, которые были добавлены или изменены в канале с момента последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="7e876-107">Delta query supports both full synchronization that retrieves all the messages in the specified channel, and incremental synchronization that retrieves those messages that have been added or changed in the channel since the last synchronization.</span></span> <span data-ttu-id="7e876-108">Как правило, сначала выполняется полная синхронизация, а затем в представление календаря периодически добавляются изменения.</span><span class="sxs-lookup"><span data-stu-id="7e876-108">Typically, you would do an initial full synchronization, and then get incremental changes to that calendar view periodically.</span></span>

<span data-ttu-id="7e876-109">Чтобы получить ответы на сообщение, используйте операцию [перечисления ответов на сообщение](channel-get-messagereply.md) или [получения ответа на сообщение](channel-list-messagereplies.md).</span><span class="sxs-lookup"><span data-stu-id="7e876-109">To get the replies for a message, use the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) operation.</span></span>

<span data-ttu-id="7e876-110">Запрос GET с функцией delta возвращает одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="7e876-110">A GET request with the delta function returns either:</span></span>

- <span data-ttu-id="7e876-111">ссылку `nextLink` (содержащую URL-адрес с вызовом функции **delta** и `skipToken`), или</span><span class="sxs-lookup"><span data-stu-id="7e876-111">A `nextLink` (that contains a URL with a **delta** function call and a `skipToken`), or</span></span>
- <span data-ttu-id="7e876-112">ссылку `deltaLink` (содержащую URL-адрес с вызовом функции **delta** и `deltaToken`).</span><span class="sxs-lookup"><span data-stu-id="7e876-112">A `deltaLink` (that contains a URL with a **delta** function call and `deltaToken`).</span></span>

<span data-ttu-id="7e876-113">Маркеры состояния полностью непрозрачны для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e876-113">State tokens are completely opaque to the client.</span></span> <span data-ttu-id="7e876-114">Чтобы продолжить цикл отслеживания изменений, просто скопируйте и примените URL-адрес `nextLink` или `deltaLink`, возвращенный последним запросом GET, при следующем вызове функции delta для этого представления календаря.</span><span class="sxs-lookup"><span data-stu-id="7e876-114">To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next delta function call for that same calendar view.</span></span> <span data-ttu-id="7e876-115">Ссылка `deltaLink` в ответе означает, что текущий цикл отслеживания изменений завершен.</span><span class="sxs-lookup"><span data-stu-id="7e876-115">A `deltaLink` returned in a response signifies that the current round of change tracking is complete.</span></span> <span data-ttu-id="7e876-116">Вы можете сохранить и использовать URL-адрес `deltaLink` в начале следующего цикла.</span><span class="sxs-lookup"><span data-stu-id="7e876-116">You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="7e876-117">Дополнительные сведения см. в документации по [разностному запросу](/graph/delta-query-overview.md).</span><span class="sxs-lookup"><span data-stu-id="7e876-117">For more information, see the [delta query](/graph/delta-query-overview.md) documentation.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e876-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e876-118">Permissions</span></span>

<span data-ttu-id="7e876-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7e876-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="7e876-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e876-121">Permission Type</span></span>                        |<span data-ttu-id="7e876-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e876-122">Permissions (from least to most privileged)</span></span>  |
|---------------------------------------|---------------------------------------------|
|<span data-ttu-id="7e876-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e876-123">Delegated (work or school account)</span></span>     |<span data-ttu-id="7e876-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e876-124">Group.Read.All, Group.ReadWrite.All</span></span>          |
|<span data-ttu-id="7e876-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e876-125">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7e876-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7e876-126">Not Supported</span></span>                                |
|<span data-ttu-id="7e876-127">Приложение</span><span class="sxs-lookup"><span data-stu-id="7e876-127">Application</span></span>                            |<span data-ttu-id="7e876-128">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e876-128">Group.Read.All, Group.ReadWrite.All</span></span>          |

> [!NOTE]
> <span data-ttu-id="7e876-129">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="7e876-129">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="7e876-130">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="7e876-130">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="7e876-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e876-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="7e876-132">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="7e876-132">Query parameters</span></span>

<span data-ttu-id="7e876-133">Отслеживание изменений в сообщениях в канале — это цикл из одного или нескольких вызовов функции **delta**.</span><span class="sxs-lookup"><span data-stu-id="7e876-133">Tracking changes in channel messages incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="7e876-134">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="7e876-134">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="7e876-135">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="7e876-135">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="7e876-136">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="7e876-136">You only need to specify any query parameters once upfront.</span></span>

<span data-ttu-id="7e876-137">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержатся закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="7e876-137">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="7e876-138">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="7e876-138">Query parameter</span></span>      | <span data-ttu-id="7e876-139">Тип</span><span class="sxs-lookup"><span data-stu-id="7e876-139">Type</span></span>   |<span data-ttu-id="7e876-140">Описание</span><span class="sxs-lookup"><span data-stu-id="7e876-140">Description</span></span>|
|:---------------|:--------|:----------|
| `$deltatoken` | <span data-ttu-id="7e876-141">string</span><span class="sxs-lookup"><span data-stu-id="7e876-141">string</span></span> | <span data-ttu-id="7e876-142">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` при предыдущем вызове функции **delta** и указывает на завершение этого цикла отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="7e876-142">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="7e876-143">Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="7e876-143">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| `$skiptoken` | <span data-ttu-id="7e876-144">string</span><span class="sxs-lookup"><span data-stu-id="7e876-144">string</span></span> | <span data-ttu-id="7e876-145">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` при предыдущем вызове функции **delta** и указывает на то, что  остаются не отслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="7e876-145">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked.</span></span> |

### <a name="optional-odata-query-parameters"></a><span data-ttu-id="7e876-146">Необязательные параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="7e876-146">Optional OData query parameters</span></span>

<span data-ttu-id="7e876-147">Этим API поддерживаются указанные ниже [параметры запросов OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7e876-147">The following [OData query parameters](/graph/query-parameters) are supported by this API:</span></span>
- <span data-ttu-id="7e876-148">`$top`, указывает максимальное количество сообщений, которое нужно получить в результате вызова.</span><span class="sxs-lookup"><span data-stu-id="7e876-148">`$top`, represents maximum number of messages to fetch in a call.</span></span> <span data-ttu-id="7e876-149">Верхний предел – **50**.</span><span class="sxs-lookup"><span data-stu-id="7e876-149">The upper limit is **50**.</span></span>
- <span data-ttu-id="7e876-150">`$skip`, указывает, сколько сообщений нужно пропустить в начале списка.</span><span class="sxs-lookup"><span data-stu-id="7e876-150">`$skip`, represents how many messages to skip at the beginning of the list.</span></span>
- <span data-ttu-id="7e876-151">`$filter` поддерживает возврат сообщений, удовлетворяющих определенным условиям.</span><span class="sxs-lookup"><span data-stu-id="7e876-151">`$filter` allows returning messages that meet a certain criteria.</span></span> <span data-ttu-id="7e876-152">Единственное свойство, поддерживающее фильтрацию, — это `lastModifiedDateTime`, при этом поддерживается только оператор **gt**.</span><span class="sxs-lookup"><span data-stu-id="7e876-152">The only property that supports filtering is `lastModifiedDateTime`, and only the **gt** and ge operators are supported.</span></span> <span data-ttu-id="7e876-153">Например, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` будет получать любые сообщения, созданные или измененные после указанной даты и времени.</span><span class="sxs-lookup"><span data-stu-id="7e876-153">For example, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` will fetch any messages created or changed after the specified date time.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e876-154">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e876-154">Request headers</span></span>
| <span data-ttu-id="7e876-155">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e876-155">Header</span></span>        | <span data-ttu-id="7e876-156">Значение</span><span class="sxs-lookup"><span data-stu-id="7e876-156">Value</span></span>                     |
|---------------|---------------------------|
| <span data-ttu-id="7e876-157">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e876-157">Authorization</span></span> | <span data-ttu-id="7e876-p111">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e876-p111">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e876-160">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e876-160">Content-Type</span></span>  | <span data-ttu-id="7e876-161">application/json</span><span class="sxs-lookup"><span data-stu-id="7e876-161">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="7e876-162">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e876-162">Request Body</span></span>

<span data-ttu-id="7e876-163">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e876-163">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e876-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e876-164">Response</span></span>

<span data-ttu-id="7e876-165">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e876-165">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span> <span data-ttu-id="7e876-166">Отклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="7e876-166">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

## <a name="examples"></a><span data-ttu-id="7e876-167">Примеры</span><span class="sxs-lookup"><span data-stu-id="7e876-167">Examples</span></span>

### <a name="example-1-initial-synchronization"></a><span data-ttu-id="7e876-168">Пример 1: Первоначальная синхронизация</span><span class="sxs-lookup"><span data-stu-id="7e876-168">Example 1: Initial synchronization</span></span>

<span data-ttu-id="7e876-169">В приведенном ниже примере показана серия из трех запросов для синхронизации сообщений в заданном канале.</span><span class="sxs-lookup"><span data-stu-id="7e876-169">The following example shows a series of three requests to synchronize the messages in the given channel.</span></span> <span data-ttu-id="7e876-170">В канале пять сообщений.</span><span class="sxs-lookup"><span data-stu-id="7e876-170">There are five messages in the channel.</span></span>

- <span data-ttu-id="7e876-171">Шаг 1. [Пример исходного запроса](#initial-request) и [ответ](#initial-request-response).</span><span class="sxs-lookup"><span data-stu-id="7e876-171">Step 1: [sample initial request](#initial-request) and [response](#initial-request-response).</span></span>
- <span data-ttu-id="7e876-172">Шаг 2. [Пример второго запроса](#second-request) и [ответ](#second-request-response).</span><span class="sxs-lookup"><span data-stu-id="7e876-172">Step 2: [sample second request](#second-request) and [response](#second-request-response)</span></span>
- <span data-ttu-id="7e876-173">Шаг 3. [Пример третьего запроса](#third-request) и [последний ответ](#third-request-response).</span><span class="sxs-lookup"><span data-stu-id="7e876-173">Step 3: [sample third request](#third-request) and [final response](#third-request-response).</span></span>

<span data-ttu-id="7e876-p114">В примерах показаны только некоторые свойства события. При фактическом вызове возвращается большинство свойств события.</span><span class="sxs-lookup"><span data-stu-id="7e876-p114">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span>

<span data-ttu-id="7e876-176">См. также, что можно сделать в [следующем цикле](#example-2-retrieving-additional-changes).</span><span class="sxs-lookup"><span data-stu-id="7e876-176">See also what you'll do in the [next round](#example-2-retrieving-additional-changes).</span></span>

#### <a name="initial-request"></a><span data-ttu-id="7e876-177">Исходный запрос</span><span class="sxs-lookup"><span data-stu-id="7e876-177">Initial request</span></span>

<span data-ttu-id="7e876-178">В этом примере сообщения канала синхронизируются впервые, поэтому исходный запрос на синхронизацию не содержит маркер состояния.</span><span class="sxs-lookup"><span data-stu-id="7e876-178">In this example, the channel messages are being synchronized for the first time, so the initial sync request does not include any state token.</span></span> <span data-ttu-id="7e876-179">В этом цикле возвращаются все события в представлении календаря.</span><span class="sxs-lookup"><span data-stu-id="7e876-179">This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="7e876-180">В запросе указывается необязательный заголовок запроса, odata.top, возвращающий 2 события одновременно.</span><span class="sxs-lookup"><span data-stu-id="7e876-180">The request specifies the optional request header, odata.top, returning 2 events at a time.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7e876-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e876-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_1"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$top=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e876-182">C#</span><span class="sxs-lookup"><span data-stu-id="7e876-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e876-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e876-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e876-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e876-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="initial-request-response"></a><span data-ttu-id="7e876-185">Ответ на исходный запрос</span><span class="sxs-lookup"><span data-stu-id="7e876-185">Initial request response</span></span>

<span data-ttu-id="7e876-186">Ответ включает два сообщения и заголовок ответа `@odata.nextLink` с маркером `skipToken`.</span><span class="sxs-lookup"><span data-stu-id="7e876-186">The response includes two messages and a `@odata.nextLink` response header with a `skipToken`.</span></span> <span data-ttu-id="7e876-187">URL-адрес `nextLink` указывает, что в канале еще остались сообщения.</span><span class="sxs-lookup"><span data-stu-id="7e876-187">The `nextLink` URL indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="7e876-188">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7e876-188">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7e876-189">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e876-189">All the properties will be returned from an actual call.</span></span>
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

#### <a name="second-request"></a><span data-ttu-id="7e876-190">Второй запрос</span><span class="sxs-lookup"><span data-stu-id="7e876-190">Second request</span></span>

<span data-ttu-id="7e876-191">Второй запрос указывает URL-адрес `nextLink`, полученный из предыдущего ответа.</span><span class="sxs-lookup"><span data-stu-id="7e876-191">The second request specifies the `nextLink` URL returned from the previous response.</span></span> <span data-ttu-id="7e876-192">Обратите внимание, что в нем больше не требуется указывать те же основные параметры, что и в исходном запросе, так как маркер `skipToken` в URL-адресе `nextLink` включает их в закодированном виде.</span><span class="sxs-lookup"><span data-stu-id="7e876-192">Notice that it no longer has to specify the same top parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7e876-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e876-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_2"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e876-194">C#</span><span class="sxs-lookup"><span data-stu-id="7e876-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e876-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e876-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e876-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e876-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="second-request-response"></a><span data-ttu-id="7e876-197">Ответ на второй запрос</span><span class="sxs-lookup"><span data-stu-id="7e876-197">Second request response</span></span>

<span data-ttu-id="7e876-198">Второй ответ содержит следующие 2 сообщения в папке и заголовок ответа `@odata.nextLink` с `skipToken`, и указывает, что в канале еще остались сообщения.</span><span class="sxs-lookup"><span data-stu-id="7e876-198">The second response returns the next 2 messages and a `@odata.nextLink` response header with a `skipToken`, indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="7e876-199">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7e876-199">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7e876-200">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e876-200">All the properties will be returned from an actual call.</span></span>
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

#### <a name="third-request"></a><span data-ttu-id="7e876-201">Третий запрос</span><span class="sxs-lookup"><span data-stu-id="7e876-201">Third request</span></span>

<span data-ttu-id="7e876-202">Третий запрос продолжает использовать маркер `nextLink`, полученный из последнего запроса на синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="7e876-202">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7e876-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e876-203">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_3"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e876-204">C#</span><span class="sxs-lookup"><span data-stu-id="7e876-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e876-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e876-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e876-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e876-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="third-request-response"></a><span data-ttu-id="7e876-207">Ответ на третий запрос</span><span class="sxs-lookup"><span data-stu-id="7e876-207">Third request response</span></span>

<span data-ttu-id="7e876-208">Третий ответ содержит только оставшиеся сообщения в канале и заголовок ответа `@odata.deltaLink` с `deltaToken`, что указывает на то, что все сообщения в канале считаны.</span><span class="sxs-lookup"><span data-stu-id="7e876-208">The third response returns the only remaining messages in the channel and a `@odata.deltaLink` response header with a `deltaToken` which indicates that all messages in the channel have been read.</span></span> <span data-ttu-id="7e876-209">Сохраните и используйте URL-адрес `deltaLink` для запроса любых новых сообщений, начиная с этого момента в следующем цикле.</span><span class="sxs-lookup"><span data-stu-id="7e876-209">Save and use the `deltaLink` URL to query for any new messages starting from this point in the next round.</span></span>

><span data-ttu-id="7e876-210">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7e876-210">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7e876-211">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e876-211">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-retrieving-additional-changes"></a><span data-ttu-id="7e876-212">Пример 2. Извлечение дополнительных изменений</span><span class="sxs-lookup"><span data-stu-id="7e876-212">Example 2: Retrieving additional changes</span></span>

<span data-ttu-id="7e876-213">С помощью ссылки `deltaLink` из последнего цикла прошлого запроса вы сможете получить только те сообщения, которые изменились (путем добавления или обновления) в этом канале с момента последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="7e876-213">Using the `deltaLink` from the last request in the last round, you will be able to get only those messages that have changed (by being added, or updated) in that channel since then.</span></span> <span data-ttu-id="7e876-214">При условии, что вы не хотите менять максимальный размер страницы ответа, ваш запрос будет выглядеть следующим образом:</span><span class="sxs-lookup"><span data-stu-id="7e876-214">Your request will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

#### <a name="request"></a><span data-ttu-id="7e876-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e876-215">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7e876-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e876-216">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_4"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e876-217">C#</span><span class="sxs-lookup"><span data-stu-id="7e876-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e876-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e876-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e876-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e876-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7e876-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e876-220">Response</span></span>

><span data-ttu-id="7e876-p123">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e876-p123">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
