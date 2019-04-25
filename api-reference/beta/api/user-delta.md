---
title: 'user: delta'
description: Получение новых, обновленных или удаленных пользователей без выполнения полного чтения коллекции пользователей целиком. Сведения об исправлениях приведены в разделе Tracking.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6fd8eb71c1b647550219ae6686a0bc814420b2fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537005"
---
# <a name="user-delta"></a><span data-ttu-id="73a87-104">user: delta</span><span class="sxs-lookup"><span data-stu-id="73a87-104">user: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73a87-105">Получение новых, обновленных или удаленных пользователей без выполнения полного чтения коллекции пользователей целиком.</span><span class="sxs-lookup"><span data-stu-id="73a87-105">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="73a87-106">Сведения [](/graph/delta-query-overview) об исправлениях приведены в разделе Tracking.</span><span class="sxs-lookup"><span data-stu-id="73a87-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="73a87-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73a87-107">Permissions</span></span>

<span data-ttu-id="73a87-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73a87-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="73a87-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73a87-110">Permission type</span></span>      | <span data-ttu-id="73a87-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73a87-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73a87-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73a87-112">Delegated (work or school account)</span></span> | <span data-ttu-id="73a87-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="73a87-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="73a87-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73a87-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73a87-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73a87-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="73a87-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73a87-116">Application</span></span> | <span data-ttu-id="73a87-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73a87-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73a87-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73a87-118">HTTP request</span></span>

<span data-ttu-id="73a87-119">Чтобы начать отслеживать изменения, выполните запрос к ресурсу users, включающий функцию delta.</span><span class="sxs-lookup"><span data-stu-id="73a87-119">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="73a87-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="73a87-120">Query parameters</span></span>

<span data-ttu-id="73a87-121">Отслеживание изменений в пользователях приводит к округлению одного или нескольких вызовов функции **Delta** .</span><span class="sxs-lookup"><span data-stu-id="73a87-121">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="73a87-122">Если вы используете любой параметр запроса (кроме `$deltatoken` и `$skiptoken`), необходимо указать его в исходном запросе **Delta** .</span><span class="sxs-lookup"><span data-stu-id="73a87-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="73a87-123">Microsoft Graph автоматически кодирует все заданные параметры в часть маркера или `nextLink` `deltaLink` URL-адрес, указанный в ответе.</span><span class="sxs-lookup"><span data-stu-id="73a87-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="73a87-124">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="73a87-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="73a87-125">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="73a87-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="73a87-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="73a87-126">Query parameter</span></span>      | <span data-ttu-id="73a87-127">Тип</span><span class="sxs-lookup"><span data-stu-id="73a87-127">Type</span></span>   |<span data-ttu-id="73a87-128">Описание</span><span class="sxs-lookup"><span data-stu-id="73a87-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="73a87-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="73a87-129">$deltatoken</span></span> | <span data-ttu-id="73a87-130">string</span><span class="sxs-lookup"><span data-stu-id="73a87-130">string</span></span> | <span data-ttu-id="73a87-p105">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции пользователей и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="73a87-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="73a87-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="73a87-133">$skiptoken</span></span> | <span data-ttu-id="73a87-134">строка</span><span class="sxs-lookup"><span data-stu-id="73a87-134">string</span></span> | <span data-ttu-id="73a87-135">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что в коллекции пользователей остаются неотслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="73a87-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="73a87-136">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="73a87-136">OData query parameters</span></span>

<span data-ttu-id="73a87-137">Этот метод поддерживает необязательные параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="73a87-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="73a87-p106">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство *id* возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="73a87-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="73a87-140">Существует ограниченная поддержка `$filter`:</span><span class="sxs-lookup"><span data-stu-id="73a87-140">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="73a87-141">Единственное поддерживаемое выражение `$filter` предназначено для отслеживания изменений в определенном объекте: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="73a87-141">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="73a87-142">Допускается фильтрация нескольких объектов.</span><span class="sxs-lookup"><span data-stu-id="73a87-142">You can filter multiple objects.</span></span> <span data-ttu-id="73a87-143">Например, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="73a87-143">For example, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="73a87-144">Максимальное количество фильтруемых объектов: 50.</span><span class="sxs-lookup"><span data-stu-id="73a87-144">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73a87-145">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73a87-145">Request headers</span></span>
| <span data-ttu-id="73a87-146">Имя</span><span class="sxs-lookup"><span data-stu-id="73a87-146">Name</span></span>       | <span data-ttu-id="73a87-147">Описание</span><span class="sxs-lookup"><span data-stu-id="73a87-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="73a87-148">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73a87-148">Authorization</span></span>  | <span data-ttu-id="73a87-149">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="73a87-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="73a87-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73a87-150">Content-Type</span></span>  | <span data-ttu-id="73a87-151">application/json</span><span class="sxs-lookup"><span data-stu-id="73a87-151">application/json</span></span> |
| <span data-ttu-id="73a87-152">Prefer</span><span class="sxs-lookup"><span data-stu-id="73a87-152">Prefer</span></span> | <span data-ttu-id="73a87-153">Возврат = минимум</span><span class="sxs-lookup"><span data-stu-id="73a87-153">return=minimal</span></span> <br><br><span data-ttu-id="73a87-154">При указании заголовка с запросом, который `deltaLink` использует объект, возвращаются только свойства объекта, которые были изменены с момента последнего цикла.</span><span class="sxs-lookup"><span data-stu-id="73a87-154">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="73a87-155">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="73a87-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73a87-156">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73a87-156">Request body</span></span>
<span data-ttu-id="73a87-157">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73a87-157">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="73a87-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="73a87-158">Response</span></span>

