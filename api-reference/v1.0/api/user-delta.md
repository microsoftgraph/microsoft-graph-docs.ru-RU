---
title: 'user: delta'
description: Get вновь созданных, обновлении или удалении пользователей без необходимости выполнять полное чтение коллекции всей пользователя. Отслеживание изменений для получения дополнительных сведений см.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6464e8ad975a5fc996c671df5a01df2988dbf79d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945617"
---
# <a name="user-delta"></a><span data-ttu-id="c41f7-104">user: delta</span><span class="sxs-lookup"><span data-stu-id="c41f7-104">user: delta</span></span>

<span data-ttu-id="c41f7-105">Get вновь созданных, обновлении или удалении пользователей без необходимости выполнять полное чтение коллекции всей пользователя.</span><span class="sxs-lookup"><span data-stu-id="c41f7-105">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="c41f7-106">Дополнительные сведения см [Отслеживание изменений](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="c41f7-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="c41f7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c41f7-107">Permissions</span></span>

<span data-ttu-id="c41f7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c41f7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c41f7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c41f7-110">Permission type</span></span>      | <span data-ttu-id="c41f7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c41f7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c41f7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c41f7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c41f7-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c41f7-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c41f7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c41f7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c41f7-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c41f7-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="c41f7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c41f7-116">Application</span></span> | <span data-ttu-id="c41f7-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c41f7-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c41f7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c41f7-118">HTTP request</span></span>

<span data-ttu-id="c41f7-119">Чтобы начать отслеживать изменения, выполните запрос к ресурсу users, включающий функцию delta.</span><span class="sxs-lookup"><span data-stu-id="c41f7-119">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="c41f7-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="c41f7-120">Query parameters</span></span>

<span data-ttu-id="c41f7-121">Отслеживание изменений в пользователи могут возникать round один или несколько вызовов функций **дельты** .</span><span class="sxs-lookup"><span data-stu-id="c41f7-121">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="c41f7-122">При использовании любого параметра запроса (отличный от `$deltatoken` и `$skiptoken`), необходимо указать его в запрос начальной **дельты** .</span><span class="sxs-lookup"><span data-stu-id="c41f7-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="c41f7-123">Microsoft Graph автоматически Кодирует указанный параметров в маркеров часть `nextLink` или `deltaLink` URL-адреса, приведенные в ответе.</span><span class="sxs-lookup"><span data-stu-id="c41f7-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="c41f7-124">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="c41f7-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="c41f7-125">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="c41f7-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="c41f7-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="c41f7-126">Query parameter</span></span>      | <span data-ttu-id="c41f7-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c41f7-127">Type</span></span>   |<span data-ttu-id="c41f7-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c41f7-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c41f7-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="c41f7-129">$deltatoken</span></span> | <span data-ttu-id="c41f7-130">строка</span><span class="sxs-lookup"><span data-stu-id="c41f7-130">string</span></span> | <span data-ttu-id="c41f7-p105">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции пользователей и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="c41f7-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="c41f7-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="c41f7-133">$skiptoken</span></span> | <span data-ttu-id="c41f7-134">строка</span><span class="sxs-lookup"><span data-stu-id="c41f7-134">string</span></span> | <span data-ttu-id="c41f7-135">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что в коллекции пользователей остаются неотслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="c41f7-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="c41f7-136">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="c41f7-136">OData query parameters</span></span>

<span data-ttu-id="c41f7-137">Этот метод поддерживает дополнительные параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c41f7-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="c41f7-p106">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство *id* возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="c41f7-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="c41f7-140">Ограниченная поддержка `$filter`:</span><span class="sxs-lookup"><span data-stu-id="c41f7-140">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="c41f7-141">Единственное поддерживаемое выражение `$filter` предназначено для отслеживания изменений в определенном объекте: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="c41f7-141">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="c41f7-142">Допускается фильтрация нескольких объектов.</span><span class="sxs-lookup"><span data-stu-id="c41f7-142">You can filter multiple objects.</span></span> <span data-ttu-id="c41f7-143">Например, `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="c41f7-143">For example, `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="c41f7-144">Максимальное количество фильтруемых объектов: 50.</span><span class="sxs-lookup"><span data-stu-id="c41f7-144">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c41f7-145">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c41f7-145">Request headers</span></span>
| <span data-ttu-id="c41f7-146">Имя</span><span class="sxs-lookup"><span data-stu-id="c41f7-146">Name</span></span>       | <span data-ttu-id="c41f7-147">Описание</span><span class="sxs-lookup"><span data-stu-id="c41f7-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c41f7-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="c41f7-148">Authorization</span></span>  | <span data-ttu-id="c41f7-149">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="c41f7-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="c41f7-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c41f7-150">Content-Type</span></span>  | <span data-ttu-id="c41f7-151">application/json</span><span class="sxs-lookup"><span data-stu-id="c41f7-151">application/json</span></span> |
| <span data-ttu-id="c41f7-152">Prefer</span><span class="sxs-lookup"><span data-stu-id="c41f7-152">Prefer</span></span> | <span data-ttu-id="c41f7-153">Возвращает = минимальный</span><span class="sxs-lookup"><span data-stu-id="c41f7-153">return=minimal</span></span> <br><br><span data-ttu-id="c41f7-154">Указание этот заголовок с запросом, который использует `deltaLink` возвращает свойства объекта, которые были изменены с момента последнего цикла.</span><span class="sxs-lookup"><span data-stu-id="c41f7-154">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="c41f7-155">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c41f7-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c41f7-156">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c41f7-156">Request body</span></span>
<span data-ttu-id="c41f7-157">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c41f7-157">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="c41f7-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="c41f7-158">Response</span></span>

<span data-ttu-id="c41f7-159">Успешно завершена, этот метод возвращает `200 OK` ответа [пользователя](../resources/user.md) и кода объект коллекции в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c41f7-159">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="c41f7-160">Ответ также включает `nextLink` URL-адрес или `deltaLink` URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="c41f7-160">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="c41f7-161">Если `nextLink` возвращается URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="c41f7-161">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="c41f7-162">Это означает, что существуют дополнительные страницы данных для получения в сеанс.</span><span class="sxs-lookup"><span data-stu-id="c41f7-162">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="c41f7-163">Приложение по-прежнему производится выполняете запросы, используя `nextLink` URL-адрес, пока не `deltaLink` URL-адрес включен в ответе.</span><span class="sxs-lookup"><span data-stu-id="c41f7-163">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="c41f7-164">Ответ включает тот же набор свойств, как и в запросе начальной дельты.</span><span class="sxs-lookup"><span data-stu-id="c41f7-164">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="c41f7-165">Это позволяет записывать полное текущего состояния объектов при начале цикла дельты.</span><span class="sxs-lookup"><span data-stu-id="c41f7-165">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="c41f7-166">Если `deltaLink` возвращается URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="c41f7-166">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="c41f7-167">Это означает, что нет дополнительных данных о состоянии существующих ресурсов должно быть возвращено.</span><span class="sxs-lookup"><span data-stu-id="c41f7-167">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="c41f7-168">Сохраните и использовать `deltaLink` URL-адрес, чтобы узнать о изменяется с ресурсом в следующего цикла.</span><span class="sxs-lookup"><span data-stu-id="c41f7-168">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="c41f7-169">У вас есть выбор для указания `Prefer:return=minimal` заголовок, чтобы включить в ответ значения для свойств, которые были изменены со времени `deltaLink` был отправлен.</span><span class="sxs-lookup"><span data-stu-id="c41f7-169">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="c41f7-170">Значение по умолчанию: возврата же свойства, что запрос на начальное дельты</span><span class="sxs-lookup"><span data-stu-id="c41f7-170">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="c41f7-171">По умолчанию, запросы с помощью `deltaLink` или `nextLink` возврата же свойства, что выбранный в запросе начальной дельты следующими способами:</span><span class="sxs-lookup"><span data-stu-id="c41f7-171">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="c41f7-172">При изменении свойства новое значение включается в ответе.</span><span class="sxs-lookup"><span data-stu-id="c41f7-172">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="c41f7-173">Этот компонент включает свойства задаются на значение null.</span><span class="sxs-lookup"><span data-stu-id="c41f7-173">This includes properties being set to null value.</span></span>
- <span data-ttu-id="c41f7-174">Если свойство не был изменен, старое значение включается в ответе.</span><span class="sxs-lookup"><span data-stu-id="c41f7-174">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="c41f7-175">Если свойство имеет значение никогда не перед его не будут включены в ответе на всех.</span><span class="sxs-lookup"><span data-stu-id="c41f7-175">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="c41f7-176">**Примечание:** С помощью этого поведения, посмотрев ответа не позволяет определить, будет ли свойство изменяется, или не.</span><span class="sxs-lookup"><span data-stu-id="c41f7-176">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="c41f7-177">Кроме того ответы дельты, как правило больших так как они содержат все значения свойств - как показано в следующем [примере второй](#request-2) .</span><span class="sxs-lookup"><span data-stu-id="c41f7-177">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="c41f7-178">Альтернатива: получить только измененные свойства</span><span class="sxs-lookup"><span data-stu-id="c41f7-178">Alternative: return only the changed properties</span></span>

<span data-ttu-id="c41f7-179">Добавление заголовка запроса на необязательный - `prefer:return=minimal` -приводит к следующим образом:</span><span class="sxs-lookup"><span data-stu-id="c41f7-179">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="c41f7-180">При изменении свойства новое значение включается в ответе.</span><span class="sxs-lookup"><span data-stu-id="c41f7-180">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="c41f7-181">Этот компонент включает свойства задаются на значение null.</span><span class="sxs-lookup"><span data-stu-id="c41f7-181">This includes properties being set to null value.</span></span>
- <span data-ttu-id="c41f7-182">Если свойство не был изменен, свойство не включается в ответ на всех.</span><span class="sxs-lookup"><span data-stu-id="c41f7-182">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="c41f7-183">(Отличается от поведения по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="c41f7-183">(Different from the default behavior.)</span></span>

> <span data-ttu-id="c41f7-184">**Примечание:** Можно добавить заголовок `deltaLink` запроса в любой момент времени в цикле дельты.</span><span class="sxs-lookup"><span data-stu-id="c41f7-184">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="c41f7-185">Заголовок влияет только на набор свойств, включенных в ответ и не затрагивает как выполняется запрос дельты.</span><span class="sxs-lookup"><span data-stu-id="c41f7-185">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="c41f7-186">В разделе в [третьем примере](#request-3) ниже.</span><span class="sxs-lookup"><span data-stu-id="c41f7-186">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="c41f7-187">Пример</span><span class="sxs-lookup"><span data-stu-id="c41f7-187">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="c41f7-188">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="c41f7-188">Request 1</span></span>

<span data-ttu-id="c41f7-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c41f7-189">The following is an example of the request.</span></span> <span data-ttu-id="c41f7-190">Существует не `$select` параметр, поэтому по умолчанию набор свойств, отслеживаемых и возвращаются.</span><span class="sxs-lookup"><span data-stu-id="c41f7-190">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="c41f7-191">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="c41f7-191">Response 1</span></span>

<span data-ttu-id="c41f7-192">Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="c41f7-192">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="c41f7-p119">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c41f7-p119">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="c41f7-195">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="c41f7-195">Request 2</span></span>

<span data-ttu-id="c41f7-196">В следующем примере показаны начального запроса, выбрав пункт 3 свойства для отслеживания изменений, с ответ по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="c41f7-196">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="c41f7-197">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="c41f7-197">Response 2</span></span>

<span data-ttu-id="c41f7-198">Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="c41f7-198">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="c41f7-199">Обратите внимание на то, что все свойства 3 включенных в ответ и не известно, какие из них были изменены с момента `deltaLink` был получен.</span><span class="sxs-lookup"><span data-stu-id="c41f7-199">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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
      "jobTitle": "jobTitle-value",
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="c41f7-200">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="c41f7-200">Request 3</span></span>

<span data-ttu-id="c41f7-201">В следующем примере показаны начального запроса, выбрав пункт 3 свойства для отслеживания изменений, поведение альтернативный минимальной ответа:</span><span class="sxs-lookup"><span data-stu-id="c41f7-201">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="c41f7-202">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="c41f7-202">Response 3</span></span>

<span data-ttu-id="c41f7-203">Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="c41f7-203">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="c41f7-204">Обратите внимание, что `mobilePhone` свойство не указан, то есть не был изменен с момента последнего разностного запроса; `displayName` и `jobTitle` включены, что означает их значения были изменены.</span><span class="sxs-lookup"><span data-stu-id="c41f7-204">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

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

- <span data-ttu-id="c41f7-205">[Использование разностного запроса для отслеживания изменений в данных Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="c41f7-205">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="c41f7-206">[Получение добавочные изменения для пользователей](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="c41f7-206">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
