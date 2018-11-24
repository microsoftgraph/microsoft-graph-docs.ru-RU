# <a name="user-delta"></a><span data-ttu-id="f063b-101">user: delta</span><span class="sxs-lookup"><span data-stu-id="f063b-101">user: delta</span></span>

<span data-ttu-id="f063b-102">Get вновь созданных, обновлении или удалении пользователей без необходимости выполнять полное чтение коллекции всей пользователя.</span><span class="sxs-lookup"><span data-stu-id="f063b-102">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="f063b-103">Дополнительные сведения см [Отслеживание изменений](../../../concepts/delta_query_overview.md) .</span><span class="sxs-lookup"><span data-stu-id="f063b-103">See [Track changes](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="f063b-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f063b-104">Permissions</span></span>

<span data-ttu-id="f063b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f063b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="f063b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f063b-107">Permission type</span></span>      | <span data-ttu-id="f063b-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f063b-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f063b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f063b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f063b-110">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f063b-110">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f063b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f063b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f063b-112">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f063b-112">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="f063b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f063b-113">Application</span></span> | <span data-ttu-id="f063b-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f063b-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f063b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f063b-115">HTTP request</span></span>

<span data-ttu-id="f063b-116">Чтобы начать отслеживать изменения, выполните запрос к ресурсу users, включающий функцию delta.</span><span class="sxs-lookup"><span data-stu-id="f063b-116">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="f063b-117">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="f063b-117">Query parameters</span></span>

<span data-ttu-id="f063b-118">Отслеживание изменений в пользователи могут возникать round один или несколько вызовов функций **дельты** .</span><span class="sxs-lookup"><span data-stu-id="f063b-118">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="f063b-119">При использовании любого параметра запроса (отличный от `$deltatoken` и `$skiptoken`), необходимо указать его в запрос начальной **дельты** .</span><span class="sxs-lookup"><span data-stu-id="f063b-119">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="f063b-120">Microsoft Graph автоматически Кодирует указанный параметров в маркеров часть `nextLink` или `deltaLink` URL-адреса, приведенные в ответе.</span><span class="sxs-lookup"><span data-stu-id="f063b-120">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="f063b-121">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="f063b-121">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="f063b-122">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="f063b-122">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="f063b-123">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="f063b-123">Query parameter</span></span>      | <span data-ttu-id="f063b-124">Тип</span><span class="sxs-lookup"><span data-stu-id="f063b-124">Type</span></span>   |<span data-ttu-id="f063b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f063b-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f063b-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="f063b-126">$deltatoken</span></span> | <span data-ttu-id="f063b-127">строка</span><span class="sxs-lookup"><span data-stu-id="f063b-127">string</span></span> | <span data-ttu-id="f063b-p104">Этот [токен состояния](../../../concepts/delta_query_overview.md) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции пользователей и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="f063b-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="f063b-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="f063b-130">$skiptoken</span></span> | <span data-ttu-id="f063b-131">строка</span><span class="sxs-lookup"><span data-stu-id="f063b-131">string</span></span> | <span data-ttu-id="f063b-132">Этот [токен состояния](../../../concepts/delta_query_overview.md) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что в коллекции пользователей остаются неотслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="f063b-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="f063b-133">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="f063b-133">OData query parameters</span></span>

<span data-ttu-id="f063b-134">Этот метод поддерживает дополнительные параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f063b-134">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="f063b-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство *id* возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="f063b-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="f063b-137">Ограниченная поддержка `$filter`:</span><span class="sxs-lookup"><span data-stu-id="f063b-137">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="f063b-138">Единственное поддерживаемое выражение `$filter` предназначено для отслеживания изменений в определенном объекте: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="f063b-138">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="f063b-139">Допускается фильтрация нескольких объектов.</span><span class="sxs-lookup"><span data-stu-id="f063b-139">You can filter multiple objects.</span></span> <span data-ttu-id="f063b-140">Например, `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="f063b-140">For example, `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="f063b-141">Максимальное количество фильтруемых объектов: 50.</span><span class="sxs-lookup"><span data-stu-id="f063b-141">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f063b-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f063b-142">Request headers</span></span>
| <span data-ttu-id="f063b-143">Имя</span><span class="sxs-lookup"><span data-stu-id="f063b-143">Name</span></span>       | <span data-ttu-id="f063b-144">Описание</span><span class="sxs-lookup"><span data-stu-id="f063b-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f063b-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="f063b-145">Authorization</span></span>  | <span data-ttu-id="f063b-146">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="f063b-146">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="f063b-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f063b-147">Content-Type</span></span>  | <span data-ttu-id="f063b-148">application/json</span><span class="sxs-lookup"><span data-stu-id="f063b-148">application/json</span></span> |
| <span data-ttu-id="f063b-149">Prefer</span><span class="sxs-lookup"><span data-stu-id="f063b-149">Prefer</span></span> | <span data-ttu-id="f063b-150">Возвращает = минимальный</span><span class="sxs-lookup"><span data-stu-id="f063b-150">return=minimal</span></span> <br><br><span data-ttu-id="f063b-151">Указание этот заголовок с запросом, который использует `deltaLink` возвращает свойства объекта, которые были изменены с момента последнего цикла.</span><span class="sxs-lookup"><span data-stu-id="f063b-151">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="f063b-152">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f063b-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f063b-153">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f063b-153">Request body</span></span>
<span data-ttu-id="f063b-154">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f063b-154">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="f063b-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="f063b-155">Response</span></span>

<span data-ttu-id="f063b-156">Успешно завершена, этот метод возвращает `200 OK` ответа [пользователя](../resources/user.md) и кода объект коллекции в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f063b-156">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="f063b-157">Ответ также включает `nextLink` URL-адрес или `deltaLink` URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="f063b-157">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="f063b-158">Если `nextLink` возвращается URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="f063b-158">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="f063b-159">Это означает, что существуют дополнительные страницы данных для получения в сеанс.</span><span class="sxs-lookup"><span data-stu-id="f063b-159">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="f063b-160">Приложение по-прежнему производится выполняете запросы, используя `nextLink` URL-адрес, пока не `deltaLink` URL-адрес включен в ответе.</span><span class="sxs-lookup"><span data-stu-id="f063b-160">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="f063b-161">Ответ включает тот же набор свойств, как и в запросе начальной дельты.</span><span class="sxs-lookup"><span data-stu-id="f063b-161">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="f063b-162">Это позволяет записывать полное текущего состояния объектов при начале цикла дельты.</span><span class="sxs-lookup"><span data-stu-id="f063b-162">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="f063b-163">Если `deltaLink` возвращается URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="f063b-163">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="f063b-164">Это означает, что нет дополнительных данных о состоянии существующих ресурсов должно быть возвращено.</span><span class="sxs-lookup"><span data-stu-id="f063b-164">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="f063b-165">Сохраните и использовать `deltaLink` URL-адрес, чтобы узнать о изменяется с ресурсом в следующего цикла.</span><span class="sxs-lookup"><span data-stu-id="f063b-165">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="f063b-166">У вас есть выбор для указания `Prefer:return=minimal` заголовок, чтобы включить в ответ значения для свойств, которые были изменены со времени `deltaLink` был отправлен.</span><span class="sxs-lookup"><span data-stu-id="f063b-166">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="f063b-167">Значение по умолчанию: возврата же свойства, что запрос на начальное дельты</span><span class="sxs-lookup"><span data-stu-id="f063b-167">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="f063b-168">По умолчанию, запросы с помощью `deltaLink` или `nextLink` возврата же свойства, что выбранный в запросе начальной дельты следующими способами:</span><span class="sxs-lookup"><span data-stu-id="f063b-168">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="f063b-169">При изменении свойства возвращает свойство в ответ JSON.</span><span class="sxs-lookup"><span data-stu-id="f063b-169">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="f063b-170">Если свойство значение пустое значение, возвращает значение свойства как значение null.</span><span class="sxs-lookup"><span data-stu-id="f063b-170">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="f063b-171">Если свойство не был изменен, возвратить значение null.</span><span class="sxs-lookup"><span data-stu-id="f063b-171">If the property has not changed, return the value as null.</span></span>

> <span data-ttu-id="f063b-172">**Примечание:** Выше поведение не возможно для различения свойства, который не был изменен и одного, которое было изменено на `null` значение.</span><span class="sxs-lookup"><span data-stu-id="f063b-172">**Note:** With the above behavior, it is not possible to differentiate between a property that has not changed and one that has changed to a `null` value.</span></span> <span data-ttu-id="f063b-173">В разделе [во втором примере](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="f063b-173">See the [second example](#request-2) below.</span></span> <span data-ttu-id="f063b-174">Если это важно, рекомендуется использовать альтернативный поведение, описанных в следующем разделе.</span><span class="sxs-lookup"><span data-stu-id="f063b-174">If this is important, we recommend using the alternative behavior described in the next section.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="f063b-175">Альтернатива: получить только измененные свойства</span><span class="sxs-lookup"><span data-stu-id="f063b-175">Alternative: return only the changed properties</span></span>

<span data-ttu-id="f063b-176">Добавление заголовка запроса на необязательный - `prefer:return=minimal` -приводит к следующим образом:</span><span class="sxs-lookup"><span data-stu-id="f063b-176">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="f063b-177">При изменении свойства возвращает свойство в ответ JSON.</span><span class="sxs-lookup"><span data-stu-id="f063b-177">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="f063b-178">Если свойство значение пустое значение, возвращает значение свойства как значение null.</span><span class="sxs-lookup"><span data-stu-id="f063b-178">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="f063b-179">Если свойство не был изменен, не включает свойство в ответ JSON.</span><span class="sxs-lookup"><span data-stu-id="f063b-179">If the property has not changed, do not include the property in the JSON response.</span></span> <span data-ttu-id="f063b-180">(Отличается от поведения по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="f063b-180">(Different from the default behavior.)</span></span>

> <span data-ttu-id="f063b-181">**Примечание:** Можно добавить заголовок `deltaLink` запроса в любой момент времени в цикле дельты.</span><span class="sxs-lookup"><span data-stu-id="f063b-181">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="f063b-182">Заголовок влияет только на набор свойств, включенных в ответ и не затрагивает как выполняется запрос дельты.</span><span class="sxs-lookup"><span data-stu-id="f063b-182">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="f063b-183">В разделе в [третьем примере](#request-3) ниже.</span><span class="sxs-lookup"><span data-stu-id="f063b-183">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="f063b-184">Пример</span><span class="sxs-lookup"><span data-stu-id="f063b-184">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="f063b-185">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="f063b-185">Request 1</span></span>

<span data-ttu-id="f063b-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f063b-186">The following is an example of the request.</span></span> <span data-ttu-id="f063b-187">Существует не `$select` параметр, поэтому по умолчанию набор свойств, отслеживаемых и возвращаются.</span><span class="sxs-lookup"><span data-stu-id="f063b-187">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="f063b-188">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="f063b-188">Response 1</span></span>

<span data-ttu-id="f063b-189">Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="f063b-189">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="f063b-p116">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f063b-p116">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "businessPhones": [
          "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

#### <a name="request-2"></a><span data-ttu-id="f063b-192">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="f063b-192">Request 2</span></span>

<span data-ttu-id="f063b-193">В следующем примере показаны начального запроса, выбрав пункт 3 свойства для отслеживания изменений, с ответ по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="f063b-193">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="f063b-194">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="f063b-194">Response 2</span></span>

<span data-ttu-id="f063b-195">Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="f063b-195">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="f063b-196">Обратите внимание, что `jobTitle` и `mobilePhone` имеет значение `null` это означает, что они могут не были изменены или были установлены пустое значение.</span><span class="sxs-lookup"><span data-stu-id="f063b-196">Note that `jobTitle` and `mobilePhone` have the value of `null` which means that they may have not changed or have been set to an empty value.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null,
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="f063b-197">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="f063b-197">Request 3</span></span>

<span data-ttu-id="f063b-198">В следующем примере показаны начального запроса, выбрав пункт 3 свойства для отслеживания изменений, поведение альтернативный минимальной ответа:</span><span class="sxs-lookup"><span data-stu-id="f063b-198">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="f063b-199">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="f063b-199">Response 3</span></span>

<span data-ttu-id="f063b-200">Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="f063b-200">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="f063b-201">Обратите внимание, что `mobilePhone` свойство не указан, то есть не был изменен с момента последнего разностного запроса; `displayName` и `jobTitle` включены, что означает их значения были изменены.</span><span class="sxs-lookup"><span data-stu-id="f063b-201">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```

- <span data-ttu-id="f063b-202">[Использование разностного запроса для отслеживания изменений в данных Microsoft Graph](../../../concepts/delta_query_overview.md).</span><span class="sxs-lookup"><span data-stu-id="f063b-202">[Use delta query to track changes in Microsoft Graph data](../../../concepts/delta_query_overview.md).</span></span>
- <span data-ttu-id="f063b-203">[Получение добавочные изменения для пользователей](../../../concepts/delta_query_users.md).</span><span class="sxs-lookup"><span data-stu-id="f063b-203">[Get incremental changes for users](../../../concepts/delta_query_users.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->