<span data-ttu-id="73a87-159">В случае успеха этот метод возвращает код ответа `200 OK` и объект коллекции [user](../resources/user.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="73a87-159">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="73a87-160">В ответ также включается `nextLink` URL-адрес `deltaLink` или URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="73a87-160">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="73a87-161">Если возвращается `nextLink` URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="73a87-161">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="73a87-162">Это указывает на необходимость извлечения дополнительных страниц данных в сеансе.</span><span class="sxs-lookup"><span data-stu-id="73a87-162">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="73a87-163">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="73a87-163">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="73a87-164">Ответ включает тот же набор свойств, что и в исходном запросе на разностный запрос.</span><span class="sxs-lookup"><span data-stu-id="73a87-164">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="73a87-165">Это позволяет захватить полное текущее состояние объектов при инициации разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="73a87-165">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="73a87-166">Если возвращается `deltaLink` URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="73a87-166">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="73a87-167">Это указывает на то, что больше нет данных о существующем состоянии ресурса, который необходимо возвратить.</span><span class="sxs-lookup"><span data-stu-id="73a87-167">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="73a87-168">Сохраните и используйте `deltaLink` URL-адрес, чтобы узнать об изменениях ресурса в следующем цикле.</span><span class="sxs-lookup"><span data-stu-id="73a87-168">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="73a87-169">Вы можете указать `Prefer:return=minimal` заголовок, чтобы включить в значения отклика только те свойства, которые были изменены с момента `deltaLink` выпуска.</span><span class="sxs-lookup"><span data-stu-id="73a87-169">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="73a87-170">По умолчанию: возврат тех же свойств, что и исходный запрос Дельта</span><span class="sxs-lookup"><span data-stu-id="73a87-170">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="73a87-171">По умолчанию запросы, использующие `deltaLink` или `nextLink` возвращающие те же свойства, что и выбранные в начальном запросе Дельта, запрашиваются следующими способами:</span><span class="sxs-lookup"><span data-stu-id="73a87-171">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="73a87-172">Если свойство изменилось, в ответ включается новое значение.</span><span class="sxs-lookup"><span data-stu-id="73a87-172">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="73a87-173">Сюда входят свойства, для которых задано значение null.</span><span class="sxs-lookup"><span data-stu-id="73a87-173">This includes properties being set to null value.</span></span>
- <span data-ttu-id="73a87-174">Если свойство не изменилось, в ответ включается старое значение.</span><span class="sxs-lookup"><span data-stu-id="73a87-174">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="73a87-175">Если свойство никогда не задается до тех пор, пока оно не будет включено в ответ вообще.</span><span class="sxs-lookup"><span data-stu-id="73a87-175">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="73a87-176">**Примечание:** Таким образом, изучив ответ, можно определить, изменяется ли свойство.</span><span class="sxs-lookup"><span data-stu-id="73a87-176">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="73a87-177">Кроме того, разностные ответы обычно имеют большой размер, так как они содержат все значения свойств, как показано во [втором примере](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="73a87-177">Also, the delta responses tend to be large because they contain all property values  - as shown in the [second example](#request-2) below.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="73a87-178">Альтернатива: возврат только измененных свойств</span><span class="sxs-lookup"><span data-stu-id="73a87-178">Alternative: return only the changed properties</span></span>

<span data-ttu-id="73a87-179">Добавление необязательного заголовка запроса `prefer:return=minimal` — приводит к следующему поведению:</span><span class="sxs-lookup"><span data-stu-id="73a87-179">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="73a87-180">Если свойство изменилось, в ответ включается новое значение.</span><span class="sxs-lookup"><span data-stu-id="73a87-180">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="73a87-181">Сюда входят свойства, для которых задано значение null.</span><span class="sxs-lookup"><span data-stu-id="73a87-181">This includes properties being set to null value.</span></span>
- <span data-ttu-id="73a87-182">Если свойство не изменилось, свойство не включается в ответ вообще.</span><span class="sxs-lookup"><span data-stu-id="73a87-182">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="73a87-183">(Отличается от поведения по умолчанию.)</span><span class="sxs-lookup"><span data-stu-id="73a87-183">(Different from the default behavior.)</span></span>

> <span data-ttu-id="73a87-184">**Примечание:** Заголовок можно добавить в `deltaLink` запрос в любой момент времени в разностном цикле.</span><span class="sxs-lookup"><span data-stu-id="73a87-184">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="73a87-185">Заголовок влияет только на набор свойств, включенных в ответ, и не влияет на то, как выполняется разностный запрос.</span><span class="sxs-lookup"><span data-stu-id="73a87-185">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="73a87-186">Просмотрите [третий пример](#request-3) ниже.</span><span class="sxs-lookup"><span data-stu-id="73a87-186">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="73a87-187">Пример</span><span class="sxs-lookup"><span data-stu-id="73a87-187">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="73a87-188">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="73a87-188">Request 1</span></span>

<span data-ttu-id="73a87-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73a87-189">The following is an example of the request.</span></span> <span data-ttu-id="73a87-190">Параметр не `$select` задан, поэтому набор свойств по умолчанию отслеживается и возвращается.</span><span class="sxs-lookup"><span data-stu-id="73a87-190">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="73a87-191">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="73a87-191">Response 1</span></span>

<span data-ttu-id="73a87-192">Ниже приведен пример ответа, полученного при использовании метода `deltaLink` , полученного при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="73a87-192">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="73a87-193">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="73a87-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="73a87-194">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73a87-194">All the properties will be returned from an actual call.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="73a87-195">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="73a87-195">Request 2</span></span>

<span data-ttu-id="73a87-196">В следующем примере показан первоначальный запрос, в котором выбирается 3 свойства для отслеживания изменений с поведением ответа по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="73a87-196">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="73a87-197">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="73a87-197">Response 2</span></span>

<span data-ttu-id="73a87-198">Ниже приведен пример ответа, полученного при использовании метода `deltaLink` , полученного при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="73a87-198">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="73a87-199">Обратите внимание на то, что в ответ включены все 3 свойства, и они не известны, какие из `deltaLink` них были изменены с момента получения.</span><span class="sxs-lookup"><span data-stu-id="73a87-199">Note that all 3 properties are included in the response and it is not known which ones have changed since the `deltaLink` was obtained.</span></span>

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

#### <a name="request-3"></a><span data-ttu-id="73a87-200">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="73a87-200">Request 3</span></span>

<span data-ttu-id="73a87-201">В следующем примере показано, как исходный запрос выбирает 3 свойства для отслеживания изменений с альтернативным поведением минимального ответа:</span><span class="sxs-lookup"><span data-stu-id="73a87-201">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="73a87-202">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="73a87-202">Response 3</span></span>

<span data-ttu-id="73a87-203">Ниже приведен пример ответа, полученного при использовании метода `deltaLink` , полученного при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="73a87-203">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="73a87-204">Обратите внимание `mobilePhone` , что свойство не включается, что означает, что он не изменился с момента последнего запроса Дельта; `displayName` и `jobTitle` включены, что означает, что их значения изменились.</span><span class="sxs-lookup"><span data-stu-id="73a87-204">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

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

- <span data-ttu-id="73a87-205">[Использование запроса изменений для отслеживания изменений в данных Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="73a87-205">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="73a87-206">[Получение добавочных изменений для пользователей](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="73a87-206">[Get incremental changes for users](/graph/delta-query-users).</span></span>

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
    "Error: /api-reference/beta/api/user-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
