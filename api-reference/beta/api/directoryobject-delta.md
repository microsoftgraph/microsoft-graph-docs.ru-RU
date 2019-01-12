---
title: 'directoryObject: дельты'
description: 'Get вновь созданных, обновлении или удалении объектов каталога из следующих типов: пользователей, группы и организационной контакт в запросе единого дельты. Отслеживание изменений для получения дополнительных сведений см.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 59ab4f819072120533215277b8b14ac1f3c94bf7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956201"
---
# <a name="directoryobject-delta"></a><span data-ttu-id="919e0-104">directoryObject: дельты</span><span class="sxs-lookup"><span data-stu-id="919e0-104">directoryObject: delta</span></span>

> <span data-ttu-id="919e0-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="919e0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="919e0-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="919e0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="919e0-107">Get вновь созданных, обновлении или удалении объектов каталога из следующих типов: [пользователей](../resources/user.md), [группы](../resources/group.md) и [организационной контактов](../resources/orgcontact.md), в запросе единого дельты.</span><span class="sxs-lookup"><span data-stu-id="919e0-107">Get newly created, updated, or deleted directory objects of the following types: [user](../resources/user.md), [group](../resources/group.md) and [organizational contact](../resources/orgcontact.md), in a single delta query.</span></span> <span data-ttu-id="919e0-108">Дополнительные сведения см [Отслеживание изменений](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="919e0-108">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="919e0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="919e0-109">Permissions</span></span>

<span data-ttu-id="919e0-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="919e0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="919e0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="919e0-112">Permission type</span></span>      | <span data-ttu-id="919e0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="919e0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="919e0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="919e0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="919e0-115">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="919e0-115">Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="919e0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="919e0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="919e0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="919e0-117">Not supported.</span></span>  |
|<span data-ttu-id="919e0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="919e0-118">Application</span></span> | <span data-ttu-id="919e0-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="919e0-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="919e0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="919e0-120">HTTP request</span></span>

<span data-ttu-id="919e0-121">Чтобы начать отслеживание изменений, внесите запроса, включая функцию дельты на directoryObjects ресурсов.</span><span class="sxs-lookup"><span data-stu-id="919e0-121">To begin tracking changes, you make a request including the delta function on the directoryObjects resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a><span data-ttu-id="919e0-122">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="919e0-122">Query parameters</span></span>

<span data-ttu-id="919e0-123">Отслеживание изменений приводит к round один или несколько вызовов функций **дельты** .</span><span class="sxs-lookup"><span data-stu-id="919e0-123">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="919e0-124">При использовании любого параметра запроса (отличный от `$deltatoken` и `$skiptoken`), необходимо указать его в запрос начальной **дельты** .</span><span class="sxs-lookup"><span data-stu-id="919e0-124">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="919e0-125">Microsoft Graph автоматически Кодирует указанный параметров в маркеров часть `nextLink` или `deltaLink` URL-адреса, приведенные в ответе.</span><span class="sxs-lookup"><span data-stu-id="919e0-125">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="919e0-126">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="919e0-126">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="919e0-127">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="919e0-127">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="919e0-128">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="919e0-128">Query parameter</span></span> | <span data-ttu-id="919e0-129">Тип</span><span class="sxs-lookup"><span data-stu-id="919e0-129">Type</span></span> |<span data-ttu-id="919e0-130">Описание</span><span class="sxs-lookup"><span data-stu-id="919e0-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="919e0-131">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="919e0-131">$deltatoken</span></span> | <span data-ttu-id="919e0-132">строка</span><span class="sxs-lookup"><span data-stu-id="919e0-132">string</span></span> | <span data-ttu-id="919e0-p106">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции пользователей и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="919e0-p106">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="919e0-135">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="919e0-135">$skiptoken</span></span> | <span data-ttu-id="919e0-136">строка</span><span class="sxs-lookup"><span data-stu-id="919e0-136">string</span></span> | <span data-ttu-id="919e0-137">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что в коллекции пользователей остаются неотслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="919e0-137">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="919e0-138">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="919e0-138">OData query parameters</span></span>

<span data-ttu-id="919e0-139">Этот метод поддерживает дополнительные параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="919e0-139">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="919e0-140">Можно использовать `$filter` с специальные `isOf` оператор для фильтрации подмножество типов, производные от directoryObject.</span><span class="sxs-lookup"><span data-stu-id="919e0-140">You can use `$filter` with the special `isOf` operator to filter a subset of types derived from directoryObject.</span></span>
  - <span data-ttu-id="919e0-141">Вы можете сочетать несколько выражений с помощью `or`, позволяет запросе единого дельты отслеживание нескольких типов.</span><span class="sxs-lookup"><span data-stu-id="919e0-141">You can combine multiple expressions using an `or`, which allows you to have a single delta query tracking multiple types.</span></span> <span data-ttu-id="919e0-142">[Третий пример](#request-3) для получения дополнительных сведений см.</span><span class="sxs-lookup"><span data-stu-id="919e0-142">See the [third example](#request-3) for details.</span></span>

## <a name="request-headers"></a><span data-ttu-id="919e0-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="919e0-143">Request headers</span></span>

| <span data-ttu-id="919e0-144">Имя</span><span class="sxs-lookup"><span data-stu-id="919e0-144">Name</span></span>       | <span data-ttu-id="919e0-145">Описание</span><span class="sxs-lookup"><span data-stu-id="919e0-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="919e0-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="919e0-146">Authorization</span></span>  | <span data-ttu-id="919e0-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="919e0-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="919e0-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="919e0-148">Content-Type</span></span>  | <span data-ttu-id="919e0-149">application/json</span><span class="sxs-lookup"><span data-stu-id="919e0-149">application/json</span></span> |
| <span data-ttu-id="919e0-150">Prefer</span><span class="sxs-lookup"><span data-stu-id="919e0-150">Prefer</span></span> | <span data-ttu-id="919e0-151">Возвращает = минимальный</span><span class="sxs-lookup"><span data-stu-id="919e0-151">return=minimal</span></span> <br><br><span data-ttu-id="919e0-152">Указание этот заголовок с запросом, который использует `deltaLink` возвращает свойства объекта, которые были изменены с момента последнего цикла.</span><span class="sxs-lookup"><span data-stu-id="919e0-152">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="919e0-153">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="919e0-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="919e0-154">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="919e0-154">Request body</span></span>

<span data-ttu-id="919e0-155">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="919e0-155">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="919e0-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="919e0-156">Response</span></span>

<span data-ttu-id="919e0-157">Успешно завершена, этот метод возвращает `200 OK` ответа [пользователя](../resources/directoryobject.md) и кода объект коллекции в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="919e0-157">If successful, this method returns `200 OK` response code and [user](../resources/directoryobject.md) collection object in the response body.</span></span> <span data-ttu-id="919e0-158">Ответ также включает `nextLink` URL-адрес или `deltaLink` URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="919e0-158">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="919e0-159">Если `nextLink` возвращается URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="919e0-159">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="919e0-160">Это означает, что существуют дополнительные страницы данных для получения в сеанс.</span><span class="sxs-lookup"><span data-stu-id="919e0-160">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="919e0-161">Приложение по-прежнему производится выполняете запросы, используя `nextLink` URL-адрес, пока не `deltaLink` URL-адрес включен в ответе.</span><span class="sxs-lookup"><span data-stu-id="919e0-161">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="919e0-162">Ответ включает тот же набор свойств, как и в запросе начальной дельты.</span><span class="sxs-lookup"><span data-stu-id="919e0-162">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="919e0-163">Это позволяет записывать полное текущего состояния объектов при начале цикла дельты.</span><span class="sxs-lookup"><span data-stu-id="919e0-163">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="919e0-164">Если `deltaLink` возвращается URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="919e0-164">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="919e0-165">Это означает, что нет дополнительных данных о состоянии существующих ресурсов должно быть возвращено.</span><span class="sxs-lookup"><span data-stu-id="919e0-165">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="919e0-166">Сохраните и использовать `deltaLink` URL-адрес, чтобы узнать о изменяется с ресурсом в следующего цикла.</span><span class="sxs-lookup"><span data-stu-id="919e0-166">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="919e0-167">У вас есть выбор для указания `Prefer:return=minimal` заголовок, чтобы включить в ответ значения для свойств, которые были изменены со времени `deltaLink` был отправлен.</span><span class="sxs-lookup"><span data-stu-id="919e0-167">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="919e0-168">Значение по умолчанию: возврата же свойства, что запрос на начальное дельты</span><span class="sxs-lookup"><span data-stu-id="919e0-168">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="919e0-169">По умолчанию, запросы с помощью `deltaLink` или `nextLink` возврата же свойства, что выбранный в запросе начальной дельты следующими способами:</span><span class="sxs-lookup"><span data-stu-id="919e0-169">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="919e0-170">При изменении свойства новое значение включается в ответе.</span><span class="sxs-lookup"><span data-stu-id="919e0-170">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="919e0-171">Этот компонент включает свойства задаются на значение null.</span><span class="sxs-lookup"><span data-stu-id="919e0-171">This includes properties being set to null value.</span></span>
- <span data-ttu-id="919e0-172">Если свойство не был изменен, старое значение включается в ответе.</span><span class="sxs-lookup"><span data-stu-id="919e0-172">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="919e0-173">Если свойство имеет значение никогда не перед его не будут включены в ответе на всех.</span><span class="sxs-lookup"><span data-stu-id="919e0-173">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="919e0-174">**Примечание:** С помощью этого поведения, посмотрев ответа не позволяет определить, будет ли свойство изменяется, или не.</span><span class="sxs-lookup"><span data-stu-id="919e0-174">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="919e0-175">Кроме того ответы дельты приводят к занимать много места, так как они содержат все значения свойств.</span><span class="sxs-lookup"><span data-stu-id="919e0-175">Also, the delta responses tend to be large because they contain all property values.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="919e0-176">Альтернатива: получить только измененные свойства</span><span class="sxs-lookup"><span data-stu-id="919e0-176">Alternative: return only the changed properties</span></span>

<span data-ttu-id="919e0-177">Добавление заголовка запроса на необязательный - `prefer:return=minimal` -приводит к следующим образом:</span><span class="sxs-lookup"><span data-stu-id="919e0-177">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="919e0-178">При изменении свойства новое значение включается в ответе.</span><span class="sxs-lookup"><span data-stu-id="919e0-178">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="919e0-179">Этот компонент включает свойства задаются на значение null.</span><span class="sxs-lookup"><span data-stu-id="919e0-179">This includes properties being set to null value.</span></span>
- <span data-ttu-id="919e0-180">Если свойство не был изменен, свойство не включается в ответ на всех.</span><span class="sxs-lookup"><span data-stu-id="919e0-180">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="919e0-181">(Отличается от поведения по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="919e0-181">(Different from the default behavior.)</span></span>

> <span data-ttu-id="919e0-182">**Примечание:** Можно добавить заголовок `deltaLink` запроса в любой момент времени в цикле дельты.</span><span class="sxs-lookup"><span data-stu-id="919e0-182">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="919e0-183">Заголовок влияет только на набор свойств, включенных в ответ и не затрагивает как выполняется запрос дельты.</span><span class="sxs-lookup"><span data-stu-id="919e0-183">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span>

## <a name="example"></a><span data-ttu-id="919e0-184">Пример</span><span class="sxs-lookup"><span data-stu-id="919e0-184">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="919e0-185">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="919e0-185">Request 1</span></span>

<span data-ttu-id="919e0-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="919e0-186">The following is an example of the request.</span></span> <span data-ttu-id="919e0-187">Существует не `$select` параметр, поэтому по умолчанию набор свойств, отслеживаемых и возвращаются.</span><span class="sxs-lookup"><span data-stu-id="919e0-187">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
```

### <a name="response-1"></a><span data-ttu-id="919e0-188">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="919e0-188">Response 1</span></span>

<span data-ttu-id="919e0-189">Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="919e0-189">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="919e0-190">Не `isOf` был использован фильтр, поэтому возвращаются все типы, производные от directoryObject.</span><span class="sxs-lookup"><span data-stu-id="919e0-190">No `isOf` filter has been used, so all types derived from directoryObject are returned.</span></span>

><span data-ttu-id="919e0-p120">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="919e0-p120">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null,
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp",
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": ["string"],
      "city": "string",
      "companyName": "string",
      "country": "string",
      "department": "string",
      "displayName": "string",
      "givenName": "string",
      "id": "string (identifier)",
      "jobTitle": "string",
      <...response trimmed for brevity...>
    },
    <...response trimmed for brevity...>
  ]
}
```

### <a name="request-2"></a><span data-ttu-id="919e0-193">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="919e0-193">Request 2</span></span>

<span data-ttu-id="919e0-194">В следующем примере показано использование поведение альтернативный минимальной ответа:</span><span class="sxs-lookup"><span data-stu-id="919e0-194">The next example shows the use of the alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```

### <a name="response-2"></a><span data-ttu-id="919e0-195">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="919e0-195">Response 2</span></span>

<span data-ttu-id="919e0-196">Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="919e0-196">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="919e0-197">Обратите внимание, что возвращаются только свойства, которые фактически были изменены.</span><span class="sxs-lookup"><span data-stu-id="919e0-197">Note only the properties that have actually changed are returned.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "displayName": "John Smith"
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "description": null,
      "displayName": "testgp"
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": "12345"
    },
    <...response trimmed for brevity...>
  ]
}
```

### <a name="request-3"></a><span data-ttu-id="919e0-198">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="919e0-198">Request 3</span></span>

<span data-ttu-id="919e0-199">В следующем примере показано использование начального запроса `isOf` оператор для фильтрации объектов пользователей и групп:</span><span class="sxs-lookup"><span data-stu-id="919e0-199">The next example shows the initial request using the `isOf` operator to filter out only user and group entities:</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```

### <a name="response-3"></a><span data-ttu-id="919e0-200">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="919e0-200">Response 3</span></span>

<span data-ttu-id="919e0-201">Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="919e0-201">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="919e0-202">Обратите внимание на то, что возвращаются только объекты пользователей и групп:</span><span class="sxs-lookup"><span data-stu-id="919e0-202">Note that only user and group objects are returned:</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null,
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp",
      <...response trimmed for brevity...>
    },
    <...response trimmed for brevity...>
  ]
}
```

- <span data-ttu-id="919e0-203">[Использование разностного запроса для отслеживания изменений в данных Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="919e0-203">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="919e0-204">[Получение добавочные изменения для пользователей](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="919e0-204">[Get incremental changes for users](/graph/delta-query-users).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
