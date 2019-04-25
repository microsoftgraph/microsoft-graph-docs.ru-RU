---
title: 'group: delta'
description: Получите только что созданные, обновленные или удаленные группы, в том числе изменения членства в группах, без необходимости выполнять полный доступ ко всей коллекции групп. Сведения об использовании запроса изменений см.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 344b9745a998dcfb1107a1af72691184732718b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522603"
---
# <a name="group-delta"></a><span data-ttu-id="49873-104">group: delta</span><span class="sxs-lookup"><span data-stu-id="49873-104">group: delta</span></span>
<span data-ttu-id="49873-105">Получите только что созданные, обновленные или удаленные группы, в том числе изменения членства в группах, без необходимости выполнять полный доступ ко всей коллекции групп.</span><span class="sxs-lookup"><span data-stu-id="49873-105">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="49873-106">Сведения об [использовании запроса изменений](/graph/delta-query-overview) см.</span><span class="sxs-lookup"><span data-stu-id="49873-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="49873-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49873-107">Permissions</span></span>

<span data-ttu-id="49873-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49873-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49873-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49873-110">Permission type</span></span>      | <span data-ttu-id="49873-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49873-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49873-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49873-112">Delegated (work or school account)</span></span> | <span data-ttu-id="49873-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49873-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="49873-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49873-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49873-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49873-115">Not supported.</span></span>    |
|<span data-ttu-id="49873-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49873-116">Application</span></span> | <span data-ttu-id="49873-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49873-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49873-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49873-118">HTTP request</span></span>

<span data-ttu-id="49873-119">Чтобы начать отслеживать изменения, выполните запрос к ресурсу groups, включающий функцию delta.</span><span class="sxs-lookup"><span data-stu-id="49873-119">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="49873-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="49873-120">Query parameters</span></span>

<span data-ttu-id="49873-p104">Отслеживание изменений в группах запускает один или более циклов вызовов **разностной** функции. Если вы используете какой-либо параметр запроса (кроме `$deltatoken` и `$skiptoken`), вам необходимо указать его в исходном **разностном** запросе. Microsoft Graph автоматически кодирует любые указанные параметры в той части предоставленного в ответе URL-адреса `nextLink` или `deltaLink`, которая содержит токен.</span><span class="sxs-lookup"><span data-stu-id="49873-p104">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="49873-124">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="49873-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="49873-125">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="49873-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="49873-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="49873-126">Query parameter</span></span> | <span data-ttu-id="49873-127">Тип</span><span class="sxs-lookup"><span data-stu-id="49873-127">Type</span></span>  |<span data-ttu-id="49873-128">Описание</span><span class="sxs-lookup"><span data-stu-id="49873-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="49873-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="49873-129">$deltatoken</span></span> | <span data-ttu-id="49873-130">string</span><span class="sxs-lookup"><span data-stu-id="49873-130">string</span></span> | <span data-ttu-id="49873-p105">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции групп и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="49873-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="49873-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="49873-133">$skiptoken</span></span> | <span data-ttu-id="49873-134">строка</span><span class="sxs-lookup"><span data-stu-id="49873-134">string</span></span> | <span data-ttu-id="49873-135">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что из коллекции групп получены не все изменения.</span><span class="sxs-lookup"><span data-stu-id="49873-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="49873-136">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="49873-136">OData query parameters</span></span>

<span data-ttu-id="49873-137">Этот метод поддерживает необязательные параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="49873-137">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="49873-p106">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство *id* возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="49873-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="49873-140">Вы можете использовать `$expand=members` для получения изменений в членстве.</span><span class="sxs-lookup"><span data-stu-id="49873-140">You can use `$expand=members` to get membership changes.</span></span>
- <span data-ttu-id="49873-141">Существует ограниченная поддержка `$filter`:</span><span class="sxs-lookup"><span data-stu-id="49873-141">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="49873-142">Единственное поддерживаемое выражение `$filter` предназначено для отслеживания изменений в определенном объекте: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="49873-142">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="49873-143">Допускается фильтрация нескольких объектов.</span><span class="sxs-lookup"><span data-stu-id="49873-143">You can filter multiple objects.</span></span> <span data-ttu-id="49873-144">Например, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="49873-144">For example, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="49873-145">Максимальное количество фильтруемых объектов: 50.</span><span class="sxs-lookup"><span data-stu-id="49873-145">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49873-146">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49873-146">Request headers</span></span>

| <span data-ttu-id="49873-147">Имя</span><span class="sxs-lookup"><span data-stu-id="49873-147">Name</span></span>       | <span data-ttu-id="49873-148">Описание</span><span class="sxs-lookup"><span data-stu-id="49873-148">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="49873-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="49873-149">Authorization</span></span>  | <span data-ttu-id="49873-150">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="49873-150">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="49873-151">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49873-151">Content-Type</span></span>  | <span data-ttu-id="49873-152">application/json</span><span class="sxs-lookup"><span data-stu-id="49873-152">application/json</span></span> |
| <span data-ttu-id="49873-153">Prefer</span><span class="sxs-lookup"><span data-stu-id="49873-153">Prefer</span></span> | <span data-ttu-id="49873-154">Возврат = минимум</span><span class="sxs-lookup"><span data-stu-id="49873-154">return=minimal</span></span> <br><br><span data-ttu-id="49873-155">При указании заголовка с запросом, который `deltaLink` использует объект, возвращаются только свойства объекта, которые были изменены с момента последнего цикла.</span><span class="sxs-lookup"><span data-stu-id="49873-155">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="49873-156">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="49873-156">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49873-157">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49873-157">Request body</span></span>

<span data-ttu-id="49873-158">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49873-158">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="49873-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="49873-159">Response</span></span>

<span data-ttu-id="49873-160">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49873-160">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="49873-161">Ответ также включает маркер состояния, который является `nextLink` URL-адресом или `deltaLink` URL-адресом.</span><span class="sxs-lookup"><span data-stu-id="49873-161">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="49873-162">Если возвращается `nextLink` URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="49873-162">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="49873-163">Это указывает на необходимость извлечения дополнительных страниц данных в сеансе.</span><span class="sxs-lookup"><span data-stu-id="49873-163">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="49873-164">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="49873-164">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="49873-165">Ответ включает тот же набор свойств, что и в исходном запросе на разностный запрос.</span><span class="sxs-lookup"><span data-stu-id="49873-165">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="49873-166">Это позволяет захватить полное текущее состояние объектов при инициации разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="49873-166">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="49873-167">Если возвращается `deltaLink` URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="49873-167">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="49873-168">Это указывает на то, что больше нет данных о существующем состоянии ресурса, который необходимо возвратить.</span><span class="sxs-lookup"><span data-stu-id="49873-168">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="49873-169">Сохраните и используйте `deltaLink` URL-адрес, чтобы узнать об изменениях ресурса в следующем цикле.</span><span class="sxs-lookup"><span data-stu-id="49873-169">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="49873-170">Вы можете указать `Prefer:return=minimal` заголовок, чтобы включить в значения отклика только те свойства, которые были изменены с момента `deltaLink` выпуска.</span><span class="sxs-lookup"><span data-stu-id="49873-170">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="49873-171">По умолчанию: возврат тех же свойств, что и исходный запрос Дельта</span><span class="sxs-lookup"><span data-stu-id="49873-171">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="49873-172">По умолчанию запросы, использующие `deltaLink` или `nextLink` возвращающие те же свойства, что и выбранные в начальном запросе Дельта, запрашиваются следующими способами:</span><span class="sxs-lookup"><span data-stu-id="49873-172">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="49873-173">Если свойство изменилось, в ответ включается новое значение.</span><span class="sxs-lookup"><span data-stu-id="49873-173">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="49873-174">Сюда входят свойства, для которых задано значение null.</span><span class="sxs-lookup"><span data-stu-id="49873-174">This includes properties being set to null value.</span></span>
- <span data-ttu-id="49873-175">Если свойство не изменилось, в ответ включается старое значение.</span><span class="sxs-lookup"><span data-stu-id="49873-175">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="49873-176">Если свойство никогда не задается до тех пор, пока оно не будет включено в ответ вообще.</span><span class="sxs-lookup"><span data-stu-id="49873-176">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="49873-177">**Примечание:** Таким образом, изучив ответ, можно определить, изменяется ли свойство.</span><span class="sxs-lookup"><span data-stu-id="49873-177">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="49873-178">Кроме того, разностные ответы обычно имеют большой размер, так как они содержат все значения свойств, как показано во [втором примере](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="49873-178">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="49873-179">Альтернатива: возврат только измененных свойств</span><span class="sxs-lookup"><span data-stu-id="49873-179">Alternative: return only the changed properties</span></span>

<span data-ttu-id="49873-180">Добавление необязательного заголовка запроса `prefer:return=minimal` — приводит к следующему поведению:</span><span class="sxs-lookup"><span data-stu-id="49873-180">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="49873-181">Если свойство изменилось, в ответ включается новое значение.</span><span class="sxs-lookup"><span data-stu-id="49873-181">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="49873-182">Сюда входят свойства, для которых задано значение null.</span><span class="sxs-lookup"><span data-stu-id="49873-182">This includes properties being set to null value.</span></span>
- <span data-ttu-id="49873-183">Если свойство не изменилось, свойство не включается в ответ вообще.</span><span class="sxs-lookup"><span data-stu-id="49873-183">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="49873-184">(Отличается от поведения по умолчанию.)</span><span class="sxs-lookup"><span data-stu-id="49873-184">(Different from the default behavior.)</span></span>

> <span data-ttu-id="49873-185">**Примечание:** Заголовок можно добавить в `deltaLink` запрос в любой момент времени в разностном цикле.</span><span class="sxs-lookup"><span data-stu-id="49873-185">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="49873-186">Заголовок влияет только на набор свойств, включенных в ответ, и не влияет на то, как выполняется разностный запрос.</span><span class="sxs-lookup"><span data-stu-id="49873-186">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="49873-187">Просмотрите [третий пример](#request-3) ниже.</span><span class="sxs-lookup"><span data-stu-id="49873-187">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="49873-188">Пример</span><span class="sxs-lookup"><span data-stu-id="49873-188">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="49873-189">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="49873-189">Request 1</span></span>

<span data-ttu-id="49873-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49873-190">The following is an example of the request.</span></span> <span data-ttu-id="49873-191">Параметр не `$select` задан, поэтому набор свойств по умолчанию отслеживается и возвращается.</span><span class="sxs-lookup"><span data-stu-id="49873-191">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response-1"></a><span data-ttu-id="49873-192">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="49873-192">Response 1</span></span>

<span data-ttu-id="49873-193">Ниже приведен пример ответа, полученного при использовании метода `deltaLink` , полученного при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="49873-193">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="49873-194">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="49873-194">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="49873-195">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49873-195">All the properties will be returned from an actual call.</span></span>
>
> <span data-ttu-id="49873-196">Обратите внимание на присутствие свойства *Members @ Delta* , которое включает идентификаторы объектов Member в группе.</span><span class="sxs-lookup"><span data-stu-id="49873-196">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="49873-197">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="49873-197">Request 2</span></span>

<span data-ttu-id="49873-198">В следующем примере показан первоначальный запрос, в котором выбирается 3 свойства для отслеживания изменений с поведением ответа по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="49873-198">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a><span data-ttu-id="49873-199">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="49873-199">Response 2</span></span>

<span data-ttu-id="49873-200">Ниже приведен пример ответа, полученного при использовании метода `deltaLink` , полученного при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="49873-200">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="49873-201">Обратите внимание на то, что в ответ включены все 3 свойства, и они не известны, какие из `deltaLink` них были изменены с момента получения.</span><span class="sxs-lookup"><span data-stu-id="49873-201">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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
      "mailNickname": "mailNickname-value"
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="49873-202">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="49873-202">Request 3</span></span>

<span data-ttu-id="49873-203">В следующем примере показано, как исходный запрос выбирает 3 свойства для отслеживания изменений с альтернативным поведением минимального ответа:</span><span class="sxs-lookup"><span data-stu-id="49873-203">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="49873-204">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="49873-204">Response 3</span></span>

<span data-ttu-id="49873-205">Ниже приведен пример ответа, полученного при использовании метода `deltaLink` , полученного при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="49873-205">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="49873-206">Обратите внимание `mailNickname` , что свойство не включается, что означает, что он не изменился с момента последнего запроса Дельта; `displayName` и `description` включены, что означает, что их значения изменились.</span><span class="sxs-lookup"><span data-stu-id="49873-206">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="49873-207">См. также</span><span class="sxs-lookup"><span data-stu-id="49873-207">See also</span></span>

- <span data-ttu-id="49873-208">[Использование запроса изменений для отслеживания изменений в данных Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="49873-208">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="49873-209">[Получение добавочных изменений для групп](/graph/delta-query-groups).</span><span class="sxs-lookup"><span data-stu-id="49873-209">[Get incremental changes for groups](/graph/delta-query-groups).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
