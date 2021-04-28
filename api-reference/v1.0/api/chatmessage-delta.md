---
title: 'chatMessage: delta'
description: Получение списка сообщений (без ответов) в канале команды. С помощью разностного запроса можно получить новые или обновленные сообщения в канале.
localization_priority: Priority
doc_type: apiPageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: ec91b75edb44f9c81ff420226bf9ebf984d002be
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052469"
---
# <a name="chatmessage-delta"></a><span data-ttu-id="b946f-104">chatMessage: delta</span><span class="sxs-lookup"><span data-stu-id="b946f-104">chatMessage: delta</span></span>

<span data-ttu-id="b946f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b946f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b946f-106">Получение списка [сообщений](../resources/chatmessage.md) (без ответов) в [канале](../resources/channel.md) [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="b946f-106">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="b946f-107">С помощью разностного запроса можно получить новые или обновленные сообщения в канале.</span><span class="sxs-lookup"><span data-stu-id="b946f-107">By using delta query, you can get new or updated messages in a channel.</span></span>

> <span data-ttu-id="b946f-108">**Примечание.** Разностный запрос возвращает сообщения только за последние восемь месяцев.</span><span class="sxs-lookup"><span data-stu-id="b946f-108">**Note:** Delta will only return messages within the last eight months.</span></span> <span data-ttu-id="b946f-109">Чтобы получить более ранние сообщения, можно воспользоваться методом [GET /teams/{team-id}/channels/{channel-id}/messages](channel-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="b946f-109">You can use [GET /teams/{team-id}/channels/{channel-id}/messages](channel-list-messages.md) to retrieve older messages.</span></span>

<span data-ttu-id="b946f-p104">Запрос изменений поддерживает как полную синхронизацию с получением всех событий в определенном представлении календаря, так и добавочную синхронизацию с получением тех событий, которые изменились в представлении календаря с момента последней синхронизации. Как правило, сначала выполняется полная синхронизация, а затем в представление сообщений периодически добавляются изменения.</span><span class="sxs-lookup"><span data-stu-id="b946f-p104">Delta query supports both full synchronization that retrieves all the messages in the specified channel, and incremental synchronization that retrieves those messages that have been added or changed in the channel since the last synchronization. Typically, you would do an initial full synchronization, and then get incremental changes to that messages view periodically.</span></span>

<span data-ttu-id="b946f-112">Чтобы получить ответы на сообщение, используйте операцию [перечисления ответов на сообщение](chatmessage-list-replies.md) или [получения ответа на сообщение](chatmessage-get.md).</span><span class="sxs-lookup"><span data-stu-id="b946f-112">To get the replies for a message, use the [list message replies](chatmessage-list-replies.md) or the [get message reply](chatmessage-get.md) operation.</span></span>

<span data-ttu-id="b946f-113">Запрос GET с функцией delta возвращает одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="b946f-113">A GET request with the delta function returns either:</span></span>

- <span data-ttu-id="b946f-114">ссылку `nextLink` (содержащую URL-адрес с вызовом функции **delta** и `skipToken`), или</span><span class="sxs-lookup"><span data-stu-id="b946f-114">A `nextLink` (that contains a URL with a **delta** function call and a `skipToken`), or</span></span>
- <span data-ttu-id="b946f-115">ссылку `deltaLink` (содержащую URL-адрес с вызовом функции **delta** и `deltaToken`).</span><span class="sxs-lookup"><span data-stu-id="b946f-115">A `deltaLink` (that contains a URL with a **delta** function call and `deltaToken`).</span></span>

<span data-ttu-id="b946f-116">Маркеры состояния полностью непрозрачны для клиента.</span><span class="sxs-lookup"><span data-stu-id="b946f-116">State tokens are completely opaque to the client.</span></span> <span data-ttu-id="b946f-117">Чтобы продолжить цикл отслеживания изменений, просто скопируйте и примените URL-адрес `nextLink` или `deltaLink`, возвращенный последним запросом GET, при следующем вызове функции delta для этого представления календаря.</span><span class="sxs-lookup"><span data-stu-id="b946f-117">To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next delta function call for that same calendar view.</span></span> <span data-ttu-id="b946f-118">Ссылка `deltaLink` в ответе означает, что текущий цикл отслеживания изменений завершен.</span><span class="sxs-lookup"><span data-stu-id="b946f-118">A `deltaLink` returned in a response signifies that the current round of change tracking is complete.</span></span> <span data-ttu-id="b946f-119">Вы можете сохранить и использовать URL-адрес `deltaLink` при начале работы для получения дополнительных изменений (сообщения, измененные или опубликованные после получения `deltaLink`).</span><span class="sxs-lookup"><span data-stu-id="b946f-119">You can save and use the `deltaLink` URL when you begin the to retrieve additional changes (messages changed or posted after acquiring `deltaLink`).</span></span>

<span data-ttu-id="b946f-120">Дополнительные сведения см. в документации по [разностному запросу](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="b946f-120">For more information, see the [delta query](/graph/delta-query-overview) documentation.</span></span>

## <a name="permissions"></a><span data-ttu-id="b946f-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b946f-121">Permissions</span></span>

<span data-ttu-id="b946f-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b946f-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="b946f-124">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b946f-124">Permission Type</span></span>                        |<span data-ttu-id="b946f-125">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b946f-125">Permissions (from least to most privileged)</span></span>  |
|---------------------------------------|---------------------------------------------|
|<span data-ttu-id="b946f-126">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b946f-126">Delegated (work or school account)</span></span>     | <span data-ttu-id="b946f-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="b946f-127">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="b946f-128">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b946f-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b946f-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b946f-129">Not Supported</span></span>                                |
|<span data-ttu-id="b946f-130">Приложение</span><span class="sxs-lookup"><span data-stu-id="b946f-130">Application</span></span>                            | <span data-ttu-id="b946f-131">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="b946f-131">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span> |

> <span data-ttu-id="b946f-132">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="b946f-132">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="b946f-133">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="b946f-133">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="b946f-134">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="b946f-134">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="b946f-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b946f-135">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="b946f-136">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="b946f-136">Query parameters</span></span>

<span data-ttu-id="b946f-137">Отслеживание изменений в сообщениях в канале — это цикл из одного или нескольких вызовов функции **delta**.</span><span class="sxs-lookup"><span data-stu-id="b946f-137">Tracking changes in channel messages incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="b946f-138">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="b946f-138">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="b946f-139">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="b946f-139">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="b946f-140">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="b946f-140">You only need to specify any query parameters once upfront.</span></span>

<span data-ttu-id="b946f-141">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержатся закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="b946f-141">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="b946f-142">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="b946f-142">Query parameter</span></span>      | <span data-ttu-id="b946f-143">Тип</span><span class="sxs-lookup"><span data-stu-id="b946f-143">Type</span></span>   |<span data-ttu-id="b946f-144">Описание</span><span class="sxs-lookup"><span data-stu-id="b946f-144">Description</span></span>|
|:---------------|:--------|:----------|
| `$deltatoken` | <span data-ttu-id="b946f-145">string</span><span class="sxs-lookup"><span data-stu-id="b946f-145">string</span></span> | <span data-ttu-id="b946f-146">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` при предыдущем вызове функции **delta** и указывает на завершение этого цикла отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="b946f-146">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="b946f-147">Сохраните URL-адрес `deltaLink` с этим маркером и примените его в первом запросе следующей итерации отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="b946f-147">Save and apply the entire `deltaLink` URL including this token in the first request of the next iteration of change tracking for that collection.</span></span>|
| `$skiptoken` | <span data-ttu-id="b946f-148">string</span><span class="sxs-lookup"><span data-stu-id="b946f-148">string</span></span> | <span data-ttu-id="b946f-149">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` при предыдущем вызове функции **delta** и указывает на то, что  остаются не отслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="b946f-149">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked.</span></span> |

### <a name="optional-odata-query-parameters"></a><span data-ttu-id="b946f-150">Необязательные параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="b946f-150">Optional OData query parameters</span></span>

<span data-ttu-id="b946f-151">Этим API поддерживаются указанные ниже [параметры запросов OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b946f-151">The following [OData query parameters](/graph/query-parameters) are supported by this API:</span></span>
- <span data-ttu-id="b946f-152">`$top`, указывает максимальное количество сообщений, которое нужно получить в результате вызова.</span><span class="sxs-lookup"><span data-stu-id="b946f-152">`$top`, represents maximum number of messages to fetch in a call.</span></span> <span data-ttu-id="b946f-153">Верхний предел – **50**.</span><span class="sxs-lookup"><span data-stu-id="b946f-153">The upper limit is **50**.</span></span>
- <span data-ttu-id="b946f-154">`$skip`, указывает, сколько сообщений нужно пропустить в начале списка.</span><span class="sxs-lookup"><span data-stu-id="b946f-154">`$skip`, represents how many messages to skip at the beginning of the list.</span></span>
- <span data-ttu-id="b946f-155">`$filter` поддерживает возврат сообщений, удовлетворяющих определенным условиям.</span><span class="sxs-lookup"><span data-stu-id="b946f-155">`$filter` allows returning messages that meet a certain criteria.</span></span> <span data-ttu-id="b946f-156">Единственное свойство, поддерживающее фильтрацию, — это `lastModifiedDateTime`, при этом поддерживается только оператор **gt**.</span><span class="sxs-lookup"><span data-stu-id="b946f-156">The only property that supports filtering is `lastModifiedDateTime`, and only the **gt** operator is supported.</span></span> <span data-ttu-id="b946f-157">Например, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` будет получать любые сообщения, созданные или измененные после указанной даты и времени.</span><span class="sxs-lookup"><span data-stu-id="b946f-157">For example, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` will fetch any messages created or changed after the specified date time.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b946f-158">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b946f-158">Request headers</span></span>
| <span data-ttu-id="b946f-159">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b946f-159">Header</span></span>        | <span data-ttu-id="b946f-160">Значение</span><span class="sxs-lookup"><span data-stu-id="b946f-160">Value</span></span>                     |
|---------------|---------------------------|
| <span data-ttu-id="b946f-161">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b946f-161">Authorization</span></span> | <span data-ttu-id="b946f-p112">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b946f-p112">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b946f-164">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b946f-164">Request Body</span></span>

<span data-ttu-id="b946f-165">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b946f-165">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b946f-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="b946f-166">Response</span></span>

<span data-ttu-id="b946f-167">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b946f-167">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span> <span data-ttu-id="b946f-168">Отклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="b946f-168">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

## <a name="examples"></a><span data-ttu-id="b946f-169">Примеры</span><span class="sxs-lookup"><span data-stu-id="b946f-169">Examples</span></span>

### <a name="example-1-initial-synchronization"></a><span data-ttu-id="b946f-170">Пример 1: Первоначальная синхронизация</span><span class="sxs-lookup"><span data-stu-id="b946f-170">Example 1: Initial synchronization</span></span>

<span data-ttu-id="b946f-171">В приведенном ниже примере показана серия из трех запросов для синхронизации сообщений в заданном канале.</span><span class="sxs-lookup"><span data-stu-id="b946f-171">The following example shows a series of three requests to synchronize the messages in the given channel.</span></span> <span data-ttu-id="b946f-172">В канале пять сообщений.</span><span class="sxs-lookup"><span data-stu-id="b946f-172">There are five messages in the channel.</span></span>

- <span data-ttu-id="b946f-173">Шаг 1. [Исходный запрос](#initial-request) и [отклик](#initial-request-response).</span><span class="sxs-lookup"><span data-stu-id="b946f-173">Step 1: [initial request](#initial-request) and [response](#initial-request-response).</span></span>
- <span data-ttu-id="b946f-174">Шаг 2. [Второй запрос](#second-request) и [отклик](#second-request-response).</span><span class="sxs-lookup"><span data-stu-id="b946f-174">Step 2: [second request](#second-request) and [response](#second-request-response)</span></span>
- <span data-ttu-id="b946f-175">Шаг 3. [Третий запрос](#third-request) и [последний отклик](#third-request-response).</span><span class="sxs-lookup"><span data-stu-id="b946f-175">Step 3: [third request](#third-request) and [final response](#third-request-response).</span></span>

<span data-ttu-id="b946f-p115">В примерах показаны только некоторые свойства события. При фактическом вызове возвращается большинство свойств события.</span><span class="sxs-lookup"><span data-stu-id="b946f-p115">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span>

<span data-ttu-id="b946f-178">Узнайте также, что нужно сделать [для получения дополнительных изменений](#example-2-retrieving-additional-changes).</span><span class="sxs-lookup"><span data-stu-id="b946f-178">See also what you'll do [to retrieve additional changes](#example-2-retrieving-additional-changes).</span></span>

#### <a name="initial-request"></a><span data-ttu-id="b946f-179">Исходный запрос</span><span class="sxs-lookup"><span data-stu-id="b946f-179">Initial request</span></span>

<span data-ttu-id="b946f-p116">В этом примере сообщения канала синхронизируются впервые, поэтому исходный запрос на синхронизацию не содержит маркер состояния. В этом цикле возвращаются все события в представлении календаря.</span><span class="sxs-lookup"><span data-stu-id="b946f-p116">In this example, the channel messages are being synchronized for the first time, so the initial sync request does not include any state token. This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="b946f-182">В запросе указывается необязательный заголовок запроса, odata.top, возвращающий 2 события одновременно.</span><span class="sxs-lookup"><span data-stu-id="b946f-182">The request specifies the optional request header, odata.top, returning 2 events at a time.</span></span>


# <a name="http"></a>[<span data-ttu-id="b946f-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="b946f-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagedeltachannel_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$top=2
```
# <a name="c"></a>[<span data-ttu-id="b946f-184">C#</span><span class="sxs-lookup"><span data-stu-id="b946f-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagedeltachannel-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b946f-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b946f-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagedeltachannel-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b946f-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b946f-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagedeltachannel-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b946f-187">Java</span><span class="sxs-lookup"><span data-stu-id="b946f-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chatmessagedeltachannel-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="initial-request-response"></a><span data-ttu-id="b946f-188">Ответ на исходный запрос</span><span class="sxs-lookup"><span data-stu-id="b946f-188">Initial request response</span></span>

<span data-ttu-id="b946f-189">Ответ включает два сообщения и заголовок ответа `@odata.nextLink` с маркером `skipToken`.</span><span class="sxs-lookup"><span data-stu-id="b946f-189">The response includes two messages and a `@odata.nextLink` response header with a `skipToken`.</span></span> <span data-ttu-id="b946f-190">URL-адрес `nextLink` указывает, что в канале еще остались сообщения.</span><span class="sxs-lookup"><span data-stu-id="b946f-190">The `nextLink` URL indicates there are more messages in the channel to get.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(chatMessage)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$skiptoken=-FG3FPHv7HuyuazNLuy3eXlzQGbEjYLUsW9-pYkmXgn5KGsaOwrCoor2W23dGNNM1KtAX4AyvpFQNVsBgsEwUOX9lw8x9zDumgJy-C-UbjZLlZDQACyC9FyrVelZus9n.--rshdLwy_WBFJd8anPXJPbSUtUD7r3V4neB5tcrG58",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1606515483514",
            "messageType": "message",
            "createdDateTime": "2020-11-27T22:18:03.514Z",
            "lastModifiedDateTime": "2020-11-27T22:18:03.514Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1606515483514?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1606515483514&parentMessageId=1606515483514",
            "policyViolation": null,
            "id": "1606515483514",
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Test"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1606691795113",
            "messageType": "message",
            "createdDateTime": "2020-11-29T23:16:35.113Z",
            "lastModifiedDateTime": "2020-11-29T23:16:35.113Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1606691795113?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1606691795113&parentMessageId=1606691795113",
            "policyViolation": null,
            "id": "1606691795113",
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "HelloWorld 11/29/2020 3:16:31 PM -08:00"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

#### <a name="second-request"></a><span data-ttu-id="b946f-191">Второй запрос</span><span class="sxs-lookup"><span data-stu-id="b946f-191">Second request</span></span>

<span data-ttu-id="b946f-192">Второй запрос указывает URL-адрес `nextLink`, полученный из предыдущего ответа.</span><span class="sxs-lookup"><span data-stu-id="b946f-192">The second request specifies the `nextLink` URL returned from the previous response.</span></span> <span data-ttu-id="b946f-193">Обратите внимание, что в нем больше не требуется указывать те же основные параметры, что и в исходном запросе, так как маркер `skipToken` в URL-адресе `nextLink` включает их в закодированном виде.</span><span class="sxs-lookup"><span data-stu-id="b946f-193">Notice that it no longer has to specify the same top parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>


# <a name="http"></a>[<span data-ttu-id="b946f-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="b946f-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagedeltachannel_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$skiptoken=-FG3FPHv7HuyuazNLuy3eXlzQGbEjYLUsW9-pYkmXgn5KGsaOwrCoor2W23dGNNM1KtAX4AyvpFQNVsBgsEwUOX9lw8x9zDumgJy-C-UbjZLlZDQACyC9FyrVelZus9n.--rshdLwy_WBFJd8anPXJPbSUtUD7r3V4neB5tcrG58
```
# <a name="c"></a>[<span data-ttu-id="b946f-195">C#</span><span class="sxs-lookup"><span data-stu-id="b946f-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagedeltachannel-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b946f-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b946f-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagedeltachannel-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b946f-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b946f-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagedeltachannel-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b946f-198">Java</span><span class="sxs-lookup"><span data-stu-id="b946f-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chatmessagedeltachannel-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="second-request-response"></a><span data-ttu-id="b946f-199">Ответ на второй запрос</span><span class="sxs-lookup"><span data-stu-id="b946f-199">Second request response</span></span>

<span data-ttu-id="b946f-200">Второй ответ содержит следующие 2 сообщения в папке и заголовок ответа `@odata.nextLink` с `skipToken`, и указывает, что в канале еще остались сообщения.</span><span class="sxs-lookup"><span data-stu-id="b946f-200">The second response returns the next 2 messages and a `@odata.nextLink` response header with a `skipToken`, indicates there are more messages in the channel to get.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(chatMessage)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$skiptoken=8UusBixEHS9UUau6uGcryrA6FpnWwMJbuTYILM1PArHxnZzDVcsHQrijNzCyIVeEauMQsKUfMhNjLWFs1o4sBS_LofJ7xMftZUfec_pijuT6cAk5ugcWCca9RCjK7iVj.DKZ9w4bX9vCR7Sj9P0_qxjLAAPiEZgxlOxxmCLMzHJ4",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1606691812117",
            "messageType": "message",
            "createdDateTime": "2020-11-29T23:16:52.117Z",
            "lastModifiedDateTime": "2020-11-29T23:16:52.117Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1606691812117?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1606691812117&parentMessageId=1606691812117",
            "policyViolation": null,
            "id": "1606691812117",
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "HelloWorld 11/29/2020 3:16:51 PM -08:00"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1606691846203",
            "messageType": "message",
            "createdDateTime": "2020-11-29T23:17:26.203Z",
            "lastModifiedDateTime": "2020-11-29T23:17:26.203Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1606691846203?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1606691846203&parentMessageId=1606691846203",
            "policyViolation": null,
            "id": "1606691846203",
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "HelloWorld 11/29/2020 3:17:25 PM -08:00"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

#### <a name="third-request"></a><span data-ttu-id="b946f-201">Третий запрос</span><span class="sxs-lookup"><span data-stu-id="b946f-201">Third request</span></span>

<span data-ttu-id="b946f-202">Третий запрос продолжает использовать маркер `nextLink`, полученный из последнего запроса на синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="b946f-202">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b946f-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="b946f-203">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagedeltachannel_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$skiptoken=8UusBixEHS9UUau6uGcryrA6FpnWwMJbuTYILM1PArHxnZzDVcsHQrijNzCyIVeEauMQsKUfMhNjLWFs1o4sBS_LofJ7xMftZUfec_pijuT6cAk5ugcWCca9RCjK7iVj.DKZ9w4bX9vCR7Sj9P0_qxjLAAPiEZgxlOxxmCLMzHJ4
```
# <a name="c"></a>[<span data-ttu-id="b946f-204">C#</span><span class="sxs-lookup"><span data-stu-id="b946f-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagedeltachannel-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b946f-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b946f-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagedeltachannel-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b946f-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b946f-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagedeltachannel-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b946f-207">Java</span><span class="sxs-lookup"><span data-stu-id="b946f-207">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chatmessagedeltachannel-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="third-request-response"></a><span data-ttu-id="b946f-208">Ответ на третий запрос</span><span class="sxs-lookup"><span data-stu-id="b946f-208">Third request response</span></span>

<span data-ttu-id="b946f-209">Третий ответ содержит только оставшиеся сообщения в канале и заголовок ответа `@odata.deltaLink` с `deltaToken`, что указывает на то, что все сообщения в канале считаны.</span><span class="sxs-lookup"><span data-stu-id="b946f-209">The third response returns the only remaining messages in the channel and a `@odata.deltaLink` response header with a `deltaToken` which indicates that all messages in the channel have been read.</span></span> <span data-ttu-id="b946f-210">Сохраните и используйте URL-адрес `deltaLink` для запроса любых новых сообщений, начиная с этого момента.</span><span class="sxs-lookup"><span data-stu-id="b946f-210">Save and use the `deltaLink` URL to query for any new messages starting from this point onwards.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(chatMessage)",
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$deltatoken=aQdvS1VwGCSRxVmZJqykmDik_JIC44iCZpv-GLiA2VnFuE5yG-kCEBROb2iaPT_y_eMWVQtBO_ejzzyIxl00ji-tQ3HzAbW4liZAVG88lO3nG_6-MBFoHY1n8y21YUzjocG-Cn1tCNeeLPLTzIe5Dw.EP9gLiCoF2CE_e6l_m1bTk2aokD9KcgfgfcLGqd1r_4",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1611351582080",
            "messageType": "message",
            "createdDateTime": "2021-01-22T21:39:42.08Z",
            "lastModifiedDateTime": "2021-01-22T21:39:42.08Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1611351582080?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1611351582080&parentMessageId=1611351582080",
            "policyViolation": null,
            "id": "1611351582080",
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "HelloWorld 1/22/2021 1:39:39 PM -08:00"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1611351603178",
            "messageType": "message",
            "createdDateTime": "2021-01-22T21:40:03.178Z",
            "lastModifiedDateTime": "2021-01-22T21:40:03.178Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1611351603178?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1611351603178&parentMessageId=1611351603178",
            "policyViolation": null,
            "id": "1611351603178",
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "HelloWorld 1/22/2021 1:40:00 PM -08:00"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

### <a name="example-2-retrieving-additional-changes"></a><span data-ttu-id="b946f-211">Пример 2. Извлечение дополнительных изменений</span><span class="sxs-lookup"><span data-stu-id="b946f-211">Example 2: Retrieving additional changes</span></span>

<span data-ttu-id="b946f-212">С помощью ссылки `deltaLink` из последнего цикла прошлого запроса вы сможете получить только те сообщения, которые изменились (путем добавления или обновления) в этом канале с момента последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b946f-212">Using the `deltaLink` from the last request in the last round, you will be able to get only those messages that have changed (by being added, or updated) in that channel since then.</span></span> <span data-ttu-id="b946f-213">При условии, что вы не хотите менять максимальный размер страницы ответа, ваш запрос будет выглядеть следующим образом:</span><span class="sxs-lookup"><span data-stu-id="b946f-213">Your request will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

#### <a name="request"></a><span data-ttu-id="b946f-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="b946f-214">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b946f-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="b946f-215">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagedeltachannel_4"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$deltatoken=aQdvS1VwGCSRxVmZJqykmDik_JIC44iCZpv-GLiA2VnFuE5yG-kCEBROb2iaPT_y_eMWVQtBO_ejzzyIxl00ji-tQ3HzAbW4liZAVG88lO3nG_6-MBFoHY1n8y21YUzjocG-Cn1tCNeeLPLTzIe5Dw.EP9gLiCoF2CE_e6l_m1bTk2aokD9KcgfgfcLGqd1r_4
```
# <a name="c"></a>[<span data-ttu-id="b946f-216">C#</span><span class="sxs-lookup"><span data-stu-id="b946f-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagedeltachannel-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b946f-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b946f-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagedeltachannel-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b946f-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b946f-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagedeltachannel-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b946f-219">Java</span><span class="sxs-lookup"><span data-stu-id="b946f-219">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chatmessagedeltachannel-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b946f-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="b946f-220">Response</span></span>

><span data-ttu-id="b946f-221">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b946f-221">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(chatMessage)",
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$deltatoken=aQdvS1VwGCSRxVmZJqykmDik_JIC44iCZpv-GLiA2VnFuE5yG-kCEBROb2iaPT_yjz2nsMoh1gXNtXii7s78HapCi5woifXqwXlVNxICh8wUUnvE2gExsa8eZ2Vy_ch5rVIhm067_1mUPML3iYUVyg.3o0rhgaBUduuxOr98An5pjBDP5JjKUiVWku3flSiOsk",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1616989510408",
            "messageType": "message",
            "createdDateTime": "2021-03-29T03:45:10.408Z",
            "lastModifiedDateTime": "2021-03-29T03:45:10.408Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616989510408?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616989510408&parentMessageId=1616989510408",
            "policyViolation": null,
            "id": "1616989510408",
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Hello World 28th March 2021"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
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


