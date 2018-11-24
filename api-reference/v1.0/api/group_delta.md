# <a name="group-delta"></a><span data-ttu-id="c5b54-101">group: delta</span><span class="sxs-lookup"><span data-stu-id="c5b54-101">group: delta</span></span>
<span data-ttu-id="c5b54-102">Get вновь созданных, обновлении или удалении групп, включая изменения членства в группе, без необходимости выполнять полное чтение коллекции всей группы.</span><span class="sxs-lookup"><span data-stu-id="c5b54-102">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="c5b54-103">Для получения дополнительных сведений в разделе [С помощью запроса дельты](../../../concepts/delta_query_overview.md) .</span><span class="sxs-lookup"><span data-stu-id="c5b54-103">See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5b54-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5b54-104">Permissions</span></span>

<span data-ttu-id="c5b54-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5b54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c5b54-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5b54-107">Permission type</span></span>      | <span data-ttu-id="c5b54-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5b54-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5b54-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5b54-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c5b54-110">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5b54-110">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c5b54-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5b54-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5b54-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5b54-112">Not supported.</span></span>    |
|<span data-ttu-id="c5b54-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5b54-113">Application</span></span> | <span data-ttu-id="c5b54-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5b54-114">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5b54-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5b54-115">HTTP request</span></span>

<span data-ttu-id="c5b54-116">Чтобы начать отслеживать изменения, выполните запрос к ресурсу groups, включающий функцию delta.</span><span class="sxs-lookup"><span data-stu-id="c5b54-116">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="c5b54-117">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="c5b54-117">Query parameters</span></span>

<span data-ttu-id="c5b54-p103">Отслеживание изменений в группах запускает один или более циклов вызовов **разностной** функции. Если вы используете какой-либо параметр запроса (кроме `$deltatoken` и `$skiptoken`), вам необходимо указать его в исходном **разностном** запросе. Microsoft Graph автоматически кодирует любые указанные параметры в той части предоставленного в ответе URL-адреса `nextLink` или `deltaLink`, которая содержит токен.</span><span class="sxs-lookup"><span data-stu-id="c5b54-p103">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="c5b54-121">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="c5b54-121">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="c5b54-122">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="c5b54-122">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="c5b54-123">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="c5b54-123">Query parameter</span></span> | <span data-ttu-id="c5b54-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c5b54-124">Type</span></span>  |<span data-ttu-id="c5b54-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c5b54-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c5b54-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="c5b54-126">$deltatoken</span></span> | <span data-ttu-id="c5b54-127">строка</span><span class="sxs-lookup"><span data-stu-id="c5b54-127">string</span></span> | <span data-ttu-id="c5b54-p104">Этот [токен состояния](../../../concepts/delta_query_overview.md) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции групп и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="c5b54-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="c5b54-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="c5b54-130">$skiptoken</span></span> | <span data-ttu-id="c5b54-131">строка</span><span class="sxs-lookup"><span data-stu-id="c5b54-131">string</span></span> | <span data-ttu-id="c5b54-132">Этот [токен состояния](../../../concepts/delta_query_overview.md) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что из коллекции групп получены не все изменения.</span><span class="sxs-lookup"><span data-stu-id="c5b54-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="c5b54-133">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="c5b54-133">OData query parameters</span></span>

<span data-ttu-id="c5b54-134">Этот метод поддерживает дополнительные параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c5b54-134">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="c5b54-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство *id* возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="c5b54-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="c5b54-137">Можно использовать `$expand=members` для получения изменения членства.</span><span class="sxs-lookup"><span data-stu-id="c5b54-137">You can use `$expand=members` to get membership changes.</span></span>
- <span data-ttu-id="c5b54-138">Ограниченная поддержка `$filter`:</span><span class="sxs-lookup"><span data-stu-id="c5b54-138">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="c5b54-139">Единственное поддерживаемое выражение `$filter` предназначено для отслеживания изменений в определенном объекте: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="c5b54-139">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="c5b54-140">Допускается фильтрация нескольких объектов.</span><span class="sxs-lookup"><span data-stu-id="c5b54-140">You can filter multiple objects.</span></span> <span data-ttu-id="c5b54-141">Например, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="c5b54-141">For example, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="c5b54-142">Максимальное количество фильтруемых объектов: 50.</span><span class="sxs-lookup"><span data-stu-id="c5b54-142">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5b54-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5b54-143">Request headers</span></span>

