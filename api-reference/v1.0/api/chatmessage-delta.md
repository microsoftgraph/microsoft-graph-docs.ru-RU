---
title: 'chatMessages: delta'
description: Получение списка сообщений (без ответов) в канале команды. С помощью разностного запроса можно получить новые или обновленные сообщения в канале.
localization_priority: Priority
doc_type: apiPageType
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: c1282d71fbd0ae51f4ce1a24549ca2721c77a260
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515662"
---
# <a name="chatmessages-delta"></a><span data-ttu-id="52f61-104">chatMessages: delta</span><span class="sxs-lookup"><span data-stu-id="52f61-104">chatMessages: delta</span></span>

<span data-ttu-id="52f61-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52f61-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="52f61-106">Получение списка [сообщений](../resources/chatmessage.md) (без ответов) в [канале](../resources/channel.md) [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="52f61-106">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="52f61-107">С помощью разностного запроса можно получить новые или обновленные сообщения в канале.</span><span class="sxs-lookup"><span data-stu-id="52f61-107">By using delta query, you can get new or updated messages in a channel.</span></span>

> <span data-ttu-id="52f61-108">**Примечание.** Разностный запрос возвращает сообщения только за последние восемь месяцев.</span><span class="sxs-lookup"><span data-stu-id="52f61-108">**Note:** Delta will only return messages within the last eight months.</span></span> <span data-ttu-id="52f61-109">Чтобы получить более ранние сообщения, можно воспользоваться методом [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="52f61-109">You can use [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md) to retrieve older messages.</span></span>

<span data-ttu-id="52f61-110">Запрос изменений поддерживает как полную синхронизацию с получением всех сообщений в определенном канале, так и добавочную синхронизацию с получением тех сообщений, которые были добавлены или изменены в канале с момента последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="52f61-110">Delta query supports both full synchronization that retrieves all the messages in the specified channel, and incremental synchronization that retrieves those messages that have been added or changed in the channel since the last synchronization.</span></span> <span data-ttu-id="52f61-111">Как правило, сначала выполняется полная синхронизация, а затем в представление календаря периодически добавляются изменения.</span><span class="sxs-lookup"><span data-stu-id="52f61-111">Typically, you would do an initial full synchronization, and then get incremental changes to that calendar view periodically.</span></span>

<span data-ttu-id="52f61-112">Чтобы получить ответы на сообщение, используйте операцию [перечисления ответов на сообщение](channel-get-messagereply.md) или [получения ответа на сообщение](channel-list-messagereplies.md).</span><span class="sxs-lookup"><span data-stu-id="52f61-112">To get the replies for a message, use the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) operation.</span></span>

<span data-ttu-id="52f61-113">Запрос GET с функцией delta возвращает одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="52f61-113">A GET request with the delta function returns either:</span></span>

- <span data-ttu-id="52f61-114">ссылку `nextLink` (содержащую URL-адрес с вызовом функции **delta** и `skipToken`), или</span><span class="sxs-lookup"><span data-stu-id="52f61-114">A `nextLink` (that contains a URL with a **delta** function call and a `skipToken`), or</span></span>
- <span data-ttu-id="52f61-115">ссылку `deltaLink` (содержащую URL-адрес с вызовом функции **delta** и `deltaToken`).</span><span class="sxs-lookup"><span data-stu-id="52f61-115">A `deltaLink` (that contains a URL with a **delta** function call and `deltaToken`).</span></span>

