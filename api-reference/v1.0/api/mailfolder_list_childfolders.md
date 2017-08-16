# <a name="list-childfolders"></a><span data-ttu-id="c0e5b-101">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="c0e5b-101">List childFolders</span></span>

<span data-ttu-id="c0e5b-p101">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="c0e5b-p101">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0e5b-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c0e5b-104">Prerequisites</span></span>
<span data-ttu-id="c0e5b-105">Для применения этого API требуется одна из указанных **областей**: *Mail.Read; Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="c0e5b-105">One of the following scopes is required to execute this API: Mail.Read; Mail.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="c0e5b-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0e5b-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c0e5b-107">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c0e5b-107">Optional query parameters</span></span>
<span data-ttu-id="c0e5b-108">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c0e5b-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c0e5b-109">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0e5b-109">Request headers</span></span>
| <span data-ttu-id="c0e5b-110">Имя</span><span class="sxs-lookup"><span data-stu-id="c0e5b-110">Name</span></span>       | <span data-ttu-id="c0e5b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c0e5b-111">Type</span></span> | <span data-ttu-id="c0e5b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c0e5b-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c0e5b-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0e5b-113">Authorization</span></span>  | <span data-ttu-id="c0e5b-114">string</span><span class="sxs-lookup"><span data-stu-id="c0e5b-114">string</span></span>  | <span data-ttu-id="c0e5b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0e5b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0e5b-117">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0e5b-117">Request body</span></span>
<span data-ttu-id="c0e5b-118">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0e5b-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0e5b-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0e5b-119">Response</span></span>

<span data-ttu-id="c0e5b-120">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [MailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0e5b-120">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0e5b-121">Пример</span><span class="sxs-lookup"><span data-stu-id="c0e5b-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0e5b-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0e5b-122">Request</span></span>
<span data-ttu-id="c0e5b-123">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0e5b-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="c0e5b-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0e5b-124">Response</span></span>
<span data-ttu-id="c0e5b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c0e5b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
