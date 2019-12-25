---
title: 'chatMessages: delta'
description: Получение списка сообщений (без ответов) в канале команды. С помощью разностного запроса можно получить новые или обновленные сообщения в канале.
localization_priority: Priority
doc_type: apiPageType
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: a843044238a954d0c03136860c4f5289497797b1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868123"
---
# <a name="chatmessages-delta"></a><span data-ttu-id="5b94c-104">chatMessages: delta</span><span class="sxs-lookup"><span data-stu-id="5b94c-104">chatMessages: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b94c-105">Получение списка [сообщений](../resources/chatmessage.md) (без ответов) в [канале](../resources/channel.md) [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="5b94c-105">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="5b94c-106">С помощью разностного запроса можно получить новые или обновленные сообщения в канале.</span><span class="sxs-lookup"><span data-stu-id="5b94c-106">By using delta query, you can get new or updated messages in a channel.</span></span>

> <span data-ttu-id="5b94c-107">**Примечание.** Разностный запрос возвращает сообщения только за последние восемь месяцев.</span><span class="sxs-lookup"><span data-stu-id="5b94c-107">**Note:** Delta will only return messages within the last eight months.</span></span> <span data-ttu-id="5b94c-108">Чтобы получить более ранние сообщения, можно воспользоваться методом [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="5b94c-108">You can use [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md) to retrieve older messages.</span></span>

<span data-ttu-id="5b94c-109">Запрос изменений поддерживает как полную синхронизацию с получением всех сообщений в определенном канале, так и добавочную синхронизацию с получением тех сообщений, которые были добавлены или изменены в канале с момента последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5b94c-109">Delta query supports both full synchronization that retrieves all the messages in the specified channel, and incremental synchronization that retrieves those messages that have been added or changed in the channel since the last synchronization.</span></span> <span data-ttu-id="5b94c-110">Как правило, сначала выполняется полная синхронизация, а затем в представление календаря периодически добавляются изменения.</span><span class="sxs-lookup"><span data-stu-id="5b94c-110">Typically, you would do an initial full synchronization, and then get incremental changes to that calendar view periodically.</span></span>

<span data-ttu-id="5b94c-111">Чтобы получить ответы на сообщение, используйте операцию [перечисления ответов на сообщение](channel-get-messagereply.md) или [получения ответа на сообщение](channel-list-messagereplies.md).</span><span class="sxs-lookup"><span data-stu-id="5b94c-111">To get the replies for a message, use the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) operation.</span></span>

<span data-ttu-id="5b94c-112">Запрос GET с функцией delta возвращает одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="5b94c-112">A GET request with the delta function returns either:</span></span>

- <span data-ttu-id="5b94c-113">ссылку `nextLink` (содержащую URL-адрес с вызовом функции **delta** и `skipToken`), или</span><span class="sxs-lookup"><span data-stu-id="5b94c-113">A `nextLink` (that contains a URL with a **delta** function call and a `skipToken`), or</span></span>
- <span data-ttu-id="5b94c-114">ссылку `deltaLink` (содержащую URL-адрес с вызовом функции **delta** и `deltaToken`).</span><span class="sxs-lookup"><span data-stu-id="5b94c-114">A `deltaLink` (that contains a URL with a **delta** function call and `deltaToken`).</span></span>

