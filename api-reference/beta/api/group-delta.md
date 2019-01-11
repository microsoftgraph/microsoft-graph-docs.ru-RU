---
title: 'group: delta'
description: Get вновь созданных, обновлении или удалении групп, включая изменения членства в группе, без необходимости выполнять полное чтение коллекции всей группы. Для получения дополнительных сведений в разделе с помощью запроса дельты.
localization_priority: Normal
ms.openlocfilehash: 5645fa950faca9f5a49b9db6288eb138553aad0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887873"
---
# <a name="group-delta"></a><span data-ttu-id="dd86f-104">group: delta</span><span class="sxs-lookup"><span data-stu-id="dd86f-104">group: delta</span></span>

> <span data-ttu-id="dd86f-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dd86f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd86f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd86f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd86f-107">Get вновь созданных, обновлении или удалении групп, включая изменения членства в группе, без необходимости выполнять полное чтение коллекции всей группы.</span><span class="sxs-lookup"><span data-stu-id="dd86f-107">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="dd86f-108">Для получения дополнительных сведений в разделе [С помощью запроса дельты](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="dd86f-108">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd86f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd86f-109">Permissions</span></span>

<span data-ttu-id="dd86f-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd86f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd86f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd86f-112">Permission type</span></span>      | <span data-ttu-id="dd86f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd86f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd86f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd86f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="dd86f-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd86f-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dd86f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd86f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd86f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd86f-117">Not supported.</span></span>    |
|<span data-ttu-id="dd86f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd86f-118">Application</span></span> | <span data-ttu-id="dd86f-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd86f-119">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd86f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd86f-120">HTTP request</span></span>

<span data-ttu-id="dd86f-121">Чтобы начать отслеживать изменения, выполните запрос к ресурсу groups, включающий функцию delta.</span><span class="sxs-lookup"><span data-stu-id="dd86f-121">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="dd86f-122">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="dd86f-122">Query parameters</span></span>

<span data-ttu-id="dd86f-p105">Отслеживание изменений в группах запускает один или более циклов вызовов **разностной** функции. Если вы используете какой-либо параметр запроса (кроме `$deltatoken` и `$skiptoken`), вам необходимо указать его в исходном **разностном** запросе. Microsoft Graph автоматически кодирует любые указанные параметры в той части предоставленного в ответе URL-адреса `nextLink` или `deltaLink`, которая содержит токен.</span><span class="sxs-lookup"><span data-stu-id="dd86f-p105">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="dd86f-126">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="dd86f-126">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="dd86f-127">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="dd86f-127">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="dd86f-128">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="dd86f-128">Query parameter</span></span> | <span data-ttu-id="dd86f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="dd86f-129">Type</span></span>  |<span data-ttu-id="dd86f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="dd86f-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dd86f-131">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="dd86f-131">$deltatoken</span></span> | <span data-ttu-id="dd86f-132">строка</span><span class="sxs-lookup"><span data-stu-id="dd86f-132">string</span></span> | <span data-ttu-id="dd86f-p106">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции групп и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="dd86f-p106">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="dd86f-135">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="dd86f-135">$skiptoken</span></span> | <span data-ttu-id="dd86f-136">строка</span><span class="sxs-lookup"><span data-stu-id="dd86f-136">string</span></span> | <span data-ttu-id="dd86f-137">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что из коллекции групп получены не все изменения.</span><span class="sxs-lookup"><span data-stu-id="dd86f-137">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="dd86f-138">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="dd86f-138">OData query parameters</span></span>

<span data-ttu-id="dd86f-139">Этот метод поддерживает дополнительные параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dd86f-139">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="dd86f-p107">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство *id* возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="dd86f-p107">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="dd86f-142">Можно использовать `$expand=members` для получения изменения членства.</span><span class="sxs-lookup"><span data-stu-id="dd86f-142">You can use `$expand=members` to get membership changes.</span></span>
- <span data-ttu-id="dd86f-143">Ограниченная поддержка `$filter`:</span><span class="sxs-lookup"><span data-stu-id="dd86f-143">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="dd86f-144">Единственное поддерживаемое выражение `$filter` предназначено для отслеживания изменений в определенном объекте: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="dd86f-144">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="dd86f-145">Допускается фильтрация нескольких объектов.</span><span class="sxs-lookup"><span data-stu-id="dd86f-145">You can filter multiple objects.</span></span> <span data-ttu-id="dd86f-146">Например, `https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="dd86f-146">For example, `https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="dd86f-147">Максимальное количество фильтруемых объектов: 50.</span><span class="sxs-lookup"><span data-stu-id="dd86f-147">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd86f-148">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd86f-148">Request headers</span></span>

| <span data-ttu-id="dd86f-149">Имя</span><span class="sxs-lookup"><span data-stu-id="dd86f-149">Name</span></span>       | <span data-ttu-id="dd86f-150">Описание</span><span class="sxs-lookup"><span data-stu-id="dd86f-150">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dd86f-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd86f-151">Authorization</span></span>  | <span data-ttu-id="dd86f-152">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="dd86f-152">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="dd86f-153">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd86f-153">Content-Type</span></span>  | <span data-ttu-id="dd86f-154">application/json</span><span class="sxs-lookup"><span data-stu-id="dd86f-154">application/json</span></span> |
| <span data-ttu-id="dd86f-155">Prefer</span><span class="sxs-lookup"><span data-stu-id="dd86f-155">Prefer</span></span> | <span data-ttu-id="dd86f-156">Возвращает = минимальный</span><span class="sxs-lookup"><span data-stu-id="dd86f-156">return=minimal</span></span> <br><br><span data-ttu-id="dd86f-157">Указание этот заголовок с запросом, который использует `deltaLink` возвращает свойства объекта, которые были изменены с момента последнего цикла.</span><span class="sxs-lookup"><span data-stu-id="dd86f-157">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="dd86f-158">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="dd86f-158">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd86f-159">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dd86f-159">Request body</span></span>

<span data-ttu-id="dd86f-160">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd86f-160">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="dd86f-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd86f-161">Response</span></span>

<span data-ttu-id="dd86f-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd86f-162">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="dd86f-163">Ответ также включает в себя состояние маркера, который соответствует любому из `nextLink` URL-адрес или `deltaLink` URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="dd86f-163">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="dd86f-164">Если `nextLink` возвращается URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="dd86f-164">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="dd86f-165">Это означает, что существуют дополнительные страницы данных для получения в сеанс.</span><span class="sxs-lookup"><span data-stu-id="dd86f-165">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="dd86f-166">Приложение по-прежнему производится выполняете запросы, используя `nextLink` URL-адрес, пока не `deltaLink` URL-адрес включен в ответе.</span><span class="sxs-lookup"><span data-stu-id="dd86f-166">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="dd86f-167">Ответ включает тот же набор свойств, как и в запросе начальной дельты.</span><span class="sxs-lookup"><span data-stu-id="dd86f-167">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="dd86f-168">Это позволяет записывать полное текущего состояния объектов при начале цикла дельты.</span><span class="sxs-lookup"><span data-stu-id="dd86f-168">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="dd86f-169">Если `deltaLink` возвращается URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="dd86f-169">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="dd86f-170">Это означает, что нет дополнительных данных о состоянии существующих ресурсов должно быть возвращено.</span><span class="sxs-lookup"><span data-stu-id="dd86f-170">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="dd86f-171">Сохраните и использовать `deltaLink` URL-адрес, чтобы узнать о изменяется с ресурсом в следующего цикла.</span><span class="sxs-lookup"><span data-stu-id="dd86f-171">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="dd86f-172">У вас есть выбор для указания `Prefer:return=minimal` заголовок, чтобы включить в ответ значения для свойств, которые были изменены со времени `deltaLink` был отправлен.</span><span class="sxs-lookup"><span data-stu-id="dd86f-172">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="dd86f-173">Значение по умолчанию: возврата же свойства, что запрос на начальное дельты</span><span class="sxs-lookup"><span data-stu-id="dd86f-173">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="dd86f-174">По умолчанию, запросы с помощью `deltaLink` или `nextLink` возврата же свойства, что выбранный в запросе начальной дельты следующими способами:</span><span class="sxs-lookup"><span data-stu-id="dd86f-174">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="dd86f-175">При изменении свойства новое значение включается в ответе.</span><span class="sxs-lookup"><span data-stu-id="dd86f-175">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="dd86f-176">Этот компонент включает свойства задаются на значение null.</span><span class="sxs-lookup"><span data-stu-id="dd86f-176">This includes properties being set to null value.</span></span>
- <span data-ttu-id="dd86f-177">Если свойство не был изменен, старое значение включается в ответе.</span><span class="sxs-lookup"><span data-stu-id="dd86f-177">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="dd86f-178">Если свойство имеет значение никогда не перед его не будут включены в ответе на всех.</span><span class="sxs-lookup"><span data-stu-id="dd86f-178">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="dd86f-179">**Примечание:** С помощью этого поведения, посмотрев ответа не позволяет определить, будет ли свойство изменяется, или не.</span><span class="sxs-lookup"><span data-stu-id="dd86f-179">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="dd86f-180">Кроме того ответы дельты, как правило больших так как они содержат все значения свойств - как показано в следующем [примере второй](#request-2) .</span><span class="sxs-lookup"><span data-stu-id="dd86f-180">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="dd86f-181">Альтернатива: получить только измененные свойства</span><span class="sxs-lookup"><span data-stu-id="dd86f-181">Alternative: return only the changed properties</span></span>

<span data-ttu-id="dd86f-182">Добавление заголовка запроса на необязательный - `prefer:return=minimal` -приводит к следующим образом:</span><span class="sxs-lookup"><span data-stu-id="dd86f-182">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="dd86f-183">При изменении свойства новое значение включается в ответе.</span><span class="sxs-lookup"><span data-stu-id="dd86f-183">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="dd86f-184">Этот компонент включает свойства задаются на значение null.</span><span class="sxs-lookup"><span data-stu-id="dd86f-184">This includes properties being set to null value.</span></span>
- <span data-ttu-id="dd86f-185">Если свойство не был изменен, свойство не включается в ответ на всех.</span><span class="sxs-lookup"><span data-stu-id="dd86f-185">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="dd86f-186">(Отличается от поведения по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="dd86f-186">(Different from the default behavior.)</span></span>

> <span data-ttu-id="dd86f-187">**Примечание:** Можно добавить заголовок `deltaLink` запроса в любой момент времени в цикле дельты.</span><span class="sxs-lookup"><span data-stu-id="dd86f-187">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="dd86f-188">Заголовок влияет только на набор свойств, включенных в ответ и не затрагивает как выполняется запрос дельты.</span><span class="sxs-lookup"><span data-stu-id="dd86f-188">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="dd86f-189">В разделе в [третьем примере](#request-3) ниже.</span><span class="sxs-lookup"><span data-stu-id="dd86f-189">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="dd86f-190">Пример</span><span class="sxs-lookup"><span data-stu-id="dd86f-190">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="dd86f-191">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="dd86f-191">Request 1</span></span>

<span data-ttu-id="dd86f-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd86f-192">The following is an example of the request.</span></span> <span data-ttu-id="dd86f-193">Существует не `$select` параметр, поэтому по умолчанию набор свойств, отслеживаемых и возвращаются.</span><span class="sxs-lookup"><span data-stu-id="dd86f-193">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta
```

#### <a name="response-1"></a><span data-ttu-id="dd86f-194">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="dd86f-194">Response 1</span></span>

<span data-ttu-id="dd86f-195">Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="dd86f-195">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="dd86f-196">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="dd86f-196">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dd86f-197">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd86f-197">All the properties will be returned from an actual call.</span></span>
>
> <span data-ttu-id="dd86f-198">Обратите внимание, сведения о присутствии *members@delta* свойства, которое включает в себя идентификаторы объектов члена группы.</span><span class="sxs-lookup"><span data-stu-id="dd86f-198">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
  "value":[
    {
      "classification": "classification-value",
      "createdDateTime":"datetime-value",
      "description":"Test group 1",
      "displayName":"TestGroup1",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

#### <a name="request-2"></a><span data-ttu-id="dd86f-199">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="dd86f-199">Request 2</span></span>

<span data-ttu-id="dd86f-200">В следующем примере показаны начального запроса, выбрав пункт 3 свойства для отслеживания изменений, с ответ по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="dd86f-200">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a><span data-ttu-id="dd86f-201">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="dd86f-201">Response 2</span></span>

<span data-ttu-id="dd86f-202">Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="dd86f-202">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="dd86f-203">Обратите внимание на то, что все свойства 3 включенных в ответ и не известно, какие из них были изменены с момента `deltaLink` был получен.</span><span class="sxs-lookup"><span data-stu-id="dd86f-203">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null,
      "mailNickname": "mailNickname-value"
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="dd86f-204">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="dd86f-204">Request 3</span></span>

<span data-ttu-id="dd86f-205">В следующем примере показаны начального запроса, выбрав пункт 3 свойства для отслеживания изменений, поведение альтернативный минимальной ответа:</span><span class="sxs-lookup"><span data-stu-id="dd86f-205">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="dd86f-206">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="dd86f-206">Response 3</span></span>

<span data-ttu-id="dd86f-207">Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="dd86f-207">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="dd86f-208">Обратите внимание, что `mailNickname` свойство не указан, то есть не был изменен с момента последнего разностного запроса; `displayName` и `description` включены, что означает их значения были изменены.</span><span class="sxs-lookup"><span data-stu-id="dd86f-208">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="dd86f-209">См. также</span><span class="sxs-lookup"><span data-stu-id="dd86f-209">See also</span></span>

- <span data-ttu-id="dd86f-210">[Использование разностного запроса для отслеживания изменений в данных Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="dd86f-210">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="dd86f-211">[Получение добавочные изменения для групп](/graph/delta-query-groups).</span><span class="sxs-lookup"><span data-stu-id="dd86f-211">[Get incremental changes for groups](/graph/delta-query-groups).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
