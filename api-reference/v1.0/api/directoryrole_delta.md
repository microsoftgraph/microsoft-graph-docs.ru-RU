# <a name="directoryrole-delta"></a><span data-ttu-id="02387-101">directoryRole: дельты</span><span class="sxs-lookup"><span data-stu-id="02387-101">directoryRole: delta</span></span>

<span data-ttu-id="02387-102">Get вновь созданные, обновлении или удалении роли каталога без выполнения полного чтения коллекции всей ресурсов.</span><span class="sxs-lookup"><span data-stu-id="02387-102">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="02387-103">Для получения дополнительных сведений в разделе [С помощью запроса дельты](../../../concepts/delta_query_overview.md) .</span><span class="sxs-lookup"><span data-stu-id="02387-103">See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="02387-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02387-104">Permissions</span></span>

<span data-ttu-id="02387-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="02387-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="02387-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02387-107">Permission type</span></span>      | <span data-ttu-id="02387-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02387-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02387-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02387-109">Delegated (work or school account)</span></span> | <span data-ttu-id="02387-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="02387-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="02387-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02387-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02387-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02387-112">Not supported.</span></span>    |
|<span data-ttu-id="02387-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02387-113">Application</span></span> | <span data-ttu-id="02387-114">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02387-114">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02387-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02387-115">HTTP request</span></span>

