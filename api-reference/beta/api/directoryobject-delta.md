---
title: 'directoryObject: Delta'
description: 'Получение новых, обновленных или удаленных объектов каталога для следующих типов: User, Group и Contact Contact в едином разностном запросе. Дополнительные сведения см. в статье "Отслеживание изменений".'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f3c547d9589c2b94e261113fafca8adc2f70f688
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718228"
---
# <a name="directoryobject-delta"></a><span data-ttu-id="bcc0d-104">directoryObject: Delta</span><span class="sxs-lookup"><span data-stu-id="bcc0d-104">directoryObject: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcc0d-105">Получение новых, обновленных или удаленных объектов каталога для следующих типов: [User](../resources/user.md), [Group](../resources/group.md) и [Contact Contact](../resources/orgcontact.md)в едином разностном запросе.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-105">Get newly created, updated, or deleted directory objects of the following types: [user](../resources/user.md), [group](../resources/group.md) and [organizational contact](../resources/orgcontact.md), in a single delta query.</span></span> <span data-ttu-id="bcc0d-106">Дополнительные сведения см. в статье [Отслеживание изменений](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="bcc0d-106">See [Track changes](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcc0d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bcc0d-107">Permissions</span></span>

<span data-ttu-id="bcc0d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcc0d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcc0d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcc0d-110">Permission type</span></span>      | <span data-ttu-id="bcc0d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcc0d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcc0d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcc0d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bcc0d-113">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bcc0d-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="bcc0d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcc0d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcc0d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-115">Not supported.</span></span>  |
|<span data-ttu-id="bcc0d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcc0d-116">Application</span></span> | <span data-ttu-id="bcc0d-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcc0d-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcc0d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcc0d-118">HTTP request</span></span>

<span data-ttu-id="bcc0d-119">Чтобы начать отслеживание изменений, создайте запрос, включающий функцию Delta в ресурсе Директорйобжектс.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-119">To begin tracking changes, you make a request including the delta function on the directoryObjects resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a><span data-ttu-id="bcc0d-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="bcc0d-120">Query parameters</span></span>

<span data-ttu-id="bcc0d-121">Отслеживание изменений приводит к округлению одного или нескольких вызовов функции **Delta** .</span><span class="sxs-lookup"><span data-stu-id="bcc0d-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="bcc0d-122">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="bcc0d-123">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="bcc0d-124">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-124">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="bcc0d-125">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="bcc0d-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="bcc0d-126">Query parameter</span></span> | <span data-ttu-id="bcc0d-127">Тип</span><span class="sxs-lookup"><span data-stu-id="bcc0d-127">Type</span></span> |<span data-ttu-id="bcc0d-128">Описание</span><span class="sxs-lookup"><span data-stu-id="bcc0d-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bcc0d-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="bcc0d-129">$deltatoken</span></span> | <span data-ttu-id="bcc0d-130">string</span><span class="sxs-lookup"><span data-stu-id="bcc0d-130">string</span></span> | <span data-ttu-id="bcc0d-p105">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции пользователей и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим маркером и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="bcc0d-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="bcc0d-133">$skiptoken</span></span> | <span data-ttu-id="bcc0d-134">строка</span><span class="sxs-lookup"><span data-stu-id="bcc0d-134">string</span></span> | <span data-ttu-id="bcc0d-135">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что в коллекции пользователей остаются неотслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="bcc0d-136">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="bcc0d-136">OData query parameters</span></span>

<span data-ttu-id="bcc0d-137">Этот метод поддерживает необязательные параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-137">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="bcc0d-138">`$filter` С помощью специального `isOf` оператора можно фильтровать подмножество типов, производных от directoryObject.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-138">You can use `$filter` with the special `isOf` operator to filter a subset of types derived from directoryObject.</span></span>
  - <span data-ttu-id="bcc0d-139">Можно объединить несколько выражений с помощью элемента `or`, который позволяет использовать одну разностную трассировку запросов нескольких типов.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-139">You can combine multiple expressions using an `or`, which allows you to have a single delta query tracking multiple types.</span></span> <span data-ttu-id="bcc0d-140">Более подробную информацию можно узнать в [третьем примере](#request-3) .</span><span class="sxs-lookup"><span data-stu-id="bcc0d-140">See the [third example](#request-3) for details.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bcc0d-141">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcc0d-141">Request headers</span></span>

