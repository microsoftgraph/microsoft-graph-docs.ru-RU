# <a name="list-joinedteams"></a><span data-ttu-id="98565-101">Список joinedTeams</span><span class="sxs-lookup"><span data-stu-id="98565-101">List joinedTeams</span></span>



<span data-ttu-id="98565-102">Загрузите группами Майкрософт, который пользователь является непосредственным членом [групп](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="98565-102">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="98565-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98565-103">Permissions</span></span>
<span data-ttu-id="98565-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="98565-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="98565-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98565-106">Permission type</span></span>      | <span data-ttu-id="98565-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98565-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98565-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98565-108">Delegated (work or school account)</span></span> | <span data-ttu-id="98565-109">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98565-109">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="98565-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98565-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98565-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98565-111">Not supported.</span></span>    |
|<span data-ttu-id="98565-112">Для приложения</span><span class="sxs-lookup"><span data-stu-id="98565-112">Application</span></span> | <span data-ttu-id="98565-113">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98565-113">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="98565-114">С разрешения пользователя делегированной эта операция работает только для «me» пользователя.</span><span class="sxs-lookup"><span data-stu-id="98565-114">With user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="98565-115">Имея разрешения приложения это работает для всех пользователей, указав идентификатор определенного пользователя. («обо мне» псевдоним не поддерживается с разрешениями приложения)</span><span class="sxs-lookup"><span data-stu-id="98565-115">With application permissions, it works for all users by specifying  the specific user id. ('me' alias is not supported with application permissions)</span></span>

## <a name="http-request"></a><span data-ttu-id="98565-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98565-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="98565-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="98565-117">Optional query parameters</span></span>
<span data-ttu-id="98565-118">[Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="98565-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98565-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98565-119">Request headers</span></span>
| <span data-ttu-id="98565-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98565-120">Header</span></span>       | <span data-ttu-id="98565-121">Значение</span><span class="sxs-lookup"><span data-stu-id="98565-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="98565-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98565-122">Authorization</span></span>  | <span data-ttu-id="98565-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98565-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="98565-125">Accept</span><span class="sxs-lookup"><span data-stu-id="98565-125">Accept</span></span>  | <span data-ttu-id="98565-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98565-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98565-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98565-127">Request body</span></span>
<span data-ttu-id="98565-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98565-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98565-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="98565-129">Response</span></span>

<span data-ttu-id="98565-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="98565-130">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="98565-131">Пример</span><span class="sxs-lookup"><span data-stu-id="98565-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98565-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="98565-132">Request</span></span>
<span data-ttu-id="98565-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98565-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/beta/me/joinedTeams
```
##### <a name="response"></a><span data-ttu-id="98565-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="98565-134">Response</span></span>
<span data-ttu-id="98565-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="98565-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
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

## <a name="see-also"></a><span data-ttu-id="98565-138">См. также</span><span class="sxs-lookup"><span data-stu-id="98565-138">See also</span></span>
[<span data-ttu-id="98565-139">Список всех групп</span><span class="sxs-lookup"><span data-stu-id="98565-139">List all teams</span></span>](../../../concepts/teams_list_all_teams.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
