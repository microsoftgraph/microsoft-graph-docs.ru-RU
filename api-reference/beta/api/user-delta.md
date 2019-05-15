---
title: 'user: delta'
description: Создавайте, обновляйте или удаляйте пользователей без необходимости полного чтения всей коллекции пользователей. Дополнительные сведения см. в статье "Отслеживание изменений".
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c4c95efda43f066f5c2fae127156cc0c076c167b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33961287"
---
# <a name="user-delta"></a><span data-ttu-id="6c19d-104">user: delta</span><span class="sxs-lookup"><span data-stu-id="6c19d-104">user: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c19d-105">Создавайте, обновляйте или удаляйте пользователей без необходимости полного чтения всей коллекции пользователей.</span><span class="sxs-lookup"><span data-stu-id="6c19d-105">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="6c19d-106">Дополнительные сведения см. в статье [Отслеживание изменений](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="6c19d-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c19d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c19d-107">Permissions</span></span>

<span data-ttu-id="6c19d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c19d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6c19d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c19d-110">Permission type</span></span>      | <span data-ttu-id="6c19d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c19d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c19d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c19d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6c19d-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6c19d-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6c19d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c19d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c19d-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c19d-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="6c19d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c19d-116">Application</span></span> | <span data-ttu-id="6c19d-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c19d-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c19d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c19d-118">HTTP request</span></span>

<span data-ttu-id="6c19d-119">Чтобы начать отслеживать изменения, выполните запрос к ресурсу users, включающий функцию delta.</span><span class="sxs-lookup"><span data-stu-id="6c19d-119">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="6c19d-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="6c19d-120">Query parameters</span></span>

<span data-ttu-id="6c19d-121">Отслеживание изменений в ресурсе users — это цикл из одного или нескольких вызовов функции **delta**.</span><span class="sxs-lookup"><span data-stu-id="6c19d-121">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="6c19d-122">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="6c19d-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="6c19d-123">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="6c19d-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="6c19d-124">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="6c19d-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="6c19d-125">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="6c19d-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="6c19d-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="6c19d-126">Query parameter</span></span>      | <span data-ttu-id="6c19d-127">Тип</span><span class="sxs-lookup"><span data-stu-id="6c19d-127">Type</span></span>   |<span data-ttu-id="6c19d-128">Описание</span><span class="sxs-lookup"><span data-stu-id="6c19d-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6c19d-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="6c19d-129">$deltatoken</span></span> | <span data-ttu-id="6c19d-130">string</span><span class="sxs-lookup"><span data-stu-id="6c19d-130">string</span></span> | <span data-ttu-id="6c19d-p105">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции пользователей и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим маркером и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="6c19d-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="6c19d-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="6c19d-133">$skiptoken</span></span> | <span data-ttu-id="6c19d-134">строка</span><span class="sxs-lookup"><span data-stu-id="6c19d-134">string</span></span> | <span data-ttu-id="6c19d-135">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что в коллекции пользователей остаются неотслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="6c19d-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="6c19d-136">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="6c19d-136">OData query parameters</span></span>

<span data-ttu-id="6c19d-137">Этот метод поддерживает необязательные параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6c19d-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="6c19d-p106">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство *id* возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="6c19d-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="6c19d-140">Имеется ограниченная поддержка параметра `$filter`:</span><span class="sxs-lookup"><span data-stu-id="6c19d-140">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="6c19d-141">Единственное поддерживаемое выражение `$filter` предназначено для отслеживания изменений в определенном объекте: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="6c19d-141">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="6c19d-142">Допускается фильтрация нескольких объектов.</span><span class="sxs-lookup"><span data-stu-id="6c19d-142">You can filter multiple objects.</span></span> <span data-ttu-id="6c19d-143">Например, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="6c19d-143">For example, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="6c19d-144">Максимальное количество фильтруемых объектов: 50.</span><span class="sxs-lookup"><span data-stu-id="6c19d-144">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c19d-145">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c19d-145">Request headers</span></span>
| <span data-ttu-id="6c19d-146">Имя</span><span class="sxs-lookup"><span data-stu-id="6c19d-146">Name</span></span>       | <span data-ttu-id="6c19d-147">Описание</span><span class="sxs-lookup"><span data-stu-id="6c19d-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6c19d-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c19d-148">Authorization</span></span>  | <span data-ttu-id="6c19d-149">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="6c19d-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="6c19d-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c19d-150">Content-Type</span></span>  | <span data-ttu-id="6c19d-151">application/json</span><span class="sxs-lookup"><span data-stu-id="6c19d-151">application/json</span></span> |
| <span data-ttu-id="6c19d-152">Prefer</span><span class="sxs-lookup"><span data-stu-id="6c19d-152">Prefer</span></span> | <span data-ttu-id="6c19d-153">return=minimal</span><span class="sxs-lookup"><span data-stu-id="6c19d-153">return=minimal</span></span> <br><br><span data-ttu-id="6c19d-154">Указание этого заголовка с запросом, использующим параметр `deltaLink`, приведет к возвращению только свойств объекта, измененных с момента последнего цикла.</span><span class="sxs-lookup"><span data-stu-id="6c19d-154">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="6c19d-155">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="6c19d-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c19d-156">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6c19d-156">Request body</span></span>
<span data-ttu-id="6c19d-157">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c19d-157">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="6c19d-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c19d-158">Response</span></span>