| <span data-ttu-id="bcc0d-142">Имя</span><span class="sxs-lookup"><span data-stu-id="bcc0d-142">Name</span></span>       | <span data-ttu-id="bcc0d-143">Описание</span><span class="sxs-lookup"><span data-stu-id="bcc0d-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bcc0d-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcc0d-144">Authorization</span></span>  | <span data-ttu-id="bcc0d-145">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="bcc0d-145">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="bcc0d-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bcc0d-146">Content-Type</span></span>  | <span data-ttu-id="bcc0d-147">application/json</span><span class="sxs-lookup"><span data-stu-id="bcc0d-147">application/json</span></span> |
| <span data-ttu-id="bcc0d-148">Prefer</span><span class="sxs-lookup"><span data-stu-id="bcc0d-148">Prefer</span></span> | <span data-ttu-id="bcc0d-149">return=minimal</span><span class="sxs-lookup"><span data-stu-id="bcc0d-149">return=minimal</span></span> <br><br><span data-ttu-id="bcc0d-150">Указание этого заголовка с запросом, использующим параметр `deltaLink`, приведет к возвращению только свойств объекта, измененных с момента последнего цикла.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-150">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="bcc0d-151">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcc0d-152">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bcc0d-152">Request body</span></span>

<span data-ttu-id="bcc0d-153">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-153">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="bcc0d-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcc0d-154">Response</span></span>

