# <a name="create-mailfolder"></a><span data-ttu-id="f0926-101">Создание объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="f0926-101">Create MailFolder</span></span>

<span data-ttu-id="f0926-102">Используйте этот API, чтобы создать папку почты в корневой папке почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="f0926-102">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0926-103">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f0926-103">Prerequisites</span></span>
<span data-ttu-id="f0926-104">Для применения этого API требуется следующая **область**: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="f0926-104">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="f0926-105">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0926-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="f0926-106">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0926-106">Request headers</span></span>
| <span data-ttu-id="f0926-107">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0926-107">Header</span></span>       | <span data-ttu-id="f0926-108">Значение</span><span class="sxs-lookup"><span data-stu-id="f0926-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f0926-109">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0926-109">Authorization</span></span>  | <span data-ttu-id="f0926-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0926-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f0926-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0926-112">Content-Type</span></span>  | <span data-ttu-id="f0926-113">application/json</span><span class="sxs-lookup"><span data-stu-id="f0926-113">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f0926-114">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0926-114">Request body</span></span>
<span data-ttu-id="f0926-p102">Предоставьте в тексте запроса объект JSON с указанными ниже параметрами. **displayName** — это единственное доступное для записи свойство объекта [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="f0926-p102">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="f0926-117">Параметр</span><span class="sxs-lookup"><span data-stu-id="f0926-117">Parameter</span></span>    | <span data-ttu-id="f0926-118">Тип</span><span class="sxs-lookup"><span data-stu-id="f0926-118">Type</span></span>   |<span data-ttu-id="f0926-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f0926-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0926-120">displayName</span><span class="sxs-lookup"><span data-stu-id="f0926-120">displayName</span></span>|<span data-ttu-id="f0926-121">String</span><span class="sxs-lookup"><span data-stu-id="f0926-121">String</span></span>|<span data-ttu-id="f0926-122">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="f0926-122">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="f0926-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0926-123">Response</span></span>

<span data-ttu-id="f0926-124">В случае успешного выполнения этот метод возвращает код ответа `201, Created` и объект [MailFolder](../resources/mailfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f0926-124">If successful, this method returns `201, Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0926-125">Пример</span><span class="sxs-lookup"><span data-stu-id="f0926-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0926-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0926-126">Request</span></span>
<span data-ttu-id="f0926-127">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0926-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```

##### <a name="response"></a><span data-ttu-id="f0926-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0926-128">Response</span></span>
<span data-ttu-id="f0926-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f0926-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