<span data-ttu-id="52f61-116">Маркеры состояния полностью непрозрачны для клиента.</span><span class="sxs-lookup"><span data-stu-id="52f61-116">State tokens are completely opaque to the client.</span></span> <span data-ttu-id="52f61-117">Чтобы продолжить цикл отслеживания изменений, просто скопируйте и примените URL-адрес `nextLink` или `deltaLink`, возвращенный последним запросом GET, при следующем вызове функции delta для этого представления календаря.</span><span class="sxs-lookup"><span data-stu-id="52f61-117">To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next delta function call for that same calendar view.</span></span> <span data-ttu-id="52f61-118">Ссылка `deltaLink` в ответе означает, что текущий цикл отслеживания изменений завершен.</span><span class="sxs-lookup"><span data-stu-id="52f61-118">A `deltaLink` returned in a response signifies that the current round of change tracking is complete.</span></span> <span data-ttu-id="52f61-119">Вы можете сохранить и использовать URL-адрес `deltaLink` в начале следующего цикла.</span><span class="sxs-lookup"><span data-stu-id="52f61-119">You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="52f61-120">Дополнительные сведения см. в документации по [разностному запросу](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="52f61-120">For more information, see the [delta query](/graph/delta-query-overview) documentation.</span></span>

## <a name="permissions"></a><span data-ttu-id="52f61-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52f61-121">Permissions</span></span>

<span data-ttu-id="52f61-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="52f61-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="52f61-124">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52f61-124">Permission Type</span></span>                        |<span data-ttu-id="52f61-125">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52f61-125">Permissions (from least to most privileged)</span></span>  |
|---------------------------------------|---------------------------------------------|
|<span data-ttu-id="52f61-126">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52f61-126">Delegated (work or school account)</span></span>| <span data-ttu-id="52f61-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="52f61-127">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="52f61-128">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52f61-128">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52f61-129">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52f61-129">Not supported.</span></span>|
|<span data-ttu-id="52f61-130">Приложение</span><span class="sxs-lookup"><span data-stu-id="52f61-130">Application</span></span>| <span data-ttu-id="52f61-131">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="52f61-131">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span> |

> <span data-ttu-id="52f61-132">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="52f61-132">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="52f61-133">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="52f61-133">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="52f61-134">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="52f61-134">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="52f61-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52f61-135">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="52f61-136">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="52f61-136">Query parameters</span></span>

<span data-ttu-id="52f61-137">Отслеживание изменений в сообщениях в канале — это цикл из одного или нескольких вызовов функции **delta**.</span><span class="sxs-lookup"><span data-stu-id="52f61-137">Tracking changes in channel messages incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="52f61-138">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="52f61-138">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="52f61-139">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="52f61-139">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="52f61-140">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="52f61-140">You only need to specify any query parameters once upfront.</span></span>

<span data-ttu-id="52f61-141">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержатся закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="52f61-141">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="52f61-142">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="52f61-142">Query parameter</span></span>      | <span data-ttu-id="52f61-143">Тип</span><span class="sxs-lookup"><span data-stu-id="52f61-143">Type</span></span>   |<span data-ttu-id="52f61-144">Описание</span><span class="sxs-lookup"><span data-stu-id="52f61-144">Description</span></span>|
|:---------------|:--------|:----------|
| `$deltatoken` | <span data-ttu-id="52f61-145">string</span><span class="sxs-lookup"><span data-stu-id="52f61-145">string</span></span> | <span data-ttu-id="52f61-146">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` при предыдущем вызове функции **delta** и указывает на завершение этого цикла отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="52f61-146">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="52f61-147">Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="52f61-147">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| `$skiptoken` | <span data-ttu-id="52f61-148">string</span><span class="sxs-lookup"><span data-stu-id="52f61-148">string</span></span> | <span data-ttu-id="52f61-149">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` при предыдущем вызове функции **delta** и указывает на то, что  остаются не отслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="52f61-149">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked.</span></span> |

### <a name="optional-odata-query-parameters"></a><span data-ttu-id="52f61-150">Необязательные параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="52f61-150">Optional OData query parameters</span></span>

<span data-ttu-id="52f61-151">Этим API поддерживаются указанные ниже [параметры запросов OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="52f61-151">The following [OData query parameters](/graph/query-parameters) are supported by this API:</span></span>
- <span data-ttu-id="52f61-152">`$top`, указывает максимальное количество сообщений, которое нужно получить в результате вызова.</span><span class="sxs-lookup"><span data-stu-id="52f61-152">`$top`, represents maximum number of messages to fetch in a call.</span></span> <span data-ttu-id="52f61-153">Верхний предел – **50**.</span><span class="sxs-lookup"><span data-stu-id="52f61-153">The upper limit is **50**.</span></span>
- <span data-ttu-id="52f61-154">`$skip`, указывает, сколько сообщений нужно пропустить в начале списка.</span><span class="sxs-lookup"><span data-stu-id="52f61-154">`$skip`, represents how many messages to skip at the beginning of the list.</span></span>
- <span data-ttu-id="52f61-155">`$filter` поддерживает возврат сообщений, удовлетворяющих определенным условиям.</span><span class="sxs-lookup"><span data-stu-id="52f61-155">`$filter` allows returning messages that meet a certain criteria.</span></span> <span data-ttu-id="52f61-156">Единственное свойство, поддерживающее фильтрацию, — это `lastModifiedDateTime`, при этом поддерживается только оператор **gt**.</span><span class="sxs-lookup"><span data-stu-id="52f61-156">The only property that supports filtering is `lastModifiedDateTime`, and only the **gt** operator is supported.</span></span> <span data-ttu-id="52f61-157">Например, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` будет получать любые сообщения, созданные или измененные после указанной даты и времени.</span><span class="sxs-lookup"><span data-stu-id="52f61-157">For example, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` will fetch any messages created or changed after the specified date time.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52f61-158">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52f61-158">Request headers</span></span>
| <span data-ttu-id="52f61-159">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52f61-159">Header</span></span>        | <span data-ttu-id="52f61-160">Значение</span><span class="sxs-lookup"><span data-stu-id="52f61-160">Value</span></span>                     |
|---------------|---------------------------|
| <span data-ttu-id="52f61-161">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52f61-161">Authorization</span></span> | <span data-ttu-id="52f61-p112">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52f61-p112">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52f61-164">Content-Type</span><span class="sxs-lookup"><span data-stu-id="52f61-164">Content-Type</span></span>  | <span data-ttu-id="52f61-165">application/json</span><span class="sxs-lookup"><span data-stu-id="52f61-165">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="52f61-166">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52f61-166">Request Body</span></span>

<span data-ttu-id="52f61-167">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52f61-167">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52f61-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="52f61-168">Response</span></span>

<span data-ttu-id="52f61-169">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52f61-169">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span> <span data-ttu-id="52f61-170">Отклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="52f61-170">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

## <a name="examples"></a><span data-ttu-id="52f61-171">Примеры</span><span class="sxs-lookup"><span data-stu-id="52f61-171">Examples</span></span>

### <a name="example-1-initial-synchronization"></a><span data-ttu-id="52f61-172">Пример 1: Первоначальная синхронизация</span><span class="sxs-lookup"><span data-stu-id="52f61-172">Example 1: Initial synchronization</span></span>

<span data-ttu-id="52f61-173">В приведенном ниже примере показана серия из трех запросов для синхронизации сообщений в заданном канале.</span><span class="sxs-lookup"><span data-stu-id="52f61-173">The following example shows a series of three requests to synchronize the messages in the given channel.</span></span> <span data-ttu-id="52f61-174">В канале пять сообщений.</span><span class="sxs-lookup"><span data-stu-id="52f61-174">There are five messages in the channel.</span></span>

- <span data-ttu-id="52f61-175">Шаг 1. [Пример исходного запроса](#initial-request) и [ответ](#initial-request-response).</span><span class="sxs-lookup"><span data-stu-id="52f61-175">Step 1: [sample initial request](#initial-request) and [response](#initial-request-response).</span></span>
- <span data-ttu-id="52f61-176">Шаг 2. [Пример второго запроса](#second-request) и [ответ](#second-request-response).</span><span class="sxs-lookup"><span data-stu-id="52f61-176">Step 2: [sample second request](#second-request) and [response](#second-request-response)</span></span>
- <span data-ttu-id="52f61-177">Шаг 3. [Пример третьего запроса](#third-request) и [последний ответ](#third-request-response).</span><span class="sxs-lookup"><span data-stu-id="52f61-177">Step 3: [sample third request](#third-request) and [final response](#third-request-response).</span></span>

<span data-ttu-id="52f61-p115">В примерах показаны только некоторые свойства события. При фактическом вызове возвращается большинство свойств события.</span><span class="sxs-lookup"><span data-stu-id="52f61-p115">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span>

<span data-ttu-id="52f61-180">См. также, что можно сделать в [следующем цикле](#example-2-retrieving-additional-changes).</span><span class="sxs-lookup"><span data-stu-id="52f61-180">See also what you'll do in the [next round](#example-2-retrieving-additional-changes).</span></span>

#### <a name="initial-request"></a><span data-ttu-id="52f61-181">Исходный запрос</span><span class="sxs-lookup"><span data-stu-id="52f61-181">Initial request</span></span>

<span data-ttu-id="52f61-182">В этом примере сообщения канала синхронизируются впервые, поэтому исходный запрос на синхронизацию не содержит маркер состояния.</span><span class="sxs-lookup"><span data-stu-id="52f61-182">In this example, the channel messages are being synchronized for the first time, so the initial sync request does not include any state token.</span></span> <span data-ttu-id="52f61-183">В этом цикле возвращаются все события в представлении календаря.</span><span class="sxs-lookup"><span data-stu-id="52f61-183">This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="52f61-184">В запросе указывается необязательный заголовок запроса, odata.top, возвращающий 2 события одновременно.</span><span class="sxs-lookup"><span data-stu-id="52f61-184">The request specifies the optional request header, odata.top, returning 2 events at a time.</span></span>



# <a name="http"></a>[<span data-ttu-id="52f61-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="52f61-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_1"
}-->
```msgraph-interactive
GET /teams/{id}/channels/{id}/messages/delta?$top=2
```
# <a name="c"></a>[<span data-ttu-id="52f61-186">C#</span><span class="sxs-lookup"><span data-stu-id="52f61-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52f61-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52f61-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52f61-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52f61-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52f61-189">Java</span><span class="sxs-lookup"><span data-stu-id="52f61-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="initial-request-response"></a><span data-ttu-id="52f61-190">Ответ на исходный запрос</span><span class="sxs-lookup"><span data-stu-id="52f61-190">Initial request response</span></span>

<span data-ttu-id="52f61-191">Ответ включает два сообщения и заголовок ответа `@odata.nextLink` с маркером `skipToken`.</span><span class="sxs-lookup"><span data-stu-id="52f61-191">The response includes two messages and a `@odata.nextLink` response header with a `skipToken`.</span></span> <span data-ttu-id="52f61-192">URL-адрес `nextLink` указывает, что в канале еще остались сообщения.</span><span class="sxs-lookup"><span data-stu-id="52f61-192">The `nextLink` URL indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="52f61-193">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="52f61-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="52f61-194">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52f61-194">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.nextLink": "/teams('id')/channels('id')/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from": {
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
            "from": {
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

#### <a name="second-request"></a><span data-ttu-id="52f61-195">Второй запрос</span><span class="sxs-lookup"><span data-stu-id="52f61-195">Second request</span></span>

<span data-ttu-id="52f61-196">Второй запрос указывает URL-адрес `nextLink`, полученный из предыдущего ответа.</span><span class="sxs-lookup"><span data-stu-id="52f61-196">The second request specifies the `nextLink` URL returned from the previous response.</span></span> <span data-ttu-id="52f61-197">Обратите внимание, что в нем больше не требуется указывать те же основные параметры, что и в исходном запросе, так как маркер `skipToken` в URL-адресе `nextLink` включает их в закодированном виде.</span><span class="sxs-lookup"><span data-stu-id="52f61-197">Notice that it no longer has to specify the same top parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>


# <a name="http"></a>[<span data-ttu-id="52f61-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="52f61-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_2"
}-->
```msgraph-interactive
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="52f61-199">C#</span><span class="sxs-lookup"><span data-stu-id="52f61-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52f61-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52f61-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52f61-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52f61-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52f61-202">Java</span><span class="sxs-lookup"><span data-stu-id="52f61-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="second-request-response"></a><span data-ttu-id="52f61-203">Ответ на второй запрос</span><span class="sxs-lookup"><span data-stu-id="52f61-203">Second request response</span></span>

<span data-ttu-id="52f61-204">Второй ответ содержит следующие 2 сообщения в папке и заголовок ответа `@odata.nextLink` с `skipToken`, и указывает, что в канале еще остались сообщения.</span><span class="sxs-lookup"><span data-stu-id="52f61-204">The second response returns the next 2 messages and a `@odata.nextLink` response header with a `skipToken`, indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="52f61-205">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="52f61-205">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="52f61-206">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52f61-206">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.nextLink": "/teams('id')/channels('id')/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from": {
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
            "from": {
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

#### <a name="third-request"></a><span data-ttu-id="52f61-207">Третий запрос</span><span class="sxs-lookup"><span data-stu-id="52f61-207">Third request</span></span>

<span data-ttu-id="52f61-208">Третий запрос продолжает использовать маркер `nextLink`, полученный из последнего запроса на синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="52f61-208">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span>



# <a name="http"></a>[<span data-ttu-id="52f61-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="52f61-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_3"
}-->
```msgraph-interactive
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="52f61-210">C#</span><span class="sxs-lookup"><span data-stu-id="52f61-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52f61-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52f61-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52f61-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52f61-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52f61-213">Java</span><span class="sxs-lookup"><span data-stu-id="52f61-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="third-request-response"></a><span data-ttu-id="52f61-214">Ответ на третий запрос</span><span class="sxs-lookup"><span data-stu-id="52f61-214">Third request response</span></span>

<span data-ttu-id="52f61-215">Третий ответ содержит только оставшиеся сообщения в канале и заголовок ответа `@odata.deltaLink` с `deltaToken`, что указывает на то, что все сообщения в канале считаны.</span><span class="sxs-lookup"><span data-stu-id="52f61-215">The third response returns the only remaining messages in the channel and a `@odata.deltaLink` response header with a `deltaToken` which indicates that all messages in the channel have been read.</span></span> <span data-ttu-id="52f61-216">Сохраните и используйте URL-адрес `deltaLink` для запроса любых новых сообщений, начиная с этого момента в следующем цикле.</span><span class="sxs-lookup"><span data-stu-id="52f61-216">Save and use the `deltaLink` URL to query for any new messages starting from this point in the next round.</span></span>

><span data-ttu-id="52f61-217">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="52f61-217">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="52f61-218">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52f61-218">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.deltaLink": "/teams('id')/channels('id')/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from": {
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

### <a name="example-2-retrieving-additional-changes"></a><span data-ttu-id="52f61-219">Пример 2. Извлечение дополнительных изменений</span><span class="sxs-lookup"><span data-stu-id="52f61-219">Example 2: Retrieving additional changes</span></span>

<span data-ttu-id="52f61-220">С помощью ссылки `deltaLink` из последнего цикла прошлого запроса вы сможете получить только те сообщения, которые изменились (путем добавления или обновления) в этом канале с момента последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="52f61-220">Using the `deltaLink` from the last request in the last round, you will be able to get only those messages that have changed (by being added, or updated) in that channel since then.</span></span> <span data-ttu-id="52f61-221">При условии, что вы не хотите менять максимальный размер страницы ответа, ваш запрос будет выглядеть следующим образом:</span><span class="sxs-lookup"><span data-stu-id="52f61-221">Your request will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

#### <a name="request"></a><span data-ttu-id="52f61-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="52f61-222">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="52f61-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="52f61-223">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_4"
}-->
```msgraph-interactive
GET /teams/{id}/channels/{id}/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="52f61-224">C#</span><span class="sxs-lookup"><span data-stu-id="52f61-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52f61-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52f61-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52f61-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52f61-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52f61-227">Java</span><span class="sxs-lookup"><span data-stu-id="52f61-227">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="52f61-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="52f61-228">Response</span></span>

><span data-ttu-id="52f61-p124">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52f61-p124">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.deltaLink": "/teams('id')/channels('id')/messages/delta?$deltatoken=c3RhcnRUaW1l5Ti1NTEyODc1ODB0OTAyXGFdZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from": {
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


