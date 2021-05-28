---
title: 'group: delta'
description: Создайте новые, обновленные или удаленные группы, в том числе изменения членства в группе, без необходимости выполнять полное чтение всей коллекции групп.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a3acfecc8f005c6468dfe681ff3410bf7a4ffbfe
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680978"
---
# <a name="group-delta"></a><span data-ttu-id="41218-103">group: delta</span><span class="sxs-lookup"><span data-stu-id="41218-103">group: delta</span></span>

<span data-ttu-id="41218-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41218-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41218-105">Создайте новые, обновленные или удаленные группы, в том числе изменения членства в группе, без необходимости выполнять полное чтение всей коллекции групп.</span><span class="sxs-lookup"><span data-stu-id="41218-105">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="41218-106">Подробные [сведения см. в материале Использование запроса Delta.](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="41218-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="41218-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41218-107">Permissions</span></span>

<span data-ttu-id="41218-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41218-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41218-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41218-110">Permission type</span></span>      | <span data-ttu-id="41218-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41218-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41218-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41218-112">Delegated (work or school account)</span></span> | <span data-ttu-id="41218-113">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="41218-113">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="41218-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41218-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41218-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41218-115">Not supported.</span></span>    |
|<span data-ttu-id="41218-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41218-116">Application</span></span> | <span data-ttu-id="41218-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41218-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41218-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41218-118">HTTP request</span></span>

<span data-ttu-id="41218-119">Чтобы начать отслеживать изменения, выполните запрос к ресурсу groups, включающий функцию delta.</span><span class="sxs-lookup"><span data-stu-id="41218-119">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="41218-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="41218-120">Query parameters</span></span>

<span data-ttu-id="41218-p103">Отслеживание изменений в группах запускает один или более циклов вызовов **разностной** функции. Если вы используете какой-либо параметр запроса (кроме `$deltatoken` и `$skiptoken`), вам необходимо указать его в исходном **разностном** запросе. Microsoft Graph автоматически кодирует любые указанные параметры в той части предоставленного в ответе URL-адреса `nextLink` или `deltaLink`, которая содержит токен.</span><span class="sxs-lookup"><span data-stu-id="41218-p103">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="41218-124">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="41218-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="41218-125">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="41218-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="41218-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="41218-126">Query parameter</span></span> | <span data-ttu-id="41218-127">Тип</span><span class="sxs-lookup"><span data-stu-id="41218-127">Type</span></span>  |<span data-ttu-id="41218-128">Описание</span><span class="sxs-lookup"><span data-stu-id="41218-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="41218-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="41218-129">$deltatoken</span></span> | <span data-ttu-id="41218-130">string</span><span class="sxs-lookup"><span data-stu-id="41218-130">string</span></span> | <span data-ttu-id="41218-p104">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции групп и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="41218-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="41218-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="41218-133">$skiptoken</span></span> | <span data-ttu-id="41218-134">string</span><span class="sxs-lookup"><span data-stu-id="41218-134">string</span></span> | <span data-ttu-id="41218-135">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что из коллекции групп получены не все изменения.</span><span class="sxs-lookup"><span data-stu-id="41218-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="41218-136">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="41218-136">OData query parameters</span></span>

<span data-ttu-id="41218-137">Этот метод поддерживает необязательные параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="41218-137">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="41218-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство *id* возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="41218-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="41218-140">Вы можете использовать `$select=members` для получения изменений членства.</span><span class="sxs-lookup"><span data-stu-id="41218-140">You can use `$select=members` to get membership changes.</span></span> <span data-ttu-id="41218-141">Вы можете дополнительно отслеживать другие изменения, такие [](../resources/group.md#relationships) как владение и другие, выбрав любые групповые отношения коллекции **типов directoryObject.**</span><span class="sxs-lookup"><span data-stu-id="41218-141">You can additionally track other changes like ownership and more by selecting any [group relationship](../resources/group.md#relationships) of type **directoryObject collection**.</span></span>
- <span data-ttu-id="41218-142">Имеется ограниченная поддержка параметра `$filter`:</span><span class="sxs-lookup"><span data-stu-id="41218-142">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="41218-143">Единственное поддерживаемое выражение `$filter` предназначено для отслеживания изменений в определенном объекте: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="41218-143">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="41218-144">Допускается фильтрация нескольких объектов.</span><span class="sxs-lookup"><span data-stu-id="41218-144">You can filter multiple objects.</span></span> <span data-ttu-id="41218-145">Например, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="41218-145">For example, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="41218-146">Максимальное количество фильтруемых объектов: 50.</span><span class="sxs-lookup"><span data-stu-id="41218-146">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41218-147">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41218-147">Request headers</span></span>

| <span data-ttu-id="41218-148">Имя</span><span class="sxs-lookup"><span data-stu-id="41218-148">Name</span></span>       | <span data-ttu-id="41218-149">Описание</span><span class="sxs-lookup"><span data-stu-id="41218-149">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="41218-150">Authorization</span><span class="sxs-lookup"><span data-stu-id="41218-150">Authorization</span></span>  | <span data-ttu-id="41218-151">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="41218-151">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="41218-152">Content-Type</span><span class="sxs-lookup"><span data-stu-id="41218-152">Content-Type</span></span>  | <span data-ttu-id="41218-153">application/json</span><span class="sxs-lookup"><span data-stu-id="41218-153">application/json</span></span> |
| <span data-ttu-id="41218-154">Prefer</span><span class="sxs-lookup"><span data-stu-id="41218-154">Prefer</span></span> | <span data-ttu-id="41218-155">return=minimal</span><span class="sxs-lookup"><span data-stu-id="41218-155">return=minimal</span></span> <br><br><span data-ttu-id="41218-156">Указание этого заголовка с запросом, использующим параметр `deltaLink`, приведет к возвращению только свойств объекта, измененных с момента последнего цикла.</span><span class="sxs-lookup"><span data-stu-id="41218-156">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="41218-157">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="41218-157">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41218-158">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41218-158">Request body</span></span>

<span data-ttu-id="41218-159">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41218-159">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="41218-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="41218-160">Response</span></span>

<span data-ttu-id="41218-161">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="41218-161">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="41218-162">Ответ также включает маркер состояния, который является `nextLink` URL-адресом или `deltaLink` URL-адресом.</span><span class="sxs-lookup"><span data-stu-id="41218-162">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="41218-163">Если возвращается URL-адрес `nextLink`:</span><span class="sxs-lookup"><span data-stu-id="41218-163">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="41218-164">Это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="41218-164">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="41218-165">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в отклик не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="41218-165">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="41218-166">Отклик включает тот же набор свойств, что и начальный разностный запрос.</span><span class="sxs-lookup"><span data-stu-id="41218-166">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="41218-167">Это позволяет фиксировать полное текущее состояние объектов при запуске разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="41218-167">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="41218-168">Если возвращается URL-адрес `deltaLink`:</span><span class="sxs-lookup"><span data-stu-id="41218-168">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="41218-169">Это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="41218-169">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="41218-170">Сохраните и используйте URL-адрес `deltaLink`, чтобы узнавать об изменениях ресурса в следующем цикле.</span><span class="sxs-lookup"><span data-stu-id="41218-170">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="41218-171">Вы можете указать заголовок `Prefer:return=minimal`, чтобы включить в значения отклика только свойства, измененные с момента создания `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="41218-171">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="41218-172">По умолчанию: возвращение свойств, совпадающих с начальным разностным запросом</span><span class="sxs-lookup"><span data-stu-id="41218-172">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="41218-173">По умолчанию запросы с использованием `deltaLink` или `nextLink` возвращают те же свойства, которые выбраны в начальном разностном запросе, следующим образом:</span><span class="sxs-lookup"><span data-stu-id="41218-173">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="41218-174">Если свойство изменилось, в отклике содержится новое значение.</span><span class="sxs-lookup"><span data-stu-id="41218-174">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="41218-175">Сюда включаются свойства с заданным значением NULL.</span><span class="sxs-lookup"><span data-stu-id="41218-175">This includes properties being set to null value.</span></span>
- <span data-ttu-id="41218-176">Если свойство не изменилось, в отклике содержится старое значение.</span><span class="sxs-lookup"><span data-stu-id="41218-176">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="41218-177">Если свойство ранее никогда не настраивалось, оно не включается в отклик.</span><span class="sxs-lookup"><span data-stu-id="41218-177">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="41218-178">**Примечание.** При таком поведении просмотр отклика не дает возможность определить, изменилось ли свойство.</span><span class="sxs-lookup"><span data-stu-id="41218-178">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="41218-179">Кроме того, разностные отклики отличаются большими размерами, так как они содержат все значения свойств, как показано [во втором примере](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="41218-179">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="41218-180">Альтернатива: возвращение только измененных свойств</span><span class="sxs-lookup"><span data-stu-id="41218-180">Alternative: return only the changed properties</span></span>

<span data-ttu-id="41218-181">Добавление необязательного заголовка запроса `prefer:return=minimal` приводит к следующему результату:</span><span class="sxs-lookup"><span data-stu-id="41218-181">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="41218-182">Если свойство изменилось, в отклике содержится новое значение.</span><span class="sxs-lookup"><span data-stu-id="41218-182">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="41218-183">Сюда включаются свойства с заданным значением NULL.</span><span class="sxs-lookup"><span data-stu-id="41218-183">This includes properties being set to null value.</span></span>
- <span data-ttu-id="41218-p116">Если свойство не изменилось, оно не включается в отклик. (Отличается от поведения по умолчанию.)</span><span class="sxs-lookup"><span data-stu-id="41218-p116">If the property has not changed, the property is not included in the response at all. (Different from the default behavior.)</span></span>

> <span data-ttu-id="41218-186">**Примечание.** Заголовок можно добавить в запрос `deltaLink` в любой момент разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="41218-186">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="41218-187">Заголовок влияет только на набор свойств, включенный в отклик, и не влияет на способ выполнения разностного запроса.</span><span class="sxs-lookup"><span data-stu-id="41218-187">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="41218-188">См. [третий пример](#request-3) ниже.</span><span class="sxs-lookup"><span data-stu-id="41218-188">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="41218-189">Пример</span><span class="sxs-lookup"><span data-stu-id="41218-189">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="41218-190">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="41218-190">Request 1</span></span>

<span data-ttu-id="41218-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41218-191">The following is an example of the request.</span></span> <span data-ttu-id="41218-192">Параметр `$select` отсутствует, поэтому отслеживается и возвращается набор свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="41218-192">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="41218-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="41218-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/delta
```
# <a name="c"></a>[<span data-ttu-id="41218-194">C#</span><span class="sxs-lookup"><span data-stu-id="41218-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41218-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41218-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41218-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41218-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41218-197">Java</span><span class="sxs-lookup"><span data-stu-id="41218-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-1"></a><span data-ttu-id="41218-198">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="41218-198">Response 1</span></span>

<span data-ttu-id="41218-199">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="41218-199">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="41218-200">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="41218-200">**Note:** The response object shown here might be shortened for readability.</span></span>
>
> <span data-ttu-id="41218-201">Обратите внимание на наличие *members@delta,* которое включает в себя ids объектов-членов в группе.</span><span class="sxs-lookup"><span data-stu-id="41218-201">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="41218-202">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="41218-202">Request 2</span></span>

<span data-ttu-id="41218-203">В следующем примере показан исходный запрос с выбором 3 свойств для отслеживания изменений с поведением отклика по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="41218-203">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>

# <a name="http"></a>[<span data-ttu-id="41218-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="41218-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta_with_select"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
```
# <a name="c"></a>[<span data-ttu-id="41218-205">C#</span><span class="sxs-lookup"><span data-stu-id="41218-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-with-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41218-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41218-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-with-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41218-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41218-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-with-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41218-208">Java</span><span class="sxs-lookup"><span data-stu-id="41218-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-with-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-2"></a><span data-ttu-id="41218-209">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="41218-209">Response 2</span></span>

<span data-ttu-id="41218-210">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="41218-210">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="41218-211">Обратите внимание, что все 3 свойства включаются в отклик, и неизвестно, какие из них изменились с момента получения `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="41218-211">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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

#### <a name="request-3"></a><span data-ttu-id="41218-212">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="41218-212">Request 3</span></span>

<span data-ttu-id="41218-213">В следующем примере показан исходный запрос с выбором 3 свойств для отслеживания изменений с альтернативным поведением отклика с минимальными результатами:</span><span class="sxs-lookup"><span data-stu-id="41218-213">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>

# <a name="http"></a>[<span data-ttu-id="41218-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="41218-214">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta_minimal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```
# <a name="c"></a>[<span data-ttu-id="41218-215">C#</span><span class="sxs-lookup"><span data-stu-id="41218-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41218-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41218-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41218-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41218-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41218-218">Java</span><span class="sxs-lookup"><span data-stu-id="41218-218">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-3"></a><span data-ttu-id="41218-219">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="41218-219">Response 3</span></span>

<span data-ttu-id="41218-220">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="41218-220">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="41218-221">Обратите внимание, что свойство `mailNickname` не включено, то есть оно не изменилось с последнего разностного запроса; `displayName` и `description` включены, то есть их значения изменились.</span><span class="sxs-lookup"><span data-stu-id="41218-221">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="41218-222">См. также</span><span class="sxs-lookup"><span data-stu-id="41218-222">See also</span></span>

- <span data-ttu-id="41218-223">[Отслеживание изменений в данных Microsoft Graph с помощью разностного запроса](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="41218-223">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="41218-224">[Получите дополнительные изменения для групп.](/graph/delta-query-groups)</span><span class="sxs-lookup"><span data-stu-id="41218-224">[Get incremental changes for groups](/graph/delta-query-groups).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

