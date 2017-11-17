# <a name="create-mailfolder"></a><span data-ttu-id="76263-101">Создание объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="76263-101">Create MailFolder</span></span>

<span data-ttu-id="76263-102">С помощью этого API можно создать дочернюю папку почты.</span><span class="sxs-lookup"><span data-stu-id="76263-102">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="76263-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76263-103">Permissions</span></span>
<span data-ttu-id="76263-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="76263-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="76263-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76263-106">Permission type</span></span>      | <span data-ttu-id="76263-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76263-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76263-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76263-108">Delegated (work or school account)</span></span> | <span data-ttu-id="76263-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76263-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="76263-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76263-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76263-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76263-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="76263-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76263-112">Application</span></span> | <span data-ttu-id="76263-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76263-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="76263-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76263-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="76263-115">Укажите родительскую папку в URL-адресе запроса как идентификатор папки либо имя известной папки `Inbox`, `Drafts`, `SentItems` или `DeletedItems`.</span><span class="sxs-lookup"><span data-stu-id="76263-115">Specify the parent folder in the query URL as a folder ID, or the `Inbox`, `Drafts`, `SentItems`, or `DeletedItems` well-known folder name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="76263-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76263-116">Request headers</span></span>
| <span data-ttu-id="76263-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="76263-117">Header</span></span>       | <span data-ttu-id="76263-118">Значение</span><span class="sxs-lookup"><span data-stu-id="76263-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="76263-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76263-119">Authorization</span></span>  | <span data-ttu-id="76263-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76263-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="76263-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76263-122">Content-Type</span></span>  | <span data-ttu-id="76263-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76263-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="76263-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76263-125">Request body</span></span>
<span data-ttu-id="76263-p104">Предоставьте в тексте запроса объект JSON с указанными ниже параметрами. **displayName** — это единственное доступное для записи свойство объекта [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="76263-p104">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="76263-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="76263-128">Parameter</span></span>    | <span data-ttu-id="76263-129">Тип</span><span class="sxs-lookup"><span data-stu-id="76263-129">Type</span></span>   |<span data-ttu-id="76263-130">Описание</span><span class="sxs-lookup"><span data-stu-id="76263-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76263-131">displayName</span><span class="sxs-lookup"><span data-stu-id="76263-131">displayName</span></span>|<span data-ttu-id="76263-132">String</span><span class="sxs-lookup"><span data-stu-id="76263-132">String</span></span>|<span data-ttu-id="76263-133">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="76263-133">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="76263-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="76263-134">Response</span></span>

<span data-ttu-id="76263-135">В случае успеха этот метод возвращает код отклика `201 Created` и объект [MailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="76263-135">If successful, this method returns `201 Created` response code and [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76263-136">Пример</span><span class="sxs-lookup"><span data-stu-id="76263-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76263-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="76263-137">Request</span></span>
<span data-ttu-id="76263-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76263-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

##### <a name="response"></a><span data-ttu-id="76263-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="76263-139">Response</span></span>
<span data-ttu-id="76263-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="76263-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