| <span data-ttu-id="c5b54-144">Имя</span><span class="sxs-lookup"><span data-stu-id="c5b54-144">Name</span></span>       | <span data-ttu-id="c5b54-145">Описание</span><span class="sxs-lookup"><span data-stu-id="c5b54-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c5b54-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5b54-146">Authorization</span></span>  | <span data-ttu-id="c5b54-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="c5b54-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="c5b54-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5b54-148">Content-Type</span></span>  | <span data-ttu-id="c5b54-149">application/json</span><span class="sxs-lookup"><span data-stu-id="c5b54-149">application/json</span></span> |
| <span data-ttu-id="c5b54-150">Prefer</span><span class="sxs-lookup"><span data-stu-id="c5b54-150">Prefer</span></span> | <span data-ttu-id="c5b54-151">Возвращает = минимальный</span><span class="sxs-lookup"><span data-stu-id="c5b54-151">return=minimal</span></span> <br><br><span data-ttu-id="c5b54-152">Указание этот заголовок с запросом, который использует `deltaLink` возвращает свойства объекта, которые были изменены с момента последнего цикла.</span><span class="sxs-lookup"><span data-stu-id="c5b54-152">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="c5b54-153">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c5b54-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5b54-154">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c5b54-154">Request body</span></span>

<span data-ttu-id="c5b54-155">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5b54-155">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="c5b54-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5b54-156">Response</span></span>

<span data-ttu-id="c5b54-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5b54-157">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="c5b54-158">Ответ также включает в себя состояние маркера, который соответствует любому из `nextLink` URL-адрес или `deltaLink` URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="c5b54-158">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="c5b54-159">Если `nextLink` возвращается URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="c5b54-159">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="c5b54-160">Это означает, что существуют дополнительные страницы данных для получения в сеанс.</span><span class="sxs-lookup"><span data-stu-id="c5b54-160">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="c5b54-161">Приложение по-прежнему производится выполняете запросы, используя `nextLink` URL-адрес, пока не `deltaLink` URL-адрес включен в ответе.</span><span class="sxs-lookup"><span data-stu-id="c5b54-161">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="c5b54-162">Ответ включает тот же набор свойств, как и в запросе начальной дельты.</span><span class="sxs-lookup"><span data-stu-id="c5b54-162">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="c5b54-163">Это позволяет записывать полное текущего состояния объектов при начале цикла дельты.</span><span class="sxs-lookup"><span data-stu-id="c5b54-163">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="c5b54-164">Если `deltaLink` возвращается URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="c5b54-164">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="c5b54-165">Это означает, что нет дополнительных данных о состоянии существующих ресурсов должно быть возвращено.</span><span class="sxs-lookup"><span data-stu-id="c5b54-165">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="c5b54-166">Сохраните и использовать `deltaLink` URL-адрес, чтобы узнать о изменяется с ресурсом в следующего цикла.</span><span class="sxs-lookup"><span data-stu-id="c5b54-166">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="c5b54-167">У вас есть выбор для указания `Prefer:return=minimal` заголовок, чтобы включить в ответ значения для свойств, которые были изменены со времени `deltaLink` был отправлен.</span><span class="sxs-lookup"><span data-stu-id="c5b54-167">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="c5b54-168">Значение по умолчанию: возврата же свойства, что запрос на начальное дельты</span><span class="sxs-lookup"><span data-stu-id="c5b54-168">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="c5b54-169">По умолчанию, запросы с помощью `deltaLink` или `nextLink` возврата же свойства, что выбранный в запросе начальной дельты следующими способами:</span><span class="sxs-lookup"><span data-stu-id="c5b54-169">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="c5b54-170">При изменении свойства возвращает свойство в ответ JSON.</span><span class="sxs-lookup"><span data-stu-id="c5b54-170">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="c5b54-171">Если свойство значение пустое значение, возвращает значение свойства как значение null.</span><span class="sxs-lookup"><span data-stu-id="c5b54-171">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="c5b54-172">Если свойство не был изменен, возвратить значение null.</span><span class="sxs-lookup"><span data-stu-id="c5b54-172">If the property has not changed, return the value as null.</span></span>

