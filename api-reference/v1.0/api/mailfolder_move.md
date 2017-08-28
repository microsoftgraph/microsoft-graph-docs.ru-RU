# <a name="mailfolder-move"></a><span data-ttu-id="667db-101">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="667db-101">mailFolder: move</span></span>

<span data-ttu-id="667db-102">Перемещение папки почты со всем ее содержимым в другую папку почты.</span><span class="sxs-lookup"><span data-stu-id="667db-102">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="667db-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="667db-103">Permissions</span></span>
<span data-ttu-id="667db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="667db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="667db-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="667db-106">Permission type</span></span>      | <span data-ttu-id="667db-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="667db-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="667db-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="667db-108">Delegated (work or school account)</span></span> | <span data-ttu-id="667db-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="667db-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="667db-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="667db-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="667db-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="667db-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="667db-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="667db-112">Application</span></span> | <span data-ttu-id="667db-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="667db-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="667db-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="667db-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```
## <a name="request-headers"></a><span data-ttu-id="667db-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="667db-115">Request headers</span></span>
| <span data-ttu-id="667db-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="667db-116">Header</span></span>       | <span data-ttu-id="667db-117">Значение</span><span class="sxs-lookup"><span data-stu-id="667db-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="667db-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="667db-118">Authorization</span></span>  | <span data-ttu-id="667db-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="667db-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="667db-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="667db-121">Content-Type</span></span>  | <span data-ttu-id="667db-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="667db-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="667db-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="667db-124">Request body</span></span>
<span data-ttu-id="667db-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="667db-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="667db-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="667db-126">Parameter</span></span>    | <span data-ttu-id="667db-127">Тип</span><span class="sxs-lookup"><span data-stu-id="667db-127">Type</span></span>   |<span data-ttu-id="667db-128">Описание</span><span class="sxs-lookup"><span data-stu-id="667db-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="667db-129">destinationId</span><span class="sxs-lookup"><span data-stu-id="667db-129">destinationId</span></span>|<span data-ttu-id="667db-130">String</span><span class="sxs-lookup"><span data-stu-id="667db-130">String</span></span>|<span data-ttu-id="667db-131">Идентификатор папки либо имя известной папки *Inbox*, *Drafts*, *SentItems* или *DeletedItems*.</span><span class="sxs-lookup"><span data-stu-id="667db-131">The folder ID, or the *Inbox*, *Drafts*, *SentItems*, or *DeletedItems* well-known folder name.</span></span>|

## <a name="response"></a><span data-ttu-id="667db-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="667db-132">Response</span></span>

<span data-ttu-id="667db-133">В случае успеха этот метод возвращает код отклика `200, OK` и объект [MailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="667db-133">If successful, this method returns `200, OK` response code and [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="667db-134">Пример</span><span class="sxs-lookup"><span data-stu-id="667db-134">Example</span></span>
<span data-ttu-id="667db-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="667db-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="667db-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="667db-136">Request</span></span>
<span data-ttu-id="667db-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="667db-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/move
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="667db-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="667db-138">Response</span></span>
<span data-ttu-id="667db-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="667db-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
