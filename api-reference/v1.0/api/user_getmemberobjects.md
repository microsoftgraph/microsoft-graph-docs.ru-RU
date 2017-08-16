# <a name="user-getmemberobjects"></a><span data-ttu-id="6e714-101">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="6e714-101">user: getMemberObjects</span></span>
<span data-ttu-id="6e714-p101">Возвращение всех групп, ролей каталога и административных подразделений, в которых состоит пользователь. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="6e714-p101">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e714-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6e714-104">Prerequisites</span></span>
<span data-ttu-id="6e714-105">Для применения этого API требуется одна из указанных **областей**: *Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="6e714-105">One of the following **scopes** is required to execute this API: *Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="6e714-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e714-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="6e714-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e714-107">Request headers</span></span>
| <span data-ttu-id="6e714-108">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e714-108">Header</span></span>       | <span data-ttu-id="6e714-109">Значение</span><span class="sxs-lookup"><span data-stu-id="6e714-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6e714-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e714-110">Authorization</span></span>  | <span data-ttu-id="6e714-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e714-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6e714-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e714-113">Content-Type</span></span>  | <span data-ttu-id="6e714-114">application/json</span><span class="sxs-lookup"><span data-stu-id="6e714-114">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6e714-115">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6e714-115">Request body</span></span>
<span data-ttu-id="6e714-116">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6e714-116">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6e714-117">Параметр</span><span class="sxs-lookup"><span data-stu-id="6e714-117">Parameter</span></span>    | <span data-ttu-id="6e714-118">Тип</span><span class="sxs-lookup"><span data-stu-id="6e714-118">Type</span></span>   |<span data-ttu-id="6e714-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6e714-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e714-120">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="6e714-120">securityEnabledOnly</span></span>|<span data-ttu-id="6e714-121">Логическое</span><span class="sxs-lookup"><span data-stu-id="6e714-121">Boolean</span></span>|<span data-ttu-id="6e714-p103">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит пользователь. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является пользователь. Примечание. Присвоить значение **true** можно только при вызове этого метода для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e714-p103">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups and directory roles that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="6e714-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e714-124">Response</span></span>

<span data-ttu-id="6e714-125">В случае успеха этот метод возвращает код отклика `200, OK` и коллекцию строк в тексте отклика, содержащую идентификаторы групп и ролей каталога, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="6e714-125">If successful, this method returns `200, OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="6e714-126">Пример</span><span class="sxs-lookup"><span data-stu-id="6e714-126">Example</span></span>
<span data-ttu-id="6e714-127">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6e714-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6e714-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e714-128">Request</span></span>
<span data-ttu-id="6e714-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e714-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="6e714-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e714-130">Response</span></span>
<span data-ttu-id="6e714-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6e714-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