> <span data-ttu-id="c5b54-173">**Примечание:** Выше поведение не возможно для различения свойства, который не был изменен и одного, которое было изменено на `null` значение.</span><span class="sxs-lookup"><span data-stu-id="c5b54-173">**Note:** With the above behavior, it is not possible to differentiate between a property that has not changed and one that has changed to a `null` value.</span></span> <span data-ttu-id="c5b54-174">В разделе [во втором примере](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="c5b54-174">See the [second example](#request-2) below.</span></span> <span data-ttu-id="c5b54-175">Если это важно, рекомендуется использовать альтернативный поведение, описанных в следующем разделе.</span><span class="sxs-lookup"><span data-stu-id="c5b54-175">If this is important, we recommend using the alternative behavior described in the next section.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="c5b54-176">Альтернатива: получить только измененные свойства</span><span class="sxs-lookup"><span data-stu-id="c5b54-176">Alternative: return only the changed properties</span></span>

<span data-ttu-id="c5b54-177">Добавление заголовка запроса на необязательный - `prefer:return=minimal` -приводит к следующим образом:</span><span class="sxs-lookup"><span data-stu-id="c5b54-177">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="c5b54-178">При изменении свойства возвращает свойство в ответ JSON.</span><span class="sxs-lookup"><span data-stu-id="c5b54-178">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="c5b54-179">Если свойство значение пустое значение, возвращает значение свойства как значение null.</span><span class="sxs-lookup"><span data-stu-id="c5b54-179">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="c5b54-180">Если свойство не был изменен, не включает свойство в ответ JSON.</span><span class="sxs-lookup"><span data-stu-id="c5b54-180">If the property has not changed, do not include the property in the JSON response.</span></span> <span data-ttu-id="c5b54-181">(Отличается от поведения по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="c5b54-181">(Different from the default behavior.)</span></span>

> <span data-ttu-id="c5b54-182">**Примечание:** Можно добавить заголовок `deltaLink` запроса в любой момент времени в цикле дельты.</span><span class="sxs-lookup"><span data-stu-id="c5b54-182">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="c5b54-183">Заголовок влияет только на набор свойств, включенных в ответ и не затрагивает как выполняется запрос дельты.</span><span class="sxs-lookup"><span data-stu-id="c5b54-183">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="c5b54-184">В разделе в [третьем примере](#request-3) ниже.</span><span class="sxs-lookup"><span data-stu-id="c5b54-184">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="c5b54-185">Пример</span><span class="sxs-lookup"><span data-stu-id="c5b54-185">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="c5b54-186">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="c5b54-186">Request 1</span></span>

<span data-ttu-id="c5b54-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5b54-187">The following is an example of the request.</span></span> <span data-ttu-id="c5b54-188">Существует не `$select` параметр, поэтому по умолчанию набор свойств, отслеживаемых и возвращаются.</span><span class="sxs-lookup"><span data-stu-id="c5b54-188">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response-1"></a><span data-ttu-id="c5b54-189">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="c5b54-189">Response 1</span></span>

<span data-ttu-id="c5b54-190">Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="c5b54-190">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="c5b54-191">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="c5b54-191">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c5b54-192">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5b54-192">All the properties will be returned from an actual call.</span></span>
>
> <span data-ttu-id="c5b54-193">Обратите внимание, сведения о присутствии *members@delta* свойства, которое включает в себя идентификаторы объектов члена группы.</span><span class="sxs-lookup"><span data-stu-id="c5b54-193">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
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

#### <a name="request-2"></a><span data-ttu-id="c5b54-194">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="c5b54-194">Request 2</span></span>

<span data-ttu-id="c5b54-195">В следующем примере показаны начального запроса, выбрав пункт 3 свойства для отслеживания изменений, с ответ по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="c5b54-195">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a><span data-ttu-id="c5b54-196">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="c5b54-196">Response 2</span></span>

<span data-ttu-id="c5b54-197">Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="c5b54-197">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="c5b54-198">Обратите внимание, что `description` и `mailNickname` имеет значение `null` это означает, что они могут не были изменены или были установлены пустое значение.</span><span class="sxs-lookup"><span data-stu-id="c5b54-198">Note that `description` and `mailNickname` have the value of `null` which means that they may have not changed or have been set to an empty value.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null,
      "mailNickname": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="c5b54-199">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="c5b54-199">Request 3</span></span>

<span data-ttu-id="c5b54-200">В следующем примере показаны начального запроса, выбрав пункт 3 свойства для отслеживания изменений, поведение альтернативный минимальной ответа:</span><span class="sxs-lookup"><span data-stu-id="c5b54-200">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="c5b54-201">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="c5b54-201">Response 3</span></span>

<span data-ttu-id="c5b54-202">Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="c5b54-202">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="c5b54-203">Обратите внимание, что `mailNickname` свойство не указан, то есть не был изменен с момента последнего разностного запроса; `displayName` и `description` включены, что означает их значения были изменены.</span><span class="sxs-lookup"><span data-stu-id="c5b54-203">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="c5b54-204">См. также</span><span class="sxs-lookup"><span data-stu-id="c5b54-204">See also</span></span>

- <span data-ttu-id="c5b54-205">[Использование разностного запроса для отслеживания изменений в данных Microsoft Graph](../../../concepts/delta_query_overview.md).</span><span class="sxs-lookup"><span data-stu-id="c5b54-205">[Use delta query to track changes in Microsoft Graph data](../../../concepts/delta_query_overview.md).</span></span>
- <span data-ttu-id="c5b54-206">[Получение добавочные изменения для групп](../../../concepts/delta_query_groups.md).</span><span class="sxs-lookup"><span data-stu-id="c5b54-206">[Get incremental changes for groups](../../../concepts/delta_query_groups.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
