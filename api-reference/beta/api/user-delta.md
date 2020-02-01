---
title: 'user: delta'
description: Создавайте, обновляйте или удаляйте пользователей без необходимости полного чтения всей коллекции пользователей.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 605b4fa7a890d1f2a74b44fe00eb3e978a2ee5dd
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2020
ms.locfileid: "41652039"
---
# <a name="user-delta"></a><span data-ttu-id="36e51-103">user: delta</span><span class="sxs-lookup"><span data-stu-id="36e51-103">user: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36e51-104">Создавайте, обновляйте или удаляйте пользователей без необходимости полного чтения всей коллекции пользователей.</span><span class="sxs-lookup"><span data-stu-id="36e51-104">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="36e51-105">Дополнительные сведения см. в статье [Отслеживание изменений](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="36e51-105">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="36e51-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36e51-106">Permissions</span></span>

<span data-ttu-id="36e51-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36e51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="36e51-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36e51-109">Permission type</span></span>      | <span data-ttu-id="36e51-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36e51-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36e51-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36e51-111">Delegated (work or school account)</span></span> | <span data-ttu-id="36e51-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="36e51-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="36e51-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36e51-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36e51-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36e51-114">Not supported.</span></span>  |
|<span data-ttu-id="36e51-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36e51-115">Application</span></span> | <span data-ttu-id="36e51-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36e51-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36e51-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36e51-117">HTTP request</span></span>

<span data-ttu-id="36e51-118">Чтобы начать отслеживать изменения, выполните запрос к ресурсу users, включающий функцию delta.</span><span class="sxs-lookup"><span data-stu-id="36e51-118">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="36e51-119">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="36e51-119">Query parameters</span></span>

<span data-ttu-id="36e51-120">Отслеживание изменений в ресурсе users — это цикл из одного или нескольких вызовов функции **delta**.</span><span class="sxs-lookup"><span data-stu-id="36e51-120">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="36e51-121">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="36e51-121">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="36e51-122">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="36e51-122">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="36e51-123">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="36e51-123">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="36e51-124">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="36e51-124">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="36e51-125">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="36e51-125">Query parameter</span></span>      | <span data-ttu-id="36e51-126">Тип</span><span class="sxs-lookup"><span data-stu-id="36e51-126">Type</span></span>   |<span data-ttu-id="36e51-127">Описание</span><span class="sxs-lookup"><span data-stu-id="36e51-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="36e51-128">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="36e51-128">$deltatoken</span></span> | <span data-ttu-id="36e51-129">string</span><span class="sxs-lookup"><span data-stu-id="36e51-129">string</span></span> | <span data-ttu-id="36e51-p104">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции пользователей и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим маркером и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="36e51-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="36e51-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="36e51-132">$skiptoken</span></span> | <span data-ttu-id="36e51-133">строка</span><span class="sxs-lookup"><span data-stu-id="36e51-133">string</span></span> | <span data-ttu-id="36e51-134">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что в коллекции пользователей остаются неотслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="36e51-134">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="36e51-135">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="36e51-135">OData query parameters</span></span>

<span data-ttu-id="36e51-136">Этот метод поддерживает необязательные параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="36e51-136">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="36e51-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство *id* возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="36e51-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="36e51-139">Имеется ограниченная поддержка параметра `$filter`:</span><span class="sxs-lookup"><span data-stu-id="36e51-139">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="36e51-140">Единственное поддерживаемое выражение `$filter` предназначено для отслеживания изменений в определенном объекте: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="36e51-140">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="36e51-141">Допускается фильтрация нескольких объектов.</span><span class="sxs-lookup"><span data-stu-id="36e51-141">You can filter multiple objects.</span></span> <span data-ttu-id="36e51-142">Например, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="36e51-142">For example, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="36e51-143">Максимальное количество фильтруемых объектов: 50.</span><span class="sxs-lookup"><span data-stu-id="36e51-143">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36e51-144">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36e51-144">Request headers</span></span>
| <span data-ttu-id="36e51-145">Имя</span><span class="sxs-lookup"><span data-stu-id="36e51-145">Name</span></span>       | <span data-ttu-id="36e51-146">Описание</span><span class="sxs-lookup"><span data-stu-id="36e51-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="36e51-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="36e51-147">Authorization</span></span>  | <span data-ttu-id="36e51-148">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="36e51-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="36e51-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="36e51-149">Content-Type</span></span>  | <span data-ttu-id="36e51-150">application/json</span><span class="sxs-lookup"><span data-stu-id="36e51-150">application/json</span></span> |
| <span data-ttu-id="36e51-151">Prefer</span><span class="sxs-lookup"><span data-stu-id="36e51-151">Prefer</span></span> | <span data-ttu-id="36e51-152">return=minimal</span><span class="sxs-lookup"><span data-stu-id="36e51-152">return=minimal</span></span> <br><br><span data-ttu-id="36e51-153">Указание этого заголовка с запросом, использующим параметр `deltaLink`, приведет к возвращению только свойств объекта, измененных с момента последнего цикла.</span><span class="sxs-lookup"><span data-stu-id="36e51-153">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="36e51-154">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="36e51-154">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36e51-155">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="36e51-155">Request body</span></span>
<span data-ttu-id="36e51-156">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36e51-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36e51-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="36e51-157">Response</span></span>