<span data-ttu-id="5b94c-115">Маркеры состояния полностью непрозрачны для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b94c-115">State tokens are completely opaque to the client.</span></span> <span data-ttu-id="5b94c-116">Чтобы продолжить цикл отслеживания изменений, просто скопируйте и примените URL-адрес `nextLink` или `deltaLink`, возвращенный последним запросом GET, при следующем вызове функции delta для этого представления календаря.</span><span class="sxs-lookup"><span data-stu-id="5b94c-116">To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next delta function call for that same calendar view.</span></span> <span data-ttu-id="5b94c-117">Ссылка `deltaLink` в ответе означает, что текущий цикл отслеживания изменений завершен.</span><span class="sxs-lookup"><span data-stu-id="5b94c-117">A `deltaLink` returned in a response signifies that the current round of change tracking is complete.</span></span> <span data-ttu-id="5b94c-118">Вы можете сохранить и использовать URL-адрес `deltaLink` в начале следующего цикла.</span><span class="sxs-lookup"><span data-stu-id="5b94c-118">You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="5b94c-119">Дополнительные сведения см. в документации по [разностному запросу](/graph/delta-query-overview.md).</span><span class="sxs-lookup"><span data-stu-id="5b94c-119">For more information, see the [delta query](/graph/delta-query-overview.md) documentation.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b94c-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b94c-120">Permissions</span></span>

<span data-ttu-id="5b94c-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5b94c-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="5b94c-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b94c-123">Permission Type</span></span>                        |<span data-ttu-id="5b94c-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b94c-124">Permissions (from least to most privileged)</span></span>  |
|---------------------------------------|---------------------------------------------|
|<span data-ttu-id="5b94c-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b94c-125">Delegated (work or school account)</span></span>     |<span data-ttu-id="5b94c-126">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b94c-126">Group.Read.All, Group.ReadWrite.All</span></span>          |
|<span data-ttu-id="5b94c-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b94c-127">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="5b94c-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b94c-128">Not Supported</span></span>                                |
|<span data-ttu-id="5b94c-129">Приложение</span><span class="sxs-lookup"><span data-stu-id="5b94c-129">Application</span></span>                            |<span data-ttu-id="5b94c-130">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b94c-130">Group.Read.All, Group.ReadWrite.All</span></span>          |

> [!NOTE]
> <span data-ttu-id="5b94c-131">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="5b94c-131">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="5b94c-132">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="5b94c-132">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="5b94c-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b94c-133">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="5b94c-134">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="5b94c-134">Query parameters</span></span>

<span data-ttu-id="5b94c-135">Отслеживание изменений в сообщениях в канале — это цикл из одного или нескольких вызовов функции **delta**.</span><span class="sxs-lookup"><span data-stu-id="5b94c-135">Tracking changes in channel messages incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="5b94c-136">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="5b94c-136">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="5b94c-137">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="5b94c-137">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="5b94c-138">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="5b94c-138">You only need to specify any query parameters once upfront.</span></span>

<span data-ttu-id="5b94c-139">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержатся закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="5b94c-139">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="5b94c-140">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="5b94c-140">Query parameter</span></span>      | <span data-ttu-id="5b94c-141">Тип</span><span class="sxs-lookup"><span data-stu-id="5b94c-141">Type</span></span>   |<span data-ttu-id="5b94c-142">Описание</span><span class="sxs-lookup"><span data-stu-id="5b94c-142">Description</span></span>|
|:---------------|:--------|:----------|
| `$deltatoken` | <span data-ttu-id="5b94c-143">string</span><span class="sxs-lookup"><span data-stu-id="5b94c-143">string</span></span> | <span data-ttu-id="5b94c-144">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` при предыдущем вызове функции **delta** и указывает на завершение этого цикла отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="5b94c-144">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="5b94c-145">Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="5b94c-145">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| `$skiptoken` | <span data-ttu-id="5b94c-146">string</span><span class="sxs-lookup"><span data-stu-id="5b94c-146">string</span></span> | <span data-ttu-id="5b94c-147">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` при предыдущем вызове функции **delta** и указывает на то, что  остаются не отслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="5b94c-147">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked.</span></span> |

### <a name="optional-odata-query-parameters"></a><span data-ttu-id="5b94c-148">Необязательные параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="5b94c-148">Optional OData query parameters</span></span>

