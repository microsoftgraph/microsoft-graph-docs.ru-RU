# <a name="create-mailfolder"></a><span data-ttu-id="e4dfd-101">Создание объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="e4dfd-101">Create MailFolder</span></span>

<span data-ttu-id="e4dfd-102">С помощью этого API можно создать папку почты в корневой папке почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="e4dfd-102">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="e4dfd-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4dfd-103">Permissions</span></span>
<span data-ttu-id="e4dfd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e4dfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e4dfd-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4dfd-106">Permission type</span></span>      | <span data-ttu-id="e4dfd-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4dfd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4dfd-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4dfd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e4dfd-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4dfd-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e4dfd-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4dfd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4dfd-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4dfd-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e4dfd-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4dfd-112">Application</span></span> | <span data-ttu-id="e4dfd-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4dfd-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4dfd-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4dfd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="e4dfd-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4dfd-115">Request headers</span></span>
| <span data-ttu-id="e4dfd-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4dfd-116">Header</span></span>       | <span data-ttu-id="e4dfd-117">Значение</span><span class="sxs-lookup"><span data-stu-id="e4dfd-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e4dfd-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4dfd-118">Authorization</span></span>  | <span data-ttu-id="e4dfd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4dfd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e4dfd-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4dfd-121">Content-Type</span></span>  | <span data-ttu-id="e4dfd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e4dfd-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e4dfd-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4dfd-123">Request body</span></span>
<span data-ttu-id="e4dfd-p103">Предоставьте в тексте запроса объект JSON с указанными ниже параметрами. **displayName** — это единственное доступное для записи свойство объекта [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="e4dfd-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="e4dfd-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="e4dfd-126">Parameter</span></span>    | <span data-ttu-id="e4dfd-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e4dfd-127">Type</span></span>   |<span data-ttu-id="e4dfd-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e4dfd-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4dfd-129">displayName</span><span class="sxs-lookup"><span data-stu-id="e4dfd-129">displayName</span></span>|<span data-ttu-id="e4dfd-130">String</span><span class="sxs-lookup"><span data-stu-id="e4dfd-130">String</span></span>|<span data-ttu-id="e4dfd-131">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="e4dfd-131">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="e4dfd-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4dfd-132">Response</span></span>

<span data-ttu-id="e4dfd-133">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [MailFolder](../resources/mailfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e4dfd-133">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4dfd-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e4dfd-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4dfd-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4dfd-135">Request</span></span>
<span data-ttu-id="e4dfd-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4dfd-136">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="e4dfd-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4dfd-137">Response</span></span>
<span data-ttu-id="e4dfd-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e4dfd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
