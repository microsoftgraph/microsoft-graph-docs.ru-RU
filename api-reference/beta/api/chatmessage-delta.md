---
title: 'chatMessages: delta'
description: Получение списка сообщений (без ответов) в канале команды. С помощью разностного запроса можно получить новые или обновленные сообщения в канале.
localization_priority: Priority
doc_type: apiPageType
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: f04fb42dfc4b85690b0a128ac06d15554f3f4957
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438542"
---
# <a name="chatmessages-delta"></a><span data-ttu-id="93c5a-104">chatMessages: delta</span><span class="sxs-lookup"><span data-stu-id="93c5a-104">chatMessages: delta</span></span>

<span data-ttu-id="93c5a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93c5a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93c5a-106">Получение списка [сообщений](../resources/chatmessage.md) (без ответов) в [канале](../resources/channel.md) [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="93c5a-106">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="93c5a-107">С помощью разностного запроса можно получить новые или обновленные сообщения в канале.</span><span class="sxs-lookup"><span data-stu-id="93c5a-107">By using delta query, you can get new or updated messages in a channel.</span></span>

> <span data-ttu-id="93c5a-108">**Примечание.** Разностный запрос возвращает сообщения только за последние восемь месяцев.</span><span class="sxs-lookup"><span data-stu-id="93c5a-108">**Note:** Delta will only return messages within the last eight months.</span></span> <span data-ttu-id="93c5a-109">Чтобы получить более ранние сообщения, можно воспользоваться методом [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="93c5a-109">You can use [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md) to retrieve older messages.</span></span>

<span data-ttu-id="93c5a-110">Запрос изменений поддерживает как полную синхронизацию с получением всех сообщений в определенном канале, так и добавочную синхронизацию с получением тех сообщений, которые были добавлены или изменены в канале с момента последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="93c5a-110">Delta query supports both full synchronization that retrieves all the messages in the specified channel, and incremental synchronization that retrieves those messages that have been added or changed in the channel since the last synchronization.</span></span> <span data-ttu-id="93c5a-111">Как правило, сначала выполняется полная синхронизация, а затем в представление календаря периодически добавляются изменения.</span><span class="sxs-lookup"><span data-stu-id="93c5a-111">Typically, you would do an initial full synchronization, and then get incremental changes to that calendar view periodically.</span></span>

<span data-ttu-id="93c5a-112">Чтобы получить ответы на сообщение, используйте операцию [перечисления ответов на сообщение](channel-get-messagereply.md) или [получения ответа на сообщение](channel-list-messagereplies.md).</span><span class="sxs-lookup"><span data-stu-id="93c5a-112">To get the replies for a message, use the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) operation.</span></span>

<span data-ttu-id="93c5a-113">Запрос GET с функцией delta возвращает одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="93c5a-113">A GET request with the delta function returns either:</span></span>

- <span data-ttu-id="93c5a-114">ссылку `nextLink` (содержащую URL-адрес с вызовом функции **delta** и `skipToken`), или</span><span class="sxs-lookup"><span data-stu-id="93c5a-114">A `nextLink` (that contains a URL with a **delta** function call and a `skipToken`), or</span></span>
- <span data-ttu-id="93c5a-115">ссылку `deltaLink` (содержащую URL-адрес с вызовом функции **delta** и `deltaToken`).</span><span class="sxs-lookup"><span data-stu-id="93c5a-115">A `deltaLink` (that contains a URL with a **delta** function call and `deltaToken`).</span></span>

<span data-ttu-id="93c5a-116">Маркеры состояния полностью непрозрачны для клиента.</span><span class="sxs-lookup"><span data-stu-id="93c5a-116">State tokens are completely opaque to the client.</span></span> <span data-ttu-id="93c5a-117">Чтобы продолжить цикл отслеживания изменений, просто скопируйте и примените URL-адрес `nextLink` или `deltaLink`, возвращенный последним запросом GET, при следующем вызове функции delta для этого представления календаря.</span><span class="sxs-lookup"><span data-stu-id="93c5a-117">To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next delta function call for that same calendar view.</span></span> <span data-ttu-id="93c5a-118">Ссылка `deltaLink` в ответе означает, что текущий цикл отслеживания изменений завершен.</span><span class="sxs-lookup"><span data-stu-id="93c5a-118">A `deltaLink` returned in a response signifies that the current round of change tracking is complete.</span></span> <span data-ttu-id="93c5a-119">Вы можете сохранить и использовать URL-адрес `deltaLink` в начале следующего цикла.</span><span class="sxs-lookup"><span data-stu-id="93c5a-119">You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="93c5a-120">Дополнительные сведения см. в документации по [разностному запросу](/graph/delta-query-overview.md).</span><span class="sxs-lookup"><span data-stu-id="93c5a-120">For more information, see the [delta query](/graph/delta-query-overview.md) documentation.</span></span>

## <a name="permissions"></a><span data-ttu-id="93c5a-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93c5a-121">Permissions</span></span>

<span data-ttu-id="93c5a-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="93c5a-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="93c5a-124">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93c5a-124">Permission Type</span></span>                        |<span data-ttu-id="93c5a-125">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93c5a-125">Permissions (from least to most privileged)</span></span>  |
|---------------------------------------|---------------------------------------------|
|<span data-ttu-id="93c5a-126">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93c5a-126">Delegated (work or school account)</span></span>     |<span data-ttu-id="93c5a-127">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93c5a-127">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span>          |
|<span data-ttu-id="93c5a-128">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93c5a-128">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="93c5a-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="93c5a-129">Not Supported</span></span>                                |
|<span data-ttu-id="93c5a-130">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93c5a-130">Application</span></span>                            |<span data-ttu-id="93c5a-131">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93c5a-131">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span>          |

> [!NOTE]
> <span data-ttu-id="93c5a-132">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="93c5a-132">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="93c5a-133">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="93c5a-133">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="93c5a-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93c5a-134">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="93c5a-135">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="93c5a-135">Query parameters</span></span>

<span data-ttu-id="93c5a-136">Отслеживание изменений в сообщениях в канале — это цикл из одного или нескольких вызовов функции **delta**.</span><span class="sxs-lookup"><span data-stu-id="93c5a-136">Tracking changes in channel messages incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="93c5a-137">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="93c5a-137">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="93c5a-138">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="93c5a-138">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="93c5a-139">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="93c5a-139">You only need to specify any query parameters once upfront.</span></span>

<span data-ttu-id="93c5a-140">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержатся закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="93c5a-140">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="93c5a-141">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="93c5a-141">Query parameter</span></span>      | <span data-ttu-id="93c5a-142">Тип</span><span class="sxs-lookup"><span data-stu-id="93c5a-142">Type</span></span>   |<span data-ttu-id="93c5a-143">Описание</span><span class="sxs-lookup"><span data-stu-id="93c5a-143">Description</span></span>|
|:---------------|:--------|:----------|
| `$deltatoken` | <span data-ttu-id="93c5a-144">string</span><span class="sxs-lookup"><span data-stu-id="93c5a-144">string</span></span> | <span data-ttu-id="93c5a-145">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` при предыдущем вызове функции **delta** и указывает на завершение этого цикла отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="93c5a-145">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="93c5a-146">Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="93c5a-146">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| `$skiptoken` | <span data-ttu-id="93c5a-147">string</span><span class="sxs-lookup"><span data-stu-id="93c5a-147">string</span></span> | <span data-ttu-id="93c5a-148">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` при предыдущем вызове функции **delta** и указывает на то, что  остаются не отслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="93c5a-148">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked.</span></span> |

### <a name="optional-odata-query-parameters"></a><span data-ttu-id="93c5a-149">Необязательные параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="93c5a-149">Optional OData query parameters</span></span>

<span data-ttu-id="93c5a-150">Этим API поддерживаются указанные ниже [параметры запросов OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="93c5a-150">The following [OData query parameters](/graph/query-parameters) are supported by this API:</span></span>
- <span data-ttu-id="93c5a-151">`$top`, указывает максимальное количество сообщений, которое нужно получить в результате вызова.</span><span class="sxs-lookup"><span data-stu-id="93c5a-151">`$top`, represents maximum number of messages to fetch in a call.</span></span> <span data-ttu-id="93c5a-152">Верхний предел – **50**.</span><span class="sxs-lookup"><span data-stu-id="93c5a-152">The upper limit is **50**.</span></span>
- <span data-ttu-id="93c5a-153">`$skip`, указывает, сколько сообщений нужно пропустить в начале списка.</span><span class="sxs-lookup"><span data-stu-id="93c5a-153">`$skip`, represents how many messages to skip at the beginning of the list.</span></span>
- <span data-ttu-id="93c5a-154">`$filter` поддерживает возврат сообщений, удовлетворяющих определенным условиям.</span><span class="sxs-lookup"><span data-stu-id="93c5a-154">`$filter` allows returning messages that meet a certain criteria.</span></span> <span data-ttu-id="93c5a-155">Единственное свойство, поддерживающее фильтрацию, — это `lastModifiedDateTime`, при этом поддерживается только оператор **gt**.</span><span class="sxs-lookup"><span data-stu-id="93c5a-155">The only property that supports filtering is `lastModifiedDateTime`, and only the **gt** operator is supported.</span></span> <span data-ttu-id="93c5a-156">Например, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` будет получать любые сообщения, созданные или измененные после указанной даты и времени.</span><span class="sxs-lookup"><span data-stu-id="93c5a-156">For example, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` will fetch any messages created or changed after the specified date time.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93c5a-157">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93c5a-157">Request headers</span></span>
| <span data-ttu-id="93c5a-158">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93c5a-158">Header</span></span>        | <span data-ttu-id="93c5a-159">Значение</span><span class="sxs-lookup"><span data-stu-id="93c5a-159">Value</span></span>                     |
|---------------|---------------------------|
| <span data-ttu-id="93c5a-160">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93c5a-160">Authorization</span></span> | <span data-ttu-id="93c5a-p112">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93c5a-p112">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93c5a-163">Content-Type</span><span class="sxs-lookup"><span data-stu-id="93c5a-163">Content-Type</span></span>  | <span data-ttu-id="93c5a-164">application/json</span><span class="sxs-lookup"><span data-stu-id="93c5a-164">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="93c5a-165">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93c5a-165">Request Body</span></span>

<span data-ttu-id="93c5a-166">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93c5a-166">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93c5a-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="93c5a-167">Response</span></span>

<span data-ttu-id="93c5a-168">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93c5a-168">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span> <span data-ttu-id="93c5a-169">Отклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="93c5a-169">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

## <a name="examples"></a><span data-ttu-id="93c5a-170">Примеры</span><span class="sxs-lookup"><span data-stu-id="93c5a-170">Examples</span></span>

### <a name="example-1-initial-synchronization"></a><span data-ttu-id="93c5a-171">Пример 1: Первоначальная синхронизация</span><span class="sxs-lookup"><span data-stu-id="93c5a-171">Example 1: Initial synchronization</span></span>

<span data-ttu-id="93c5a-172">В приведенном ниже примере показана серия из трех запросов для синхронизации сообщений в заданном канале.</span><span class="sxs-lookup"><span data-stu-id="93c5a-172">The following example shows a series of three requests to synchronize the messages in the given channel.</span></span> <span data-ttu-id="93c5a-173">В канале пять сообщений.</span><span class="sxs-lookup"><span data-stu-id="93c5a-173">There are five messages in the channel.</span></span>

- <span data-ttu-id="93c5a-174">Шаг 1. [Пример исходного запроса](#initial-request) и [ответ](#initial-request-response).</span><span class="sxs-lookup"><span data-stu-id="93c5a-174">Step 1: [sample initial request](#initial-request) and [response](#initial-request-response).</span></span>
- <span data-ttu-id="93c5a-175">Шаг 2. [Пример второго запроса](#second-request) и [ответ](#second-request-response).</span><span class="sxs-lookup"><span data-stu-id="93c5a-175">Step 2: [sample second request](#second-request) and [response](#second-request-response)</span></span>
- <span data-ttu-id="93c5a-176">Шаг 3. [Пример третьего запроса](#third-request) и [последний ответ](#third-request-response).</span><span class="sxs-lookup"><span data-stu-id="93c5a-176">Step 3: [sample third request](#third-request) and [final response](#third-request-response).</span></span>

<span data-ttu-id="93c5a-p115">В примерах показаны только некоторые свойства события. При фактическом вызове возвращается большинство свойств события.</span><span class="sxs-lookup"><span data-stu-id="93c5a-p115">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span>

<span data-ttu-id="93c5a-179">См. также, что можно сделать в [следующем цикле](#example-2-retrieving-additional-changes).</span><span class="sxs-lookup"><span data-stu-id="93c5a-179">See also what you'll do in the [next round](#example-2-retrieving-additional-changes).</span></span>

#### <a name="initial-request"></a><span data-ttu-id="93c5a-180">Исходный запрос</span><span class="sxs-lookup"><span data-stu-id="93c5a-180">Initial request</span></span>

<span data-ttu-id="93c5a-181">В этом примере сообщения канала синхронизируются впервые, поэтому исходный запрос на синхронизацию не содержит маркер состояния.</span><span class="sxs-lookup"><span data-stu-id="93c5a-181">In this example, the channel messages are being synchronized for the first time, so the initial sync request does not include any state token.</span></span> <span data-ttu-id="93c5a-182">В этом цикле возвращаются все события в представлении календаря.</span><span class="sxs-lookup"><span data-stu-id="93c5a-182">This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="93c5a-183">В запросе указывается необязательный заголовок запроса, odata.top, возвращающий 2 события одновременно.</span><span class="sxs-lookup"><span data-stu-id="93c5a-183">The request specifies the optional request header, odata.top, returning 2 events at a time.</span></span>


# <a name="http"></a>[<span data-ttu-id="93c5a-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="93c5a-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_1"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$top=2
```
# <a name="c"></a>[<span data-ttu-id="93c5a-185">C#</span><span class="sxs-lookup"><span data-stu-id="93c5a-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93c5a-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93c5a-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93c5a-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93c5a-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="initial-request-response"></a><span data-ttu-id="93c5a-188">Ответ на исходный запрос</span><span class="sxs-lookup"><span data-stu-id="93c5a-188">Initial request response</span></span>

<span data-ttu-id="93c5a-189">Ответ включает два сообщения и заголовок ответа `@odata.nextLink` с маркером `skipToken`.</span><span class="sxs-lookup"><span data-stu-id="93c5a-189">The response includes two messages and a `@odata.nextLink` response header with a `skipToken`.</span></span> <span data-ttu-id="93c5a-190">URL-адрес `nextLink` указывает, что в канале еще остались сообщения.</span><span class="sxs-lookup"><span data-stu-id="93c5a-190">The `nextLink` URL indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="93c5a-191">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="93c5a-191">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="93c5a-192">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93c5a-192">All the properties will be returned from an actual call.</span></span>
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

#### <a name="second-request"></a><span data-ttu-id="93c5a-193">Второй запрос</span><span class="sxs-lookup"><span data-stu-id="93c5a-193">Second request</span></span>

<span data-ttu-id="93c5a-194">Второй запрос указывает URL-адрес `nextLink`, полученный из предыдущего ответа.</span><span class="sxs-lookup"><span data-stu-id="93c5a-194">The second request specifies the `nextLink` URL returned from the previous response.</span></span> <span data-ttu-id="93c5a-195">Обратите внимание, что в нем больше не требуется указывать те же основные параметры, что и в исходном запросе, так как маркер `skipToken` в URL-адресе `nextLink` включает их в закодированном виде.</span><span class="sxs-lookup"><span data-stu-id="93c5a-195">Notice that it no longer has to specify the same top parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>


# <a name="http"></a>[<span data-ttu-id="93c5a-196">HTTP</span><span class="sxs-lookup"><span data-stu-id="93c5a-196">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_2"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="93c5a-197">C#</span><span class="sxs-lookup"><span data-stu-id="93c5a-197">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93c5a-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93c5a-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93c5a-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93c5a-199">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="second-request-response"></a><span data-ttu-id="93c5a-200">Ответ на второй запрос</span><span class="sxs-lookup"><span data-stu-id="93c5a-200">Second request response</span></span>

<span data-ttu-id="93c5a-201">Второй ответ содержит следующие 2 сообщения в папке и заголовок ответа `@odata.nextLink` с `skipToken`, и указывает, что в канале еще остались сообщения.</span><span class="sxs-lookup"><span data-stu-id="93c5a-201">The second response returns the next 2 messages and a `@odata.nextLink` response header with a `skipToken`, indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="93c5a-202">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="93c5a-202">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="93c5a-203">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93c5a-203">All the properties will be returned from an actual call.</span></span>
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

#### <a name="third-request"></a><span data-ttu-id="93c5a-204">Третий запрос</span><span class="sxs-lookup"><span data-stu-id="93c5a-204">Third request</span></span>

<span data-ttu-id="93c5a-205">Третий запрос продолжает использовать маркер `nextLink`, полученный из последнего запроса на синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="93c5a-205">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span>


# <a name="http"></a>[<span data-ttu-id="93c5a-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="93c5a-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_3"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="93c5a-207">C#</span><span class="sxs-lookup"><span data-stu-id="93c5a-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93c5a-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93c5a-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93c5a-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93c5a-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="third-request-response"></a><span data-ttu-id="93c5a-210">Ответ на третий запрос</span><span class="sxs-lookup"><span data-stu-id="93c5a-210">Third request response</span></span>

<span data-ttu-id="93c5a-211">Третий ответ содержит только оставшиеся сообщения в канале и заголовок ответа `@odata.deltaLink` с `deltaToken`, что указывает на то, что все сообщения в канале считаны.</span><span class="sxs-lookup"><span data-stu-id="93c5a-211">The third response returns the only remaining messages in the channel and a `@odata.deltaLink` response header with a `deltaToken` which indicates that all messages in the channel have been read.</span></span> <span data-ttu-id="93c5a-212">Сохраните и используйте URL-адрес `deltaLink` для запроса любых новых сообщений, начиная с этого момента в следующем цикле.</span><span class="sxs-lookup"><span data-stu-id="93c5a-212">Save and use the `deltaLink` URL to query for any new messages starting from this point in the next round.</span></span>

><span data-ttu-id="93c5a-213">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="93c5a-213">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="93c5a-214">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93c5a-214">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-retrieving-additional-changes"></a><span data-ttu-id="93c5a-215">Пример 2. Извлечение дополнительных изменений</span><span class="sxs-lookup"><span data-stu-id="93c5a-215">Example 2: Retrieving additional changes</span></span>

<span data-ttu-id="93c5a-216">С помощью ссылки `deltaLink` из последнего цикла прошлого запроса вы сможете получить только те сообщения, которые изменились (путем добавления или обновления) в этом канале с момента последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="93c5a-216">Using the `deltaLink` from the last request in the last round, you will be able to get only those messages that have changed (by being added, or updated) in that channel since then.</span></span> <span data-ttu-id="93c5a-217">При условии, что вы не хотите менять максимальный размер страницы ответа, ваш запрос будет выглядеть следующим образом:</span><span class="sxs-lookup"><span data-stu-id="93c5a-217">Your request will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

#### <a name="request"></a><span data-ttu-id="93c5a-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="93c5a-218">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="93c5a-219">HTTP</span><span class="sxs-lookup"><span data-stu-id="93c5a-219">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_4"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="93c5a-220">C#</span><span class="sxs-lookup"><span data-stu-id="93c5a-220">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93c5a-221">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93c5a-221">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93c5a-222">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93c5a-222">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="93c5a-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="93c5a-223">Response</span></span>

><span data-ttu-id="93c5a-p124">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93c5a-p124">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
