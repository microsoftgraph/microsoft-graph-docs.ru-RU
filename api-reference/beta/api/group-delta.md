---
title: 'group: delta'
description: Получите только что созданные, обновленные или удаленные группы, в том числе изменения членства в группах, без необходимости выполнять полный доступ ко всей коллекции групп. Сведения об использовании запроса изменений см.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: ff525bf807cf7f4d2932aad30f61dab157dc6619
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329721"
---
# <a name="group-delta"></a><span data-ttu-id="f58fb-104">group: delta</span><span class="sxs-lookup"><span data-stu-id="f58fb-104">group: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f58fb-105">Получите только что созданные, обновленные или удаленные группы, в том числе изменения членства в группах, без необходимости выполнять полный доступ ко всей коллекции групп.</span><span class="sxs-lookup"><span data-stu-id="f58fb-105">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="f58fb-106">Сведения об [использовании запроса изменений](/graph/delta-query-overview) см.</span><span class="sxs-lookup"><span data-stu-id="f58fb-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="f58fb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f58fb-107">Permissions</span></span>

<span data-ttu-id="f58fb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f58fb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f58fb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f58fb-110">Permission type</span></span>      | <span data-ttu-id="f58fb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f58fb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f58fb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f58fb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f58fb-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f58fb-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f58fb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f58fb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f58fb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f58fb-115">Not supported.</span></span>    |
|<span data-ttu-id="f58fb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f58fb-116">Application</span></span> | <span data-ttu-id="f58fb-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f58fb-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f58fb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f58fb-118">HTTP request</span></span>

<span data-ttu-id="f58fb-119">Чтобы начать отслеживать изменения, выполните запрос к ресурсу groups, включающий функцию delta.</span><span class="sxs-lookup"><span data-stu-id="f58fb-119">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="f58fb-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="f58fb-120">Query parameters</span></span>

<span data-ttu-id="f58fb-p104">Отслеживание изменений в группах запускает один или более циклов вызовов **разностной** функции. Если вы используете какой-либо параметр запроса (кроме `$deltatoken` и `$skiptoken`), вам необходимо указать его в исходном **разностном** запросе. Microsoft Graph автоматически кодирует любые указанные параметры в той части предоставленного в ответе URL-адреса `nextLink` или `deltaLink`, которая содержит токен.</span><span class="sxs-lookup"><span data-stu-id="f58fb-p104">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="f58fb-124">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="f58fb-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="f58fb-125">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="f58fb-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="f58fb-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="f58fb-126">Query parameter</span></span> | <span data-ttu-id="f58fb-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f58fb-127">Type</span></span>  |<span data-ttu-id="f58fb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f58fb-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f58fb-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="f58fb-129">$deltatoken</span></span> | <span data-ttu-id="f58fb-130">string</span><span class="sxs-lookup"><span data-stu-id="f58fb-130">string</span></span> | <span data-ttu-id="f58fb-p105">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции групп и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="f58fb-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="f58fb-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="f58fb-133">$skiptoken</span></span> | <span data-ttu-id="f58fb-134">строка</span><span class="sxs-lookup"><span data-stu-id="f58fb-134">string</span></span> | <span data-ttu-id="f58fb-135">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что из коллекции групп получены не все изменения.</span><span class="sxs-lookup"><span data-stu-id="f58fb-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="f58fb-136">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="f58fb-136">OData query parameters</span></span>

<span data-ttu-id="f58fb-137">Этот метод поддерживает необязательные параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f58fb-137">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="f58fb-p106">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство *id* возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="f58fb-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="f58fb-140">Вы можете использовать `$expand=members` для получения изменений в членстве.</span><span class="sxs-lookup"><span data-stu-id="f58fb-140">You can use `$expand=members` to get membership changes.</span></span>
- <span data-ttu-id="f58fb-141">Имеется ограниченная поддержка параметра `$filter`:</span><span class="sxs-lookup"><span data-stu-id="f58fb-141">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="f58fb-142">Единственное поддерживаемое выражение `$filter` предназначено для отслеживания изменений в определенном объекте: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="f58fb-142">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="f58fb-143">Допускается фильтрация нескольких объектов.</span><span class="sxs-lookup"><span data-stu-id="f58fb-143">You can filter multiple objects.</span></span> <span data-ttu-id="f58fb-144">Например, `https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="f58fb-144">For example, `https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="f58fb-145">Максимальное количество фильтруемых объектов: 50.</span><span class="sxs-lookup"><span data-stu-id="f58fb-145">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f58fb-146">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f58fb-146">Request headers</span></span>