<span data-ttu-id="6c19d-159">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c19d-159">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="6c19d-160">Оклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="6c19d-160">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="6c19d-161">Если возвращается URL-адрес `nextLink`:</span><span class="sxs-lookup"><span data-stu-id="6c19d-161">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="6c19d-162">Это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="6c19d-162">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="6c19d-163">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в отклик не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="6c19d-163">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="6c19d-164">Отклик включает тот же набор свойств, что и начальный разностный запрос.</span><span class="sxs-lookup"><span data-stu-id="6c19d-164">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="6c19d-165">Это позволяет фиксировать полное текущее состояние объектов при запуске разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="6c19d-165">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="6c19d-166">Если возвращается URL-адрес `deltaLink`:</span><span class="sxs-lookup"><span data-stu-id="6c19d-166">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="6c19d-167">Это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="6c19d-167">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="6c19d-168">Сохраните и используйте URL-адрес `deltaLink`, чтобы узнавать об изменениях ресурса в следующем цикле.</span><span class="sxs-lookup"><span data-stu-id="6c19d-168">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="6c19d-169">Вы можете указать заголовок `Prefer:return=minimal`, чтобы включить в значения отклика только свойства, измененные с момента создания `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="6c19d-169">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="6c19d-170">По умолчанию: возвращение свойств, совпадающих с начальным разностным запросом</span><span class="sxs-lookup"><span data-stu-id="6c19d-170">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="6c19d-171">По умолчанию запросы с использованием `deltaLink` или `nextLink` возвращают те же свойства, которые выбраны в начальном разностном запросе, следующим образом:</span><span class="sxs-lookup"><span data-stu-id="6c19d-171">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="6c19d-172">Если свойство изменилось, в отклике содержится новое значение.</span><span class="sxs-lookup"><span data-stu-id="6c19d-172">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="6c19d-173">Сюда включаются свойства с заданным значением NULL.</span><span class="sxs-lookup"><span data-stu-id="6c19d-173">This includes properties being set to null value.</span></span>
- <span data-ttu-id="6c19d-174">Если свойство не изменилось, в отклике содержится старое значение.</span><span class="sxs-lookup"><span data-stu-id="6c19d-174">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="6c19d-175">Если свойство ранее никогда не настраивалось, оно не включается в отклик.</span><span class="sxs-lookup"><span data-stu-id="6c19d-175">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="6c19d-176">**Примечание.** При таком поведении просмотр отклика не дает возможность определить, изменилось ли свойство.</span><span class="sxs-lookup"><span data-stu-id="6c19d-176">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="6c19d-177">Кроме того, разностные отклики отличаются большими размерами, так как они содержат все значения свойств, как показано [во втором примере](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="6c19d-177">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="6c19d-178">Альтернатива: возвращение только измененных свойств</span><span class="sxs-lookup"><span data-stu-id="6c19d-178">Alternative: return only the changed properties</span></span>

<span data-ttu-id="6c19d-179">Добавление необязательного заголовка запроса `prefer:return=minimal` приводит к следующему результату:</span><span class="sxs-lookup"><span data-stu-id="6c19d-179">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="6c19d-180">Если свойство изменилось, в отклике содержится новое значение.</span><span class="sxs-lookup"><span data-stu-id="6c19d-180">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="6c19d-181">Сюда включаются свойства с заданным значением NULL.</span><span class="sxs-lookup"><span data-stu-id="6c19d-181">This includes properties being set to null value.</span></span>
- <span data-ttu-id="6c19d-182">Если свойство не изменилось, оно не включается в отклик.</span><span class="sxs-lookup"><span data-stu-id="6c19d-182">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="6c19d-183">(Отличается от поведения по умолчанию.)</span><span class="sxs-lookup"><span data-stu-id="6c19d-183">(Different from the default behavior.)</span></span>

> <span data-ttu-id="6c19d-184">**Примечание.** Заголовок можно добавить в запрос `deltaLink` в любой момент разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="6c19d-184">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="6c19d-185">Заголовок влияет только на набор свойств, включенный в отклик, и не влияет на способ выполнения разностного запроса.</span><span class="sxs-lookup"><span data-stu-id="6c19d-185">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="6c19d-186">См. [третий пример](#request-3) ниже.</span><span class="sxs-lookup"><span data-stu-id="6c19d-186">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="6c19d-187">Пример</span><span class="sxs-lookup"><span data-stu-id="6c19d-187">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="6c19d-188">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="6c19d-188">Request 1</span></span>

<span data-ttu-id="6c19d-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c19d-189">The following is an example of the request.</span></span> <span data-ttu-id="6c19d-190">Параметр `$select` отсутствует, поэтому отслеживается и возвращается набор свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6c19d-190">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="6c19d-191">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="6c19d-191">Response 1</span></span>

<span data-ttu-id="6c19d-192">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="6c19d-192">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="6c19d-p119">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c19d-p119">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6c19d-195">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="6c19d-195">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6c19d-196">C#</span><span class="sxs-lookup"><span data-stu-id="6c19d-196">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_delta-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c19d-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c19d-197">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_delta-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

#### <a name="request-2"></a><span data-ttu-id="6c19d-198">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="6c19d-198">Request 2</span></span>

<span data-ttu-id="6c19d-199">В следующем примере показан исходный запрос с выбором 3 свойств для отслеживания изменений с поведением отклика по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="6c19d-199">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta_select"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="6c19d-200">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="6c19d-200">Response 2</span></span>

<span data-ttu-id="6c19d-201">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="6c19d-201">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="6c19d-202">Обратите внимание, что все 3 свойства включаются в отклик, и неизвестно, какие из них изменились с момента получения `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="6c19d-202">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6c19d-203">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="6c19d-203">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6c19d-204">C#</span><span class="sxs-lookup"><span data-stu-id="6c19d-204">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_delta_select-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c19d-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c19d-205">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_delta_select-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

#### <a name="request-3"></a><span data-ttu-id="6c19d-206">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="6c19d-206">Request 3</span></span>

<span data-ttu-id="6c19d-207">В следующем примере показан исходный запрос с выбором 3 свойств для отслеживания изменений с альтернативным поведением отклика с минимальными результатами:</span><span class="sxs-lookup"><span data-stu-id="6c19d-207">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta_minimal"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="6c19d-208">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="6c19d-208">Response 3</span></span>

<span data-ttu-id="6c19d-209">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="6c19d-209">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="6c19d-210">Обратите внимание, что свойство `mobilePhone` не включено, то есть оно не изменилось с последнего разностного запроса; `displayName` и `jobTitle` включены, то есть их значения изменились.</span><span class="sxs-lookup"><span data-stu-id="6c19d-210">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6c19d-211">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="6c19d-211">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6c19d-212">C#</span><span class="sxs-lookup"><span data-stu-id="6c19d-212">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_delta_minimal-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c19d-213">Javascript</span><span class="sxs-lookup"><span data-stu-id="6c19d-213">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_delta_minimal-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

- <span data-ttu-id="6c19d-214">[Отслеживание изменений в данных Microsoft Graph с помощью разностного запроса](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="6c19d-214">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="6c19d-215">[Получение добавочных изменений для пользователей](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="6c19d-215">[Get incremental changes for users](/graph/delta-query-users).</span></span>

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
    "Error: /api-reference/beta/api/user-delta.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-delta.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-delta.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-delta.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-delta.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-delta.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
