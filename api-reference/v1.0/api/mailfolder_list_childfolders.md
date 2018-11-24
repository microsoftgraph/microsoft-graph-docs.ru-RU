# <a name="list-childfolders"></a><span data-ttu-id="eb174-101">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="eb174-101">List childFolders</span></span>

<span data-ttu-id="eb174-p101">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="eb174-p101">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="eb174-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb174-104">Permissions</span></span>
<span data-ttu-id="eb174-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eb174-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eb174-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb174-107">Permission type</span></span>      | <span data-ttu-id="eb174-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb174-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb174-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb174-109">Delegated (work or school account)</span></span> | <span data-ttu-id="eb174-110">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb174-110">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eb174-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb174-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb174-112">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb174-112">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eb174-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb174-113">Application</span></span> | <span data-ttu-id="eb174-114">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb174-114">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb174-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb174-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eb174-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eb174-116">Optional query parameters</span></span>
<span data-ttu-id="eb174-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eb174-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="eb174-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb174-118">Request headers</span></span>
| <span data-ttu-id="eb174-119">Имя</span><span class="sxs-lookup"><span data-stu-id="eb174-119">Name</span></span>       | <span data-ttu-id="eb174-120">Тип</span><span class="sxs-lookup"><span data-stu-id="eb174-120">Type</span></span> | <span data-ttu-id="eb174-121">Описание</span><span class="sxs-lookup"><span data-stu-id="eb174-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="eb174-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb174-122">Authorization</span></span>  | <span data-ttu-id="eb174-123">string</span><span class="sxs-lookup"><span data-stu-id="eb174-123">string</span></span>  | <span data-ttu-id="eb174-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb174-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb174-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb174-126">Request body</span></span>
<span data-ttu-id="eb174-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb174-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb174-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb174-128">Response</span></span>

<span data-ttu-id="eb174-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [MailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eb174-129">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eb174-130">Пример</span><span class="sxs-lookup"><span data-stu-id="eb174-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb174-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb174-131">Request</span></span>
<span data-ttu-id="eb174-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb174-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="eb174-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb174-133">Response</span></span>
<span data-ttu-id="eb174-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="eb174-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