<span data-ttu-id="02387-116">Чтобы начать отслеживание изменений, внесите запроса, включая функцию **дельты** на [directoryRole](../resources/directoryrole.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="02387-116">To begin tracking changes, you make a request including the **delta** function on the [directoryRole](../resources/directoryrole.md) resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

## <a name="query-parameters"></a><span data-ttu-id="02387-117">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="02387-117">Query parameters</span></span>

<span data-ttu-id="02387-118">Отслеживание изменений приводит к round один или несколько вызовов функций **дельты** .</span><span class="sxs-lookup"><span data-stu-id="02387-118">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="02387-119">При использовании любого параметра запроса (отличный от `$deltatoken` и `$skiptoken`), необходимо указать его в запрос начальной **дельты** .</span><span class="sxs-lookup"><span data-stu-id="02387-119">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="02387-120">Microsoft Graph автоматически Кодирует указанный параметров в маркеров часть `nextLink` или `deltaLink` URL-адреса, приведенные в ответе.</span><span class="sxs-lookup"><span data-stu-id="02387-120">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="02387-121">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="02387-121">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="02387-122">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="02387-122">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="02387-123">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="02387-123">Query parameter</span></span>      | <span data-ttu-id="02387-124">Тип</span><span class="sxs-lookup"><span data-stu-id="02387-124">Type</span></span>   |<span data-ttu-id="02387-125">Описание</span><span class="sxs-lookup"><span data-stu-id="02387-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="02387-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="02387-126">$deltatoken</span></span> | <span data-ttu-id="02387-127">строка</span><span class="sxs-lookup"><span data-stu-id="02387-127">string</span></span> | <span data-ttu-id="02387-128">[Состояние токен](../../../concepts/delta_query_overview.md) , возвращенный в `deltaLink` URL-адрес предыдущей вызов функции **дельты** для одной коллекции ресурсов, указывающее, завершения этого цикла отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="02387-128">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="02387-129">Сохранить и применить весь `deltaLink` URL-адрес, включая этот маркер в первый запрос следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="02387-129">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="02387-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="02387-130">$skiptoken</span></span> | <span data-ttu-id="02387-131">строка</span><span class="sxs-lookup"><span data-stu-id="02387-131">string</span></span> | <span data-ttu-id="02387-132">[Состояние токен](../../../concepts/delta_query_overview.md) , возвращенный в `nextLink` URL-адрес предыдущей вызов функции **дельты** , показывающее, есть дополнительные изменения в отслеживаются в одном семействе ресурсов.</span><span class="sxs-lookup"><span data-stu-id="02387-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="02387-133">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="02387-133">OData query parameters</span></span>

<span data-ttu-id="02387-134">Этот метод поддерживает параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="02387-134">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="02387-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="02387-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span>

- <span data-ttu-id="02387-137">Ограниченная поддержка `$filter`:</span><span class="sxs-lookup"><span data-stu-id="02387-137">There is limited support for `$filter`:</span></span>

  - <span data-ttu-id="02387-138">Поддерживаются только `$filter` выражение — для отслеживания изменений для конкретных ресурсы по идентификатору: `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="02387-138">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="02387-139">Число идентификаторы, которые можно задать ограничивается Максимальная длина URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="02387-139">The number of ids you can specify is limited by the maximum URL length.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02387-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02387-140">Request headers</span></span>

| <span data-ttu-id="02387-141">Имя</span><span class="sxs-lookup"><span data-stu-id="02387-141">Name</span></span>       | <span data-ttu-id="02387-142">Описание</span><span class="sxs-lookup"><span data-stu-id="02387-142">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="02387-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="02387-143">Authorization</span></span>  | <span data-ttu-id="02387-144">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="02387-144">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="02387-145">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02387-145">Content-Type</span></span>  | <span data-ttu-id="02387-146">application/json</span><span class="sxs-lookup"><span data-stu-id="02387-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="02387-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02387-147">Request body</span></span>

<span data-ttu-id="02387-148">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02387-148">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="02387-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="02387-149">Response</span></span>

<span data-ttu-id="02387-150">Успешно завершена, этот метод возвращает `200 OK` кода и [directoryRole](../resources/directoryrole.md) коллекции объект ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="02387-150">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="02387-151">Ответ также включает `nextLink` URL-адрес или `deltaLink` URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="02387-151">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="02387-152">Если `nextLink` возвращается URL-адрес, существуют дополнительные страницы данных для получения в сеанс.</span><span class="sxs-lookup"><span data-stu-id="02387-152">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="02387-153">Приложение по-прежнему производится выполняете запросы, используя `nextLink` URL-адрес, пока не `deltaLink` URL-адрес включен в ответе.</span><span class="sxs-lookup"><span data-stu-id="02387-153">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="02387-154">Если `deltaLink` возвращается URL-адрес, нет дополнительных данных о состоянии существующих ресурсов должно быть возвращено.</span><span class="sxs-lookup"><span data-stu-id="02387-154">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="02387-155">Сохранение `deltaLink` URL-адрес и его применения в следующем вызове **дельты** сведения об изменениях в ресурса в будущем.</span><span class="sxs-lookup"><span data-stu-id="02387-155">Save `deltaLink` URL and apply it in the next **delta** call to learn about changes to the resource in the future.</span></span>

### <a name="example"></a><span data-ttu-id="02387-156">Пример</span><span class="sxs-lookup"><span data-stu-id="02387-156">Example</span></span>

##### <a name="request"></a><span data-ttu-id="02387-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="02387-157">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/directoryRoles/delta
```

##### <a name="response"></a><span data-ttu-id="02387-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="02387-158">Response</span></span>

<span data-ttu-id="02387-p110">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02387-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryRoles",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/directoryRoles/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
      {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="02387-161">См. также</span><span class="sxs-lookup"><span data-stu-id="02387-161">See also</span></span>

- <span data-ttu-id="02387-162">[Использование разностного запроса для отслеживания изменений в данных Microsoft Graph](../../../concepts/delta_query_overview.md) для получения дополнительных сведений</span><span class="sxs-lookup"><span data-stu-id="02387-162">[Use delta query to track changes in Microsoft Graph data](../../../concepts/delta_query_overview.md) for more details</span></span>
- <span data-ttu-id="02387-163">[Примеры запросов](../../../concepts/delta_query_users.md)</span><span class="sxs-lookup"><span data-stu-id="02387-163">[Get incremental changes for users](../../../concepts/delta_query_users.md) for an example requests.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->