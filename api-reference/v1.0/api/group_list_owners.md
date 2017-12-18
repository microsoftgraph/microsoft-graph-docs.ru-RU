# <a name="list-owners"></a><span data-ttu-id="71272-101">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="71272-101">List owners</span></span>
<span data-ttu-id="71272-p101">Получение списка владельцев группы. Владельцы — это пользователи, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="71272-p101">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="71272-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71272-104">Permissions</span></span>
<span data-ttu-id="71272-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="71272-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71272-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71272-107">Permission type</span></span>      | <span data-ttu-id="71272-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71272-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71272-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71272-109">Delegated (work or school account)</span></span> | <span data-ttu-id="71272-110">Group.Read.All и User.ReadBasic.All, Group.Read.All и User.Read.All, Group.Read.All и User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71272-110">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="71272-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71272-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71272-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71272-112">Not supported.</span></span>    |
|<span data-ttu-id="71272-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71272-113">Application</span></span> | <span data-ttu-id="71272-114">Group.Read.All и User.Read.All, Group.Read.All и User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71272-114">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71272-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71272-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71272-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71272-116">Optional query parameters</span></span>
<span data-ttu-id="71272-117">Этот метод поддерживает [параметры запросов OData](../../../concepts/query_parameters.md) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="71272-117">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71272-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71272-118">Request headers</span></span>
| <span data-ttu-id="71272-119">Имя</span><span class="sxs-lookup"><span data-stu-id="71272-119">Name</span></span>       | <span data-ttu-id="71272-120">Тип</span><span class="sxs-lookup"><span data-stu-id="71272-120">Type</span></span> | <span data-ttu-id="71272-121">Описание</span><span class="sxs-lookup"><span data-stu-id="71272-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="71272-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71272-122">Authorization</span></span>  | <span data-ttu-id="71272-123">string</span><span class="sxs-lookup"><span data-stu-id="71272-123">string</span></span>  | <span data-ttu-id="71272-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71272-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71272-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71272-126">Request body</span></span>
<span data-ttu-id="71272-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71272-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71272-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="71272-128">Response</span></span>
<span data-ttu-id="71272-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71272-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71272-130">Пример</span><span class="sxs-lookup"><span data-stu-id="71272-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="71272-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="71272-131">Request</span></span>
<span data-ttu-id="71272-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71272-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="71272-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="71272-133">Response</span></span>
<span data-ttu-id="71272-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="71272-134">The following is an example of the response.</span></span>
><span data-ttu-id="71272-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="71272-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="71272-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71272-136">All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.user"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
