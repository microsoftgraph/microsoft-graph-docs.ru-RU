---
title: 'directoryObject: Delta'
description: 'Получение новых, обновленных или удаленных объектов каталога для следующих типов: User, Group и Contact Contact в едином разностном запросе. Сведения об исправлениях приведены в разделе Tracking.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 56ee662050858ff3d46b12b6885ba9e418d0e59d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455172"
---
# <a name="directoryobject-delta"></a><span data-ttu-id="bed02-104">directoryObject: Delta</span><span class="sxs-lookup"><span data-stu-id="bed02-104">directoryObject: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bed02-105">Получение новых, обновленных или удаленных объектов каталога для следующих типов: [User](../resources/user.md), [Group](../resources/group.md) и [Contact Contact](../resources/orgcontact.md)в едином разностном запросе.</span><span class="sxs-lookup"><span data-stu-id="bed02-105">Get newly created, updated, or deleted directory objects of the following types: [user](../resources/user.md), [group](../resources/group.md) and [organizational contact](../resources/orgcontact.md), in a single delta query.</span></span> <span data-ttu-id="bed02-106">Сведения [](/graph/delta-query-overview) об исправлениях приведены в разделе Tracking.</span><span class="sxs-lookup"><span data-stu-id="bed02-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="bed02-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bed02-107">Permissions</span></span>

<span data-ttu-id="bed02-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bed02-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bed02-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bed02-110">Permission type</span></span>      | <span data-ttu-id="bed02-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bed02-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bed02-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bed02-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bed02-113">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bed02-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="bed02-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bed02-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bed02-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bed02-115">Not supported.</span></span>  |
|<span data-ttu-id="bed02-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bed02-116">Application</span></span> | <span data-ttu-id="bed02-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bed02-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bed02-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bed02-118">HTTP request</span></span>

<span data-ttu-id="bed02-119">Чтобы начать отслеживание изменений, создайте запрос, включающий функцию Delta в ресурсе Директорйобжектс.</span><span class="sxs-lookup"><span data-stu-id="bed02-119">To begin tracking changes, you make a request including the delta function on the directoryObjects resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a><span data-ttu-id="bed02-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="bed02-120">Query parameters</span></span>

<span data-ttu-id="bed02-121">Отслеживание изменений приводит к округлению одного или нескольких вызовов функции **Delta** .</span><span class="sxs-lookup"><span data-stu-id="bed02-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="bed02-122">Если вы используете любой параметр запроса (кроме `$deltatoken` и `$skiptoken`), необходимо указать его в исходном запросе **Delta** .</span><span class="sxs-lookup"><span data-stu-id="bed02-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="bed02-123">Microsoft Graph автоматически кодирует все заданные параметры в часть маркера или `nextLink` `deltaLink` URL-адрес, указанный в ответе.</span><span class="sxs-lookup"><span data-stu-id="bed02-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="bed02-124">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="bed02-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="bed02-125">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="bed02-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="bed02-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="bed02-126">Query parameter</span></span> | <span data-ttu-id="bed02-127">Тип</span><span class="sxs-lookup"><span data-stu-id="bed02-127">Type</span></span> |<span data-ttu-id="bed02-128">Описание</span><span class="sxs-lookup"><span data-stu-id="bed02-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bed02-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="bed02-129">$deltatoken</span></span> | <span data-ttu-id="bed02-130">string</span><span class="sxs-lookup"><span data-stu-id="bed02-130">string</span></span> | <span data-ttu-id="bed02-p105">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции пользователей и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="bed02-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="bed02-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="bed02-133">$skiptoken</span></span> | <span data-ttu-id="bed02-134">строка</span><span class="sxs-lookup"><span data-stu-id="bed02-134">string</span></span> | <span data-ttu-id="bed02-135">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что в коллекции пользователей остаются неотслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="bed02-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="bed02-136">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="bed02-136">OData query parameters</span></span>

<span data-ttu-id="bed02-137">Этот метод поддерживает необязательные параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bed02-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="bed02-138">`$filter` С помощью специального `isOf` оператора можно фильтровать подмножество типов, производных от directoryObject.</span><span class="sxs-lookup"><span data-stu-id="bed02-138">You can use `$filter` with the special `isOf` operator to filter a subset of types derived from directoryObject.</span></span>
  - <span data-ttu-id="bed02-139">Можно объединить несколько выражений с помощью элемента `or`, который позволяет использовать одну разностную трассировку запросов нескольких типов.</span><span class="sxs-lookup"><span data-stu-id="bed02-139">You can combine multiple expressions using an `or`, which allows you to have a single delta query tracking multiple types.</span></span> <span data-ttu-id="bed02-140">Более подробную информацию можно узнать в [третьем примере](#request-3) .</span><span class="sxs-lookup"><span data-stu-id="bed02-140">See the [third example](#request-3) for details.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bed02-141">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bed02-141">Request headers</span></span>

| <span data-ttu-id="bed02-142">Имя</span><span class="sxs-lookup"><span data-stu-id="bed02-142">Name</span></span>       | <span data-ttu-id="bed02-143">Описание</span><span class="sxs-lookup"><span data-stu-id="bed02-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bed02-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="bed02-144">Authorization</span></span>  | <span data-ttu-id="bed02-145">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="bed02-145">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="bed02-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bed02-146">Content-Type</span></span>  | <span data-ttu-id="bed02-147">application/json</span><span class="sxs-lookup"><span data-stu-id="bed02-147">application/json</span></span> |
| <span data-ttu-id="bed02-148">Prefer</span><span class="sxs-lookup"><span data-stu-id="bed02-148">Prefer</span></span> | <span data-ttu-id="bed02-149">Возврат = минимум</span><span class="sxs-lookup"><span data-stu-id="bed02-149">return=minimal</span></span> <br><br><span data-ttu-id="bed02-150">При указании заголовка с запросом, который `deltaLink` использует объект, возвращаются только свойства объекта, которые были изменены с момента последнего цикла.</span><span class="sxs-lookup"><span data-stu-id="bed02-150">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="bed02-151">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bed02-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bed02-152">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bed02-152">Request body</span></span>

<span data-ttu-id="bed02-153">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bed02-153">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="bed02-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="bed02-154">Response</span></span>

<span data-ttu-id="bed02-155">В случае успеха этот метод возвращает код ответа `200 OK` и объект коллекции [user](../resources/directoryobject.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bed02-155">If successful, this method returns `200 OK` response code and [user](../resources/directoryobject.md) collection object in the response body.</span></span> <span data-ttu-id="bed02-156">В ответ также включается `nextLink` URL-адрес `deltaLink` или URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="bed02-156">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="bed02-157">Если возвращается `nextLink` URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="bed02-157">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="bed02-158">Это указывает на необходимость извлечения дополнительных страниц данных в сеансе.</span><span class="sxs-lookup"><span data-stu-id="bed02-158">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="bed02-159">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="bed02-159">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="bed02-160">Ответ включает тот же набор свойств, что и в исходном запросе на разностный запрос.</span><span class="sxs-lookup"><span data-stu-id="bed02-160">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="bed02-161">Это позволяет захватить полное текущее состояние объектов при инициации разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="bed02-161">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="bed02-162">Если возвращается `deltaLink` URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="bed02-162">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="bed02-163">Это указывает на то, что больше нет данных о существующем состоянии ресурса, который необходимо возвратить.</span><span class="sxs-lookup"><span data-stu-id="bed02-163">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="bed02-164">Сохраните и используйте `deltaLink` URL-адрес, чтобы узнать об изменениях ресурса в следующем цикле.</span><span class="sxs-lookup"><span data-stu-id="bed02-164">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="bed02-165">Вы можете указать `Prefer:return=minimal` заголовок, чтобы включить в значения отклика только те свойства, которые были изменены с момента `deltaLink` выпуска.</span><span class="sxs-lookup"><span data-stu-id="bed02-165">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="bed02-166">По умолчанию: возврат тех же свойств, что и исходный запрос Дельта</span><span class="sxs-lookup"><span data-stu-id="bed02-166">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="bed02-167">По умолчанию запросы, использующие `deltaLink` или `nextLink` возвращающие те же свойства, что и выбранные в начальном запросе Дельта, запрашиваются следующими способами:</span><span class="sxs-lookup"><span data-stu-id="bed02-167">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="bed02-168">Если свойство изменилось, в ответ включается новое значение.</span><span class="sxs-lookup"><span data-stu-id="bed02-168">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="bed02-169">Сюда входят свойства, для которых задано значение null.</span><span class="sxs-lookup"><span data-stu-id="bed02-169">This includes properties being set to null value.</span></span>
- <span data-ttu-id="bed02-170">Если свойство не изменилось, в ответ включается старое значение.</span><span class="sxs-lookup"><span data-stu-id="bed02-170">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="bed02-171">Если свойство никогда не задается до тех пор, пока оно не будет включено в ответ вообще.</span><span class="sxs-lookup"><span data-stu-id="bed02-171">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="bed02-172">**Примечание:** Таким образом, изучив ответ, можно определить, изменяется ли свойство.</span><span class="sxs-lookup"><span data-stu-id="bed02-172">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="bed02-173">Кроме того, разностные ответы обычно имеют большой размер, так как они содержат все значения свойств.</span><span class="sxs-lookup"><span data-stu-id="bed02-173">Also, the delta responses tend to be large because they contain all property values.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="bed02-174">Альтернатива: возврат только измененных свойств</span><span class="sxs-lookup"><span data-stu-id="bed02-174">Alternative: return only the changed properties</span></span>

<span data-ttu-id="bed02-175">Добавление необязательного заголовка запроса `prefer:return=minimal` — приводит к следующему поведению:</span><span class="sxs-lookup"><span data-stu-id="bed02-175">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="bed02-176">Если свойство изменилось, в ответ включается новое значение.</span><span class="sxs-lookup"><span data-stu-id="bed02-176">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="bed02-177">Сюда входят свойства, для которых задано значение null.</span><span class="sxs-lookup"><span data-stu-id="bed02-177">This includes properties being set to null value.</span></span>
- <span data-ttu-id="bed02-178">Если свойство не изменилось, свойство не включается в ответ вообще.</span><span class="sxs-lookup"><span data-stu-id="bed02-178">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="bed02-179">(Отличается от поведения по умолчанию.)</span><span class="sxs-lookup"><span data-stu-id="bed02-179">(Different from the default behavior.)</span></span>

> <span data-ttu-id="bed02-180">**Примечание:** Заголовок можно добавить в `deltaLink` запрос в любой момент времени в разностном цикле.</span><span class="sxs-lookup"><span data-stu-id="bed02-180">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="bed02-181">Заголовок влияет только на набор свойств, включенных в ответ, и не влияет на то, как выполняется разностный запрос.</span><span class="sxs-lookup"><span data-stu-id="bed02-181">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span>

## <a name="example"></a><span data-ttu-id="bed02-182">Пример</span><span class="sxs-lookup"><span data-stu-id="bed02-182">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="bed02-183">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="bed02-183">Request 1</span></span>

<span data-ttu-id="bed02-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bed02-184">The following is an example of the request.</span></span> <span data-ttu-id="bed02-185">Параметр не `$select` задан, поэтому набор свойств по умолчанию отслеживается и возвращается.</span><span class="sxs-lookup"><span data-stu-id="bed02-185">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
```

### <a name="response-1"></a><span data-ttu-id="bed02-186">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="bed02-186">Response 1</span></span>

<span data-ttu-id="bed02-187">Ниже приведен пример ответа, полученного при использовании метода `deltaLink` , полученного при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="bed02-187">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="bed02-188">Фильтр `isOf` не использовался, поэтому возвращаются все типы, производные от directoryObject.</span><span class="sxs-lookup"><span data-stu-id="bed02-188">No `isOf` filter has been used, so all types derived from directoryObject are returned.</span></span>

><span data-ttu-id="bed02-189">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bed02-189">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bed02-190">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bed02-190">All the properties will be returned from an actual call.</span></span>

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

### <a name="request-2"></a><span data-ttu-id="bed02-191">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="bed02-191">Request 2</span></span>

<span data-ttu-id="bed02-192">В следующем примере показано использование альтернативного поведения минимального ответа:</span><span class="sxs-lookup"><span data-stu-id="bed02-192">The next example shows the use of the alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```

### <a name="response-2"></a><span data-ttu-id="bed02-193">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="bed02-193">Response 2</span></span>

<span data-ttu-id="bed02-194">Ниже приведен пример ответа, полученного при использовании метода `deltaLink` , полученного при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="bed02-194">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="bed02-195">Обратите внимание, что возвращаются только те свойства, которые действительно изменились.</span><span class="sxs-lookup"><span data-stu-id="bed02-195">Note only the properties that have actually changed are returned.</span></span>

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

### <a name="request-3"></a><span data-ttu-id="bed02-196">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="bed02-196">Request 3</span></span>

<span data-ttu-id="bed02-197">В следующем примере показан начальный запрос с помощью `isOf` оператора для фильтрации только сущностей "пользователь" и "Группа":</span><span class="sxs-lookup"><span data-stu-id="bed02-197">The next example shows the initial request using the `isOf` operator to filter out only user and group entities:</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```

### <a name="response-3"></a><span data-ttu-id="bed02-198">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="bed02-198">Response 3</span></span>

<span data-ttu-id="bed02-199">Ниже приведен пример ответа, полученного при использовании метода `deltaLink` , полученного при инициализации запроса.</span><span class="sxs-lookup"><span data-stu-id="bed02-199">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="bed02-200">Обратите внимание, что возвращаются только объекты user и Group:</span><span class="sxs-lookup"><span data-stu-id="bed02-200">Note that only user and group objects are returned:</span></span>

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

- <span data-ttu-id="bed02-201">[Использование запроса изменений для отслеживания изменений в данных Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="bed02-201">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="bed02-202">[Получение добавочных изменений для пользователей](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="bed02-202">[Get incremental changes for users](/graph/delta-query-users).</span></span>

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
    "Error: /api-reference/beta/api/directoryobject-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