<span data-ttu-id="bcc0d-155">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции [user](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-155">If successful, this method returns `200 OK` response code and [user](../resources/directoryobject.md) collection object in the response body.</span></span> <span data-ttu-id="bcc0d-156">Оклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-156">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="bcc0d-157">Если возвращается URL-адрес `nextLink`:</span><span class="sxs-lookup"><span data-stu-id="bcc0d-157">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="bcc0d-158">Это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-158">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="bcc0d-159">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в отклик не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-159">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="bcc0d-160">Отклик включает тот же набор свойств, что и начальный разностный запрос.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-160">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="bcc0d-161">Это позволяет фиксировать полное текущее состояние объектов при запуске разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-161">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="bcc0d-162">Если возвращается URL-адрес `deltaLink`:</span><span class="sxs-lookup"><span data-stu-id="bcc0d-162">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="bcc0d-163">Это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-163">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="bcc0d-164">Сохраните и используйте URL-адрес `deltaLink`, чтобы узнавать об изменениях ресурса в следующем цикле.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-164">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="bcc0d-165">Вы можете указать заголовок `Prefer:return=minimal`, чтобы включить в значения отклика только свойства, измененные с момента создания `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-165">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="bcc0d-166">По умолчанию: возвращение свойств, совпадающих с начальным разностным запросом</span><span class="sxs-lookup"><span data-stu-id="bcc0d-166">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="bcc0d-167">По умолчанию запросы с использованием `deltaLink` или `nextLink` возвращают те же свойства, которые выбраны в начальном разностном запросе, следующим образом:</span><span class="sxs-lookup"><span data-stu-id="bcc0d-167">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="bcc0d-168">Если свойство изменилось, в отклике содержится новое значение.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-168">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="bcc0d-169">Сюда включаются свойства с заданным значением NULL.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-169">This includes properties being set to null value.</span></span>
- <span data-ttu-id="bcc0d-170">Если свойство не изменилось, в отклике содержится старое значение.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-170">If the property has not changed, the old value is included in the response.</span></span>
- <span data-ttu-id="bcc0d-171">Если свойство ранее никогда не настраивалось, оно не включается в отклик.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-171">If the property has never been set before it will not be included in the response at all.</span></span>


> <span data-ttu-id="bcc0d-172">**Примечание.** При таком поведении просмотр отклика не дает возможность определить, изменилось ли свойство.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-172">**Note:** With this behavior, by looking at the response it is not possible to tell whether a property is changing or not.</span></span> <span data-ttu-id="bcc0d-173">Кроме того, разностные ответы обычно имеют большой размер, так как они содержат все значения свойств.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-173">Also, the delta responses tend to be large because they contain all property values.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="bcc0d-174">Альтернатива: возвращение только измененных свойств</span><span class="sxs-lookup"><span data-stu-id="bcc0d-174">Alternative: return only the changed properties</span></span>

<span data-ttu-id="bcc0d-175">Добавление необязательного заголовка запроса `prefer:return=minimal` приводит к следующему результату:</span><span class="sxs-lookup"><span data-stu-id="bcc0d-175">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="bcc0d-176">Если свойство изменилось, в отклике содержится новое значение.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-176">If the property has changed, the new value is included in the response.</span></span> <span data-ttu-id="bcc0d-177">Сюда включаются свойства с заданным значением NULL.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-177">This includes properties being set to null value.</span></span>
- <span data-ttu-id="bcc0d-178">Если свойство не изменилось, оно не включается в отклик.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-178">If the property has not changed, the property is not included in the response at all.</span></span> <span data-ttu-id="bcc0d-179">(Отличается от поведения по умолчанию.)</span><span class="sxs-lookup"><span data-stu-id="bcc0d-179">(Different from the default behavior.)</span></span>

> <span data-ttu-id="bcc0d-180">**Примечание.** Заголовок можно добавить в запрос `deltaLink` в любой момент разностного цикла.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-180">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="bcc0d-181">Заголовок влияет только на набор свойств, включенный в отклик, и не влияет на способ выполнения разностного запроса.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-181">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span>

## <a name="example"></a><span data-ttu-id="bcc0d-182">Пример</span><span class="sxs-lookup"><span data-stu-id="bcc0d-182">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="bcc0d-183">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="bcc0d-183">Request 1</span></span>

<span data-ttu-id="bcc0d-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-184">The following is an example of the request.</span></span> <span data-ttu-id="bcc0d-185">Параметр `$select` отсутствует, поэтому отслеживается и возвращается набор свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-185">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bcc0d-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcc0d-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directory_object_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/delta
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bcc0d-187">C#</span><span class="sxs-lookup"><span data-stu-id="bcc0d-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directory-object-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bcc0d-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcc0d-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directory-object-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bcc0d-189">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bcc0d-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directory-object-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-1"></a><span data-ttu-id="bcc0d-190">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="bcc0d-190">Response 1</span></span>

<span data-ttu-id="bcc0d-191">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-191">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="bcc0d-192">Фильтр `isOf` не использовался, поэтому возвращаются все типы, производные от directoryObject.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-192">No `isOf` filter has been used, so all types derived from directoryObject are returned.</span></span>

><span data-ttu-id="bcc0d-193">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bcc0d-194">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-194">All the properties will be returned from an actual call.</span></span>

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

### <a name="request-2"></a><span data-ttu-id="bcc0d-195">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="bcc0d-195">Request 2</span></span>

<span data-ttu-id="bcc0d-196">В следующем примере показано использование альтернативного поведения минимального ответа:</span><span class="sxs-lookup"><span data-stu-id="bcc0d-196">The next example shows the use of the alternative minimal response behavior:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bcc0d-197">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcc0d-197">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bcc0d-198">C#</span><span class="sxs-lookup"><span data-stu-id="bcc0d-198">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bcc0d-199">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcc0d-199">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bcc0d-200">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bcc0d-200">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-2"></a><span data-ttu-id="bcc0d-201">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="bcc0d-201">Response 2</span></span>

<span data-ttu-id="bcc0d-202">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-202">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="bcc0d-203">Обратите внимание, что возвращаются только те свойства, которые действительно изменились.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-203">Note only the properties that have actually changed are returned.</span></span>

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

### <a name="request-3"></a><span data-ttu-id="bcc0d-204">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="bcc0d-204">Request 3</span></span>

<span data-ttu-id="bcc0d-205">В следующем примере показан начальный запрос с помощью `isOf` оператора для фильтрации только сущностей "пользователь" и "Группа":</span><span class="sxs-lookup"><span data-stu-id="bcc0d-205">The next example shows the initial request using the `isOf` operator to filter out only user and group entities:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bcc0d-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcc0d-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bcc0d-207">C#</span><span class="sxs-lookup"><span data-stu-id="bcc0d-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bcc0d-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcc0d-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bcc0d-209">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bcc0d-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-3"></a><span data-ttu-id="bcc0d-210">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="bcc0d-210">Response 3</span></span>

<span data-ttu-id="bcc0d-211">Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса.</span><span class="sxs-lookup"><span data-stu-id="bcc0d-211">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="bcc0d-212">Обратите внимание, что возвращаются только объекты user и Group:</span><span class="sxs-lookup"><span data-stu-id="bcc0d-212">Note that only user and group objects are returned:</span></span>

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

- <span data-ttu-id="bcc0d-213">[Отслеживание изменений в данных Microsoft Graph с помощью разностного запроса](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="bcc0d-213">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>
- <span data-ttu-id="bcc0d-214">[Получение добавочных изменений для пользователей](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="bcc0d-214">[Get incremental changes for users](/graph/delta-query-users).</span></span>

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
