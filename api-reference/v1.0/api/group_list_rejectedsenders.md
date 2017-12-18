# <a name="list-rejectedsenders"></a><span data-ttu-id="fca6c-101">Список rejectedSenders</span><span class="sxs-lookup"><span data-stu-id="fca6c-101">List rejectedSenders</span></span>
<span data-ttu-id="fca6c-102">Получение пользователей или групп из списка rejectedSenders для данной группы.</span><span class="sxs-lookup"><span data-stu-id="fca6c-102">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="fca6c-p101">Пользователи из списка запрещенных отправителей не могут отправлять записи в беседы группы (определенные в URL-адресе запроса GET). Убедитесь, что в списках запрещенных и разрешенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="fca6c-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="fca6c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fca6c-105">Permissions</span></span>
<span data-ttu-id="fca6c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fca6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fca6c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fca6c-108">Permission type</span></span>      | <span data-ttu-id="fca6c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fca6c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fca6c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fca6c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fca6c-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fca6c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fca6c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fca6c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fca6c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fca6c-113">Not supported.</span></span>    |
|<span data-ttu-id="fca6c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fca6c-114">Application</span></span> | <span data-ttu-id="fca6c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fca6c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fca6c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fca6c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fca6c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fca6c-117">Optional query parameters</span></span>
<span data-ttu-id="fca6c-118">Этот метод поддерживает [параметры запросов OData](../../../concepts/query_parameters.md) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fca6c-118">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fca6c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fca6c-119">Request headers</span></span>
| <span data-ttu-id="fca6c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fca6c-120">Header</span></span>       | <span data-ttu-id="fca6c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fca6c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fca6c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fca6c-122">Authorization</span></span>  | <span data-ttu-id="fca6c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fca6c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fca6c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fca6c-125">Request body</span></span>
<span data-ttu-id="fca6c-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fca6c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fca6c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="fca6c-127">Response</span></span>
<span data-ttu-id="fca6c-128">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fca6c-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fca6c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fca6c-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fca6c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fca6c-130">Request</span></span>
<span data-ttu-id="fca6c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fca6c-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```

#### <a name="response"></a><span data-ttu-id="fca6c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="fca6c-132">Response</span></span>
<span data-ttu-id="fca6c-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fca6c-133">The following is an example of the response.</span></span>
><span data-ttu-id="fca6c-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fca6c-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fca6c-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fca6c-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->