| <span data-ttu-id="f58fb-147">Имя</span><span class="sxs-lookup"><span data-stu-id="f58fb-147">Name</span></span>       | <span data-ttu-id="f58fb-148">Описание</span><span class="sxs-lookup"><span data-stu-id="f58fb-148">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f58fb-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="f58fb-149">Authorization</span></span>  | <span data-ttu-id="f58fb-150">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="f58fb-150">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="f58fb-151">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f58fb-151">Content-Type</span></span>  | <span data-ttu-id="f58fb-152">application/json</span><span class="sxs-lookup"><span data-stu-id="f58fb-152">application/json</span></span> |
| <span data-ttu-id="f58fb-153">Prefer</span><span class="sxs-lookup"><span data-stu-id="f58fb-153">Prefer</span></span> | <span data-ttu-id="f58fb-154">return=minimal</span><span class="sxs-lookup"><span data-stu-id="f58fb-154">return=minimal</span></span> <br><br><span data-ttu-id="f58fb-155">Указание этого заголовка с запросом, использующим параметр `deltaLink`, приведет к возвращению только свойств объекта, измененных с момента последнего цикла.</span><span class="sxs-lookup"><span data-stu-id="f58fb-155">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="f58fb-156">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="f58fb-156">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f58fb-157">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f58fb-157">Request body</span></span>

<span data-ttu-id="f58fb-158">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f58fb-158">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="f58fb-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="f58fb-159">Response</span></span>