<span data-ttu-id="36e51-158">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36e51-158">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="36e51-159">Оклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="36e51-159">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="36e51-160">Если возвращается URL-адрес `nextLink`:</span><span class="sxs-lookup"><span data-stu-id="36e51-160">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="36e51-161">Это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="36e51-161">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="36e51-162">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в отклик не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="36e51-162">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="36e51-163">Отклик включает тот же набор свойств, что и начальный разностный запрос.</span><span class="sxs-lookup"><span data-stu-id="36e51-163">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="36e51-164">Это позволяет фиксировать полное текущее состояние объектов при запуске разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="36e51-164">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="36e51-165">Если возвращается URL-адрес `deltaLink`:</span><span class="sxs-lookup"><span data-stu-id="36e51-165">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="36e51-166">Это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="36e51-166">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="36e51-167">Сохраните и используйте URL-адрес `deltaLink`, чтобы узнавать об изменениях ресурса в следующем цикле.</span><span class="sxs-lookup"><span data-stu-id="36e51-167">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="36e51-168">Вы можете указать заголовок `Prefer:return=minimal`, чтобы включить в значения отклика только свойства, измененные с момента создания `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="36e51-168">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="36e51-169">По умолчанию: возвращение свойств, совпадающих с начальным разностным запросом</span><span class="sxs-lookup"><span data-stu-id="36e51-169">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="36e51-170">По умолчанию запросы с использованием `deltaLink` или `nextLink` возвращают те же свойства, которые выбраны в начальном разностном запросе, следующим образом:</span><span class="sxs-lookup"><span data-stu-id="36e51-170">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="36e51-171">Если свойство изменилось, в отклике содержится новое значение.</span><span class="sxs-lookup"><span data-stu-id="36e51-171">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="36e51-172">Сюда включаются свойства с заданным значением NULL.</span><span class="sxs-lookup"><span data-stu-id="36e51-172">This includes properties being set to null value.</span></span>
- <span data-ttu-id="36e51-173">Если свойство не изменилось, в отклике содержится старое значение.</span><span class="sxs-lookup"><span data-stu-id="36e51-173">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="36e51-174">Если свойство ранее никогда не настраивалось, оно не включается в отклик.</span><span class="sxs-lookup"><span data-stu-id="36e51-174">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="36e51-175">**Примечание.** При таком поведении просмотр отклика не дает возможность определить, изменилось ли свойство.</span><span class="sxs-lookup"><span data-stu-id="36e51-175">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="36e51-176">Кроме того, разностные отклики отличаются большими размерами, так как они содержат все значения свойств, как показано в [примере 2](#example-2-selecting-three-properties).</span><span class="sxs-lookup"><span data-stu-id="36e51-176">Also, the delta responses tend to be large because they contain all property values  - as shown in [Example 2](#example-2-selecting-three-properties).</span></span>

### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="36e51-177">Альтернатива: возвращение только измененных свойств</span><span class="sxs-lookup"><span data-stu-id="36e51-177">Alternative: return only the changed properties</span></span>

<span data-ttu-id="36e51-178">Добавление необязательного заголовка запроса `prefer:return=minimal` приводит к следующему результату:</span><span class="sxs-lookup"><span data-stu-id="36e51-178">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="36e51-179">Если свойство изменилось, в отклике содержится новое значение.</span><span class="sxs-lookup"><span data-stu-id="36e51-179">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="36e51-180">Сюда включаются свойства с заданным значением NULL.</span><span class="sxs-lookup"><span data-stu-id="36e51-180">This includes properties being set to null value.</span></span>
- <span data-ttu-id="36e51-181">Если свойство не изменилось, оно не включается в отклик.</span><span class="sxs-lookup"><span data-stu-id="36e51-181">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="36e51-182">(Отличается от поведения по умолчанию.)</span><span class="sxs-lookup"><span data-stu-id="36e51-182">(Different from the default behavior.)</span></span>

> <span data-ttu-id="36e51-183">**Примечание.** Заголовок можно добавить в запрос `deltaLink` в любой момент разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="36e51-183">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="36e51-184">Заголовок влияет только на набор свойств, включенный в отклик, и не влияет на способ выполнения разностного запроса.</span><span class="sxs-lookup"><span data-stu-id="36e51-184">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="36e51-185">См. [пример 3](#example-3-alternative-minimal-response-behavior).</span><span class="sxs-lookup"><span data-stu-id="36e51-185">See [Example 3](#example-3-alternative-minimal-response-behavior).</span></span>

## <a name="examples"></a><span data-ttu-id="36e51-186">Примеры</span><span class="sxs-lookup"><span data-stu-id="36e51-186">Examples</span></span>

### <a name="example-1-default-properties"></a><span data-ttu-id="36e51-187">Пример 1. Свойства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="36e51-187">Example 1: Default properties</span></span>

#### <a name="request"></a><span data-ttu-id="36e51-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="36e51-188">Request</span></span>

<span data-ttu-id="36e51-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36e51-189">The following is an example of the request.</span></span> <span data-ttu-id="36e51-190">Параметр `$select` отсутствует, поэтому отслеживается и возвращается набор свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="36e51-190">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="36e51-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="36e51-191">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/delta
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="36e51-192">C#</span><span class="sxs-lookup"><span data-stu-id="36e51-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36e51-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36e51-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36e51-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36e51-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36e51-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="36e51-195">Response</span></span>

<span data-ttu-id="36e51-196">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="36e51-196">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="36e51-p118">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36e51-p118">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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

### <a name="example-2-selecting-three-properties"></a><span data-ttu-id="36e51-199">Пример 2. Выбор трех свойств</span><span class="sxs-lookup"><span data-stu-id="36e51-199">Example 2: Selecting three properties</span></span>

#### <a name="request"></a><span data-ttu-id="36e51-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="36e51-200">Request</span></span>

<span data-ttu-id="36e51-201">В следующем примере показан исходный запрос с выбором трех свойств для отслеживания изменений с поведением отклика по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="36e51-201">The next example shows the initial request selecting three properties for change tracking, with default response behavior.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="36e51-202">HTTP</span><span class="sxs-lookup"><span data-stu-id="36e51-202">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta_select"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="36e51-203">C#</span><span class="sxs-lookup"><span data-stu-id="36e51-203">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36e51-204">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36e51-204">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36e51-205">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36e51-205">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36e51-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="36e51-206">Response</span></span>

<span data-ttu-id="36e51-207">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="36e51-207">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="36e51-208">Обратите внимание, что все три свойства включаются в отклик, и неизвестно, какие из них изменились с момента получения `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="36e51-208">Note that all three properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": "jobTitle-value",
      "mobilePhone": null
    }
  ]
}
```

### <a name="example-3-alternative-minimal-response-behavior"></a><span data-ttu-id="36e51-209">Пример 3. Альтернативное поведение минимального отклика</span><span class="sxs-lookup"><span data-stu-id="36e51-209">Example 3: Alternative minimal response behavior</span></span>

#### <a name="request"></a><span data-ttu-id="36e51-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="36e51-210">Request</span></span>

<span data-ttu-id="36e51-211">В следующем примере показан исходный запрос с выбором трех свойств для отслеживания изменений с альтернативным поведением отклика с минимальными результатами.</span><span class="sxs-lookup"><span data-stu-id="36e51-211">The next example shows the initial request selecting three properties for change tracking, with alternative minimal response behavior.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="36e51-212">HTTP</span><span class="sxs-lookup"><span data-stu-id="36e51-212">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delta_minimal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="36e51-213">C#</span><span class="sxs-lookup"><span data-stu-id="36e51-213">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36e51-214">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36e51-214">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36e51-215">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36e51-215">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36e51-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="36e51-216">Response</span></span>

<span data-ttu-id="36e51-217">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="36e51-217">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="36e51-218">Обратите внимание, что свойство `mobilePhone` не включено, то есть оно не изменилось с последнего разностного запроса; `displayName` и `jobTitle` включены, то есть их значения изменились.</span><span class="sxs-lookup"><span data-stu-id="36e51-218">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```
## <a name="see-also"></a><span data-ttu-id="36e51-219">См. также</span><span class="sxs-lookup"><span data-stu-id="36e51-219">See also</span></span>

- <span data-ttu-id="36e51-220">[Отслеживание изменений в данных Microsoft Graph с помощью разностного запроса](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="36e51-220">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="36e51-221">[Получение добавочных изменений для пользователей](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="36e51-221">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
