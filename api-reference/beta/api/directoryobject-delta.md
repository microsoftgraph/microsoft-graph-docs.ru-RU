---
title: 'directoryObject: delta'
description: 'Получите вновь созданные, обновленные или удаленные объекты каталога следующих типов: пользовательский, групповой и организационный контакт в одном запросе дельты. Дополнительные сведения см. в статье "Отслеживание изменений".'
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 88a78e85d640c5d6e5c62fef239f29485d820897
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946654"
---
# <a name="directoryobject-delta"></a><span data-ttu-id="aa832-104">directoryObject: delta</span><span class="sxs-lookup"><span data-stu-id="aa832-104">directoryObject: delta</span></span>

<span data-ttu-id="aa832-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa832-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa832-106">Получите вновь созданные, обновленные или удаленные объекты каталога следующих [типов:](../resources/user.md) [пользовательский,](../resources/group.md) групповой и организационный контакт [в](../resources/orgcontact.md)одном запросе дельты.</span><span class="sxs-lookup"><span data-stu-id="aa832-106">Get newly created, updated, or deleted directory objects of the following types: [user](../resources/user.md), [group](../resources/group.md) and [organizational contact](../resources/orgcontact.md), in a single delta query.</span></span> <span data-ttu-id="aa832-107">Дополнительные сведения см. в статье [Отслеживание изменений](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="aa832-107">See [change tracking](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa832-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa832-108">Permissions</span></span>

<span data-ttu-id="aa832-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa832-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa832-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa832-111">Permission type</span></span>      | <span data-ttu-id="aa832-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa832-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa832-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa832-113">Delegated (work or school account)</span></span> | <span data-ttu-id="aa832-114">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aa832-114">Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="aa832-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa832-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa832-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa832-116">Not supported.</span></span>  |
|<span data-ttu-id="aa832-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa832-117">Application</span></span> | <span data-ttu-id="aa832-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa832-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa832-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa832-119">HTTP request</span></span>

<span data-ttu-id="aa832-120">Чтобы начать отслеживание изменений, необходимо сделать запрос, включив функцию дельты на ресурсе directoryObjects.</span><span class="sxs-lookup"><span data-stu-id="aa832-120">To begin tracking changes, you make a request including the delta function on the directoryObjects resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a><span data-ttu-id="aa832-121">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="aa832-121">Query parameters</span></span>

<span data-ttu-id="aa832-122">Отслеживание изменений вызывает один или несколько вызовов функции **дельты.**</span><span class="sxs-lookup"><span data-stu-id="aa832-122">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="aa832-123">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="aa832-123">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="aa832-124">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="aa832-124">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="aa832-125">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="aa832-125">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="aa832-126">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="aa832-126">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="aa832-127">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="aa832-127">Query parameter</span></span> | <span data-ttu-id="aa832-128">Тип</span><span class="sxs-lookup"><span data-stu-id="aa832-128">Type</span></span> |<span data-ttu-id="aa832-129">Описание</span><span class="sxs-lookup"><span data-stu-id="aa832-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aa832-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="aa832-130">$deltatoken</span></span> | <span data-ttu-id="aa832-131">string</span><span class="sxs-lookup"><span data-stu-id="aa832-131">string</span></span> | <span data-ttu-id="aa832-p105">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции пользователей и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим маркером и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="aa832-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="aa832-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="aa832-134">$skiptoken</span></span> | <span data-ttu-id="aa832-135">строка</span><span class="sxs-lookup"><span data-stu-id="aa832-135">string</span></span> | <span data-ttu-id="aa832-136">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что в коллекции пользователей остаются неотслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="aa832-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="aa832-137">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="aa832-137">OData query parameters</span></span>

<span data-ttu-id="aa832-138">Этот метод поддерживает необязательные параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="aa832-138">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="aa832-139">С помощью специального оператора можно `$filter` `isOf` отфильтровать подмножество типов, полученных из directoryObject.</span><span class="sxs-lookup"><span data-stu-id="aa832-139">You can use `$filter` with the special `isOf` operator to filter a subset of types derived from directoryObject.</span></span>
  - <span data-ttu-id="aa832-140">Вы можете объединить несколько выражений с помощью одного запроса дельты, отслеживая `or` несколько типов.</span><span class="sxs-lookup"><span data-stu-id="aa832-140">You can combine multiple expressions using an `or`, which allows you to have a single delta query tracking multiple types.</span></span> <span data-ttu-id="aa832-141">Сведения [см. в третьем](#request-3) примере.</span><span class="sxs-lookup"><span data-stu-id="aa832-141">See the [third example](#request-3) for details.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa832-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa832-142">Request headers</span></span>

| <span data-ttu-id="aa832-143">Имя</span><span class="sxs-lookup"><span data-stu-id="aa832-143">Name</span></span>       | <span data-ttu-id="aa832-144">Описание</span><span class="sxs-lookup"><span data-stu-id="aa832-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aa832-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa832-145">Authorization</span></span>  | <span data-ttu-id="aa832-146">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="aa832-146">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="aa832-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aa832-147">Content-Type</span></span>  | <span data-ttu-id="aa832-148">application/json</span><span class="sxs-lookup"><span data-stu-id="aa832-148">application/json</span></span> |
| <span data-ttu-id="aa832-149">Prefer</span><span class="sxs-lookup"><span data-stu-id="aa832-149">Prefer</span></span> | <span data-ttu-id="aa832-150">return=minimal</span><span class="sxs-lookup"><span data-stu-id="aa832-150">return=minimal</span></span> <br><br><span data-ttu-id="aa832-151">Указание этого заголовка с запросом, использующим параметр `deltaLink`, приведет к возвращению только свойств объекта, измененных с момента последнего цикла.</span><span class="sxs-lookup"><span data-stu-id="aa832-151">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="aa832-152">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="aa832-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa832-153">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa832-153">Request body</span></span>

<span data-ttu-id="aa832-154">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa832-154">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="aa832-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa832-155">Response</span></span>

<span data-ttu-id="aa832-156">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции [user](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa832-156">If successful, this method returns `200 OK` response code and [user](../resources/directoryobject.md) collection object in the response body.</span></span> <span data-ttu-id="aa832-157">Оклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="aa832-157">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="aa832-158">Если возвращается URL-адрес `nextLink`:</span><span class="sxs-lookup"><span data-stu-id="aa832-158">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="aa832-159">Это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="aa832-159">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="aa832-160">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в отклик не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="aa832-160">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="aa832-161">Отклик включает тот же набор свойств, что и начальный разностный запрос.</span><span class="sxs-lookup"><span data-stu-id="aa832-161">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="aa832-162">Это позволяет фиксировать полное текущее состояние объектов при запуске разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="aa832-162">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="aa832-163">Если возвращается URL-адрес `deltaLink`:</span><span class="sxs-lookup"><span data-stu-id="aa832-163">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="aa832-164">Это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="aa832-164">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="aa832-165">Сохраните и используйте URL-адрес `deltaLink`, чтобы узнавать об изменениях ресурса в следующем цикле.</span><span class="sxs-lookup"><span data-stu-id="aa832-165">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="aa832-166">Вы можете указать заголовок `Prefer:return=minimal`, чтобы включить в значения отклика только свойства, измененные с момента создания `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="aa832-166">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="aa832-167">По умолчанию: возвращение свойств, совпадающих с начальным разностным запросом</span><span class="sxs-lookup"><span data-stu-id="aa832-167">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="aa832-168">По умолчанию запросы с использованием `deltaLink` или `nextLink` возвращают те же свойства, которые выбраны в начальном разностном запросе, следующим образом:</span><span class="sxs-lookup"><span data-stu-id="aa832-168">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="aa832-169">Если свойство изменилось, в отклике содержится новое значение.</span><span class="sxs-lookup"><span data-stu-id="aa832-169">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="aa832-170">Сюда включаются свойства с заданным значением NULL.</span><span class="sxs-lookup"><span data-stu-id="aa832-170">This includes properties being set to null value.</span></span>
- <span data-ttu-id="aa832-171">Если свойство не изменилось, в отклике содержится старое значение.</span><span class="sxs-lookup"><span data-stu-id="aa832-171">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="aa832-172">Если свойство ранее никогда не настраивалось, оно не включается в отклик.</span><span class="sxs-lookup"><span data-stu-id="aa832-172">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="aa832-173">**Примечание.** При таком поведении просмотр отклика не дает возможность определить, изменилось ли свойство.</span><span class="sxs-lookup"><span data-stu-id="aa832-173">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="aa832-174">Кроме того, ответы дельты, как правило, большие, так как они содержат все значения свойств.</span><span class="sxs-lookup"><span data-stu-id="aa832-174">Also, the delta responses tend to be large because they contain all property values.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="aa832-175">Альтернатива: возвращение только измененных свойств</span><span class="sxs-lookup"><span data-stu-id="aa832-175">Alternative: return only the changed properties</span></span>

<span data-ttu-id="aa832-176">Добавление необязательного заголовка запроса `prefer:return=minimal` приводит к следующему результату:</span><span class="sxs-lookup"><span data-stu-id="aa832-176">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="aa832-177">Если свойство изменилось, в отклике содержится новое значение.</span><span class="sxs-lookup"><span data-stu-id="aa832-177">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="aa832-178">Сюда включаются свойства с заданным значением NULL.</span><span class="sxs-lookup"><span data-stu-id="aa832-178">This includes properties being set to null value.</span></span>
- <span data-ttu-id="aa832-179">Если свойство не изменилось, оно не включается в отклик.</span><span class="sxs-lookup"><span data-stu-id="aa832-179">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="aa832-180">(Отличается от поведения по умолчанию.)</span><span class="sxs-lookup"><span data-stu-id="aa832-180">(Different from the default behavior.)</span></span>

> <span data-ttu-id="aa832-181">**Примечание.** Заголовок можно добавить в запрос `deltaLink` в любой момент разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="aa832-181">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="aa832-182">Заголовок влияет только на набор свойств, включенный в отклик, и не влияет на способ выполнения разностного запроса.</span><span class="sxs-lookup"><span data-stu-id="aa832-182">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span>

## <a name="example"></a><span data-ttu-id="aa832-183">Пример</span><span class="sxs-lookup"><span data-stu-id="aa832-183">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="aa832-184">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="aa832-184">Request 1</span></span>

<span data-ttu-id="aa832-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa832-185">The following is an example of the request.</span></span> <span data-ttu-id="aa832-186">Параметр `$select` отсутствует, поэтому отслеживается и возвращается набор свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="aa832-186">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="aa832-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa832-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directory_object_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/delta
```
# <a name="c"></a>[<span data-ttu-id="aa832-188">C#</span><span class="sxs-lookup"><span data-stu-id="aa832-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directory-object-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa832-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa832-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directory-object-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa832-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa832-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directory-object-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa832-191">Java</span><span class="sxs-lookup"><span data-stu-id="aa832-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directory-object-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-1"></a><span data-ttu-id="aa832-192">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="aa832-192">Response 1</span></span>

<span data-ttu-id="aa832-193">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="aa832-193">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="aa832-194">Фильтр не используется, поэтому возвращаются все типы, полученные из `isOf` directoryObject.</span><span class="sxs-lookup"><span data-stu-id="aa832-194">No `isOf` filter has been used, so all types derived from directoryObject are returned.</span></span>

><span data-ttu-id="aa832-195">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="aa832-195">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="aa832-196">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa832-196">All the properties will be returned from an actual call.</span></span>

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
      "jobTitle": null
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp"
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
      "jobTitle": "string"
    }
  ]
}
```

### <a name="request-2"></a><span data-ttu-id="aa832-197">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="aa832-197">Request 2</span></span>

<span data-ttu-id="aa832-198">В следующем примере показано использование альтернативного минимального поведения отклика:</span><span class="sxs-lookup"><span data-stu-id="aa832-198">The next example shows the use of the alternative minimal response behavior:</span></span>

# <a name="http"></a>[<span data-ttu-id="aa832-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa832-199">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```
# <a name="c"></a>[<span data-ttu-id="aa832-200">C#</span><span class="sxs-lookup"><span data-stu-id="aa832-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa832-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa832-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa832-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa832-202">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa832-203">Java</span><span class="sxs-lookup"><span data-stu-id="aa832-203">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-2"></a><span data-ttu-id="aa832-204">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="aa832-204">Response 2</span></span>

<span data-ttu-id="aa832-205">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="aa832-205">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="aa832-206">Обратите внимание, что возвращаются только фактически измененные свойства.</span><span class="sxs-lookup"><span data-stu-id="aa832-206">Note only the properties that have actually changed are returned.</span></span>

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
    }
  ]
}
```

### <a name="request-3"></a><span data-ttu-id="aa832-207">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="aa832-207">Request 3</span></span>

<span data-ttu-id="aa832-208">В следующем примере показан начальный запрос с помощью оператора для фильтрации только `isOf` пользовательских и групповых сущностями:</span><span class="sxs-lookup"><span data-stu-id="aa832-208">The next example shows the initial request using the `isOf` operator to filter out only user and group entities:</span></span>

# <a name="http"></a>[<span data-ttu-id="aa832-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa832-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```
# <a name="c"></a>[<span data-ttu-id="aa832-210">C#</span><span class="sxs-lookup"><span data-stu-id="aa832-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa832-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa832-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa832-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa832-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa832-213">Java</span><span class="sxs-lookup"><span data-stu-id="aa832-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-3"></a><span data-ttu-id="aa832-214">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="aa832-214">Response 3</span></span>

<span data-ttu-id="aa832-215">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="aa832-215">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="aa832-216">Обратите внимание, что возвращаются только объекты пользователя и группы:</span><span class="sxs-lookup"><span data-stu-id="aa832-216">Note that only user and group objects are returned:</span></span>

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
      "jobTitle": null
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp"
    }
  ]
}
```

- <span data-ttu-id="aa832-217">[Отслеживание изменений в данных Microsoft Graph с помощью разностного запроса](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="aa832-217">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="aa832-218">[Получение добавочных изменений для пользователей](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="aa832-218">[Get incremental changes for users](/graph/delta-query-users).</span></span>

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