<span data-ttu-id="5b94c-149">Этим API поддерживаются указанные ниже [параметры запросов OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5b94c-149">The following [OData query parameters](/graph/query-parameters) are supported by this API:</span></span>
- <span data-ttu-id="5b94c-150">`$top`, указывает максимальное количество сообщений, которое нужно получить в результате вызова.</span><span class="sxs-lookup"><span data-stu-id="5b94c-150">`$top`, represents maximum number of messages to fetch in a call.</span></span> <span data-ttu-id="5b94c-151">Верхний предел – **50**.</span><span class="sxs-lookup"><span data-stu-id="5b94c-151">The upper limit is **50**.</span></span>
- <span data-ttu-id="5b94c-152">`$skip`, указывает, сколько сообщений нужно пропустить в начале списка.</span><span class="sxs-lookup"><span data-stu-id="5b94c-152">`$skip`, represents how many messages to skip at the beginning of the list.</span></span>
- <span data-ttu-id="5b94c-153">`$filter` поддерживает возврат сообщений, удовлетворяющих определенным условиям.</span><span class="sxs-lookup"><span data-stu-id="5b94c-153">`$filter` allows returning messages that meet a certain criteria.</span></span> <span data-ttu-id="5b94c-154">Единственное свойство, поддерживающее фильтрацию, — это `lastModifiedDateTime`, при этом поддерживается только оператор **gt**.</span><span class="sxs-lookup"><span data-stu-id="5b94c-154">The only property that supports filtering is `lastModifiedDateTime`, and only the **gt** operator is supported.</span></span> <span data-ttu-id="5b94c-155">Например, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` будет получать любые сообщения, созданные или измененные после указанной даты и времени.</span><span class="sxs-lookup"><span data-stu-id="5b94c-155">For example, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` will fetch any messages created or changed after the specified date time.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b94c-156">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b94c-156">Request headers</span></span>
| <span data-ttu-id="5b94c-157">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b94c-157">Header</span></span>        | <span data-ttu-id="5b94c-158">Значение</span><span class="sxs-lookup"><span data-stu-id="5b94c-158">Value</span></span>                     |
|---------------|---------------------------|
| <span data-ttu-id="5b94c-159">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b94c-159">Authorization</span></span> | <span data-ttu-id="5b94c-p112">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b94c-p112">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b94c-162">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b94c-162">Content-Type</span></span>  | <span data-ttu-id="5b94c-163">application/json</span><span class="sxs-lookup"><span data-stu-id="5b94c-163">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="5b94c-164">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b94c-164">Request Body</span></span>

<span data-ttu-id="5b94c-165">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b94c-165">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b94c-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b94c-166">Response</span></span>

<span data-ttu-id="5b94c-167">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b94c-167">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span> <span data-ttu-id="5b94c-168">Отклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="5b94c-168">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

## <a name="examples"></a><span data-ttu-id="5b94c-169">Примеры</span><span class="sxs-lookup"><span data-stu-id="5b94c-169">Examples</span></span>

### <a name="example-1-initial-synchronization"></a><span data-ttu-id="5b94c-170">Пример 1: Первоначальная синхронизация</span><span class="sxs-lookup"><span data-stu-id="5b94c-170">Example 1: Initial synchronization</span></span>

<span data-ttu-id="5b94c-171">В приведенном ниже примере показана серия из трех запросов для синхронизации сообщений в заданном канале.</span><span class="sxs-lookup"><span data-stu-id="5b94c-171">The following example shows a series of three requests to synchronize the messages in the given channel.</span></span> <span data-ttu-id="5b94c-172">В канале пять сообщений.</span><span class="sxs-lookup"><span data-stu-id="5b94c-172">There are five messages in the channel.</span></span>

- <span data-ttu-id="5b94c-173">Шаг 1. [Пример исходного запроса](#initial-request) и [ответ](#initial-request-response).</span><span class="sxs-lookup"><span data-stu-id="5b94c-173">Step 1: [sample initial request](#initial-request) and [response](#initial-request-response).</span></span>
- <span data-ttu-id="5b94c-174">Шаг 2. [Пример второго запроса](#second-request) и [ответ](#second-request-response).</span><span class="sxs-lookup"><span data-stu-id="5b94c-174">Step 2: [sample second request](#second-request) and [response](#second-request-response)</span></span>
- <span data-ttu-id="5b94c-175">Шаг 3. [Пример третьего запроса](#third-request) и [последний ответ](#third-request-response).</span><span class="sxs-lookup"><span data-stu-id="5b94c-175">Step 3: [sample third request](#third-request) and [final response](#third-request-response).</span></span>

<span data-ttu-id="5b94c-p115">В примерах показаны только некоторые свойства события. При фактическом вызове возвращается большинство свойств события.</span><span class="sxs-lookup"><span data-stu-id="5b94c-p115">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span>

<span data-ttu-id="5b94c-178">См. также, что можно сделать в [следующем цикле](#example-2-retrieving-additional-changes).</span><span class="sxs-lookup"><span data-stu-id="5b94c-178">See also what you'll do in the [next round](#example-2-retrieving-additional-changes).</span></span>

#### <a name="initial-request"></a><span data-ttu-id="5b94c-179">Исходный запрос</span><span class="sxs-lookup"><span data-stu-id="5b94c-179">Initial request</span></span>

<span data-ttu-id="5b94c-180">В этом примере сообщения канала синхронизируются впервые, поэтому исходный запрос на синхронизацию не содержит маркер состояния.</span><span class="sxs-lookup"><span data-stu-id="5b94c-180">In this example, the channel messages are being synchronized for the first time, so the initial sync request does not include any state token.</span></span> <span data-ttu-id="5b94c-181">В этом цикле возвращаются все события в представлении календаря.</span><span class="sxs-lookup"><span data-stu-id="5b94c-181">This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="5b94c-182">В запросе указывается необязательный заголовок запроса, odata.top, возвращающий 2 события одновременно.</span><span class="sxs-lookup"><span data-stu-id="5b94c-182">The request specifies the optional request header, odata.top, returning 2 events at a time.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5b94c-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b94c-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_1"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$top=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5b94c-184">C#</span><span class="sxs-lookup"><span data-stu-id="5b94c-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b94c-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b94c-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5b94c-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b94c-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="initial-request-response"></a><span data-ttu-id="5b94c-187">Ответ на исходный запрос</span><span class="sxs-lookup"><span data-stu-id="5b94c-187">Initial request response</span></span>

<span data-ttu-id="5b94c-188">Ответ включает два сообщения и заголовок ответа `@odata.nextLink` с маркером `skipToken`.</span><span class="sxs-lookup"><span data-stu-id="5b94c-188">The response includes two messages and a `@odata.nextLink` response header with a `skipToken`.</span></span> <span data-ttu-id="5b94c-189">URL-адрес `nextLink` указывает, что в канале еще остались сообщения.</span><span class="sxs-lookup"><span data-stu-id="5b94c-189">The `nextLink` URL indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="5b94c-190">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5b94c-190">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5b94c-191">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b94c-191">All the properties will be returned from an actual call.</span></span>
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

#### <a name="second-request"></a><span data-ttu-id="5b94c-192">Второй запрос</span><span class="sxs-lookup"><span data-stu-id="5b94c-192">Second request</span></span>

<span data-ttu-id="5b94c-193">Второй запрос указывает URL-адрес `nextLink`, полученный из предыдущего ответа.</span><span class="sxs-lookup"><span data-stu-id="5b94c-193">The second request specifies the `nextLink` URL returned from the previous response.</span></span> <span data-ttu-id="5b94c-194">Обратите внимание, что в нем больше не требуется указывать те же основные параметры, что и в исходном запросе, так как маркер `skipToken` в URL-адресе `nextLink` включает их в закодированном виде.</span><span class="sxs-lookup"><span data-stu-id="5b94c-194">Notice that it no longer has to specify the same top parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5b94c-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b94c-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_2"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5b94c-196">C#</span><span class="sxs-lookup"><span data-stu-id="5b94c-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b94c-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b94c-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5b94c-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b94c-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="second-request-response"></a><span data-ttu-id="5b94c-199">Ответ на второй запрос</span><span class="sxs-lookup"><span data-stu-id="5b94c-199">Second request response</span></span>

<span data-ttu-id="5b94c-200">Второй ответ содержит следующие 2 сообщения в папке и заголовок ответа `@odata.nextLink` с `skipToken`, и указывает, что в канале еще остались сообщения.</span><span class="sxs-lookup"><span data-stu-id="5b94c-200">The second response returns the next 2 messages and a `@odata.nextLink` response header with a `skipToken`, indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="5b94c-201">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5b94c-201">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5b94c-202">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b94c-202">All the properties will be returned from an actual call.</span></span>
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

#### <a name="third-request"></a><span data-ttu-id="5b94c-203">Третий запрос</span><span class="sxs-lookup"><span data-stu-id="5b94c-203">Third request</span></span>

<span data-ttu-id="5b94c-204">Третий запрос продолжает использовать маркер `nextLink`, полученный из последнего запроса на синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="5b94c-204">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5b94c-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b94c-205">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_3"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5b94c-206">C#</span><span class="sxs-lookup"><span data-stu-id="5b94c-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b94c-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b94c-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5b94c-208">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b94c-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="third-request-response"></a><span data-ttu-id="5b94c-209">Ответ на третий запрос</span><span class="sxs-lookup"><span data-stu-id="5b94c-209">Third request response</span></span>

<span data-ttu-id="5b94c-210">Третий ответ содержит только оставшиеся сообщения в канале и заголовок ответа `@odata.deltaLink` с `deltaToken`, что указывает на то, что все сообщения в канале считаны.</span><span class="sxs-lookup"><span data-stu-id="5b94c-210">The third response returns the only remaining messages in the channel and a `@odata.deltaLink` response header with a `deltaToken` which indicates that all messages in the channel have been read.</span></span> <span data-ttu-id="5b94c-211">Сохраните и используйте URL-адрес `deltaLink` для запроса любых новых сообщений, начиная с этого момента в следующем цикле.</span><span class="sxs-lookup"><span data-stu-id="5b94c-211">Save and use the `deltaLink` URL to query for any new messages starting from this point in the next round.</span></span>

><span data-ttu-id="5b94c-212">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5b94c-212">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5b94c-213">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b94c-213">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-retrieving-additional-changes"></a><span data-ttu-id="5b94c-214">Пример 2. Извлечение дополнительных изменений</span><span class="sxs-lookup"><span data-stu-id="5b94c-214">Example 2: Retrieving additional changes</span></span>

<span data-ttu-id="5b94c-215">С помощью ссылки `deltaLink` из последнего цикла прошлого запроса вы сможете получить только те сообщения, которые изменились (путем добавления или обновления) в этом канале с момента последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5b94c-215">Using the `deltaLink` from the last request in the last round, you will be able to get only those messages that have changed (by being added, or updated) in that channel since then.</span></span> <span data-ttu-id="5b94c-216">При условии, что вы не хотите менять максимальный размер страницы ответа, ваш запрос будет выглядеть следующим образом:</span><span class="sxs-lookup"><span data-stu-id="5b94c-216">Your request will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

#### <a name="request"></a><span data-ttu-id="5b94c-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b94c-217">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5b94c-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b94c-218">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_4"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5b94c-219">C#</span><span class="sxs-lookup"><span data-stu-id="5b94c-219">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b94c-220">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b94c-220">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5b94c-221">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b94c-221">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5b94c-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b94c-222">Response</span></span>

><span data-ttu-id="5b94c-p124">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b94c-p124">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