<span data-ttu-id="f58fb-160">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f58fb-160">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="f58fb-161">Ответ также включает маркер состояния, который является `nextLink` URL-адресом или `deltaLink` URL-адресом.</span><span class="sxs-lookup"><span data-stu-id="f58fb-161">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="f58fb-162">Если возвращается URL-адрес `nextLink`:</span><span class="sxs-lookup"><span data-stu-id="f58fb-162">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="f58fb-163">Это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="f58fb-163">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="f58fb-164">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в отклик не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="f58fb-164">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="f58fb-165">Отклик включает тот же набор свойств, что и начальный разностный запрос.</span><span class="sxs-lookup"><span data-stu-id="f58fb-165">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="f58fb-166">Это позволяет фиксировать полное текущее состояние объектов при запуске разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="f58fb-166">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="f58fb-167">Если возвращается URL-адрес `deltaLink`:</span><span class="sxs-lookup"><span data-stu-id="f58fb-167">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="f58fb-168">Это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="f58fb-168">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="f58fb-169">Сохраните и используйте URL-адрес `deltaLink`, чтобы узнавать об изменениях ресурса в следующем цикле.</span><span class="sxs-lookup"><span data-stu-id="f58fb-169">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="f58fb-170">Вы можете указать заголовок `Prefer:return=minimal`, чтобы включить в значения отклика только свойства, измененные с момента создания `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="f58fb-170">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="f58fb-171">По умолчанию: возвращение свойств, совпадающих с начальным разностным запросом</span><span class="sxs-lookup"><span data-stu-id="f58fb-171">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="f58fb-172">По умолчанию запросы с использованием `deltaLink` или `nextLink` возвращают те же свойства, которые выбраны в начальном разностном запросе, следующим образом:</span><span class="sxs-lookup"><span data-stu-id="f58fb-172">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="f58fb-173">Если свойство изменилось, в отклике содержится новое значение.</span><span class="sxs-lookup"><span data-stu-id="f58fb-173">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="f58fb-174">Сюда включаются свойства с заданным значением NULL.</span><span class="sxs-lookup"><span data-stu-id="f58fb-174">This includes properties being set to null value.</span></span>
- <span data-ttu-id="f58fb-175">Если свойство не изменилось, в отклике содержится старое значение.</span><span class="sxs-lookup"><span data-stu-id="f58fb-175">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="f58fb-176">Если свойство ранее никогда не настраивалось, оно не включается в отклик.</span><span class="sxs-lookup"><span data-stu-id="f58fb-176">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="f58fb-177">**Примечание.** При таком поведении просмотр отклика не дает возможность определить, изменилось ли свойство.</span><span class="sxs-lookup"><span data-stu-id="f58fb-177">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="f58fb-178">Кроме того, разностные отклики отличаются большими размерами, так как они содержат все значения свойств, как показано [во втором примере](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="f58fb-178">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="f58fb-179">Альтернатива: возвращение только измененных свойств</span><span class="sxs-lookup"><span data-stu-id="f58fb-179">Alternative: return only the changed properties</span></span>

<span data-ttu-id="f58fb-180">Добавление необязательного заголовка запроса `prefer:return=minimal` приводит к следующему результату:</span><span class="sxs-lookup"><span data-stu-id="f58fb-180">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="f58fb-181">Если свойство изменилось, в отклике содержится новое значение.</span><span class="sxs-lookup"><span data-stu-id="f58fb-181">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="f58fb-182">Сюда включаются свойства с заданным значением NULL.</span><span class="sxs-lookup"><span data-stu-id="f58fb-182">This includes properties being set to null value.</span></span>
- <span data-ttu-id="f58fb-183">Если свойство не изменилось, оно не включается в отклик.</span><span class="sxs-lookup"><span data-stu-id="f58fb-183">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="f58fb-184">(Отличается от поведения по умолчанию.)</span><span class="sxs-lookup"><span data-stu-id="f58fb-184">(Different from the default behavior.)</span></span>

> <span data-ttu-id="f58fb-185">**Примечание.** Заголовок можно добавить в запрос `deltaLink` в любой момент разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="f58fb-185">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="f58fb-186">Заголовок влияет только на набор свойств, включенный в отклик, и не влияет на способ выполнения разностного запроса.</span><span class="sxs-lookup"><span data-stu-id="f58fb-186">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="f58fb-187">См. [третий пример](#request-3) ниже.</span><span class="sxs-lookup"><span data-stu-id="f58fb-187">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="f58fb-188">Пример</span><span class="sxs-lookup"><span data-stu-id="f58fb-188">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="f58fb-189">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="f58fb-189">Request 1</span></span>

<span data-ttu-id="f58fb-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f58fb-190">The following is an example of the request.</span></span> <span data-ttu-id="f58fb-191">Параметр `$select` отсутствует, поэтому отслеживается и возвращается набор свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f58fb-191">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta
```

#### <a name="response-1"></a><span data-ttu-id="f58fb-192">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="f58fb-192">Response 1</span></span>

<span data-ttu-id="f58fb-193">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="f58fb-193">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="f58fb-194">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f58fb-194">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f58fb-195">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f58fb-195">All the properties will be returned from an actual call.</span></span>
>
> <span data-ttu-id="f58fb-196">Обратите внимание на присутствие свойства *Members @ Delta* , которое включает идентификаторы объектов Member в группе.</span><span class="sxs-lookup"><span data-stu-id="f58fb-196">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="f58fb-197">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="f58fb-197">Request 2</span></span>

<span data-ttu-id="f58fb-198">В следующем примере показан исходный запрос с выбором 3 свойств для отслеживания изменений с поведением отклика по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="f58fb-198">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a><span data-ttu-id="f58fb-199">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="f58fb-199">Response 2</span></span>

<span data-ttu-id="f58fb-200">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="f58fb-200">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="f58fb-201">Обратите внимание, что все 3 свойства включаются в отклик, и неизвестно, какие из них изменились с момента получения `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="f58fb-201">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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

#### <a name="request-3"></a><span data-ttu-id="f58fb-202">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="f58fb-202">Request 3</span></span>

<span data-ttu-id="f58fb-203">В следующем примере показан исходный запрос с выбором 3 свойств для отслеживания изменений с альтернативным поведением отклика с минимальными результатами:</span><span class="sxs-lookup"><span data-stu-id="f58fb-203">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="f58fb-204">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="f58fb-204">Response 3</span></span>

<span data-ttu-id="f58fb-205">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="f58fb-205">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="f58fb-206">Обратите внимание, что свойство `mailNickname` не включено, то есть оно не изменилось с последнего разностного запроса; `displayName` и `description` включены, то есть их значения изменились.</span><span class="sxs-lookup"><span data-stu-id="f58fb-206">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="f58fb-207">См. также</span><span class="sxs-lookup"><span data-stu-id="f58fb-207">See also</span></span>

- <span data-ttu-id="f58fb-208">[Отслеживание изменений в данных Microsoft Graph с помощью разностного запроса](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="f58fb-208">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="f58fb-209">[Получение добавочных изменений для групп](/graph/delta-query-groups).</span><span class="sxs-lookup"><span data-stu-id="f58fb-209">[Get incremental changes for groups](/graph/delta-query-groups).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
