# <a name="get-mailfolder"></a><span data-ttu-id="553f5-101">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="553f5-101">Get mailFolder</span></span>

<span data-ttu-id="553f5-102">Получение свойств и связей объекта папки сообщений.</span><span class="sxs-lookup"><span data-stu-id="553f5-102">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="553f5-103">Существует два сценария, где приложение может получить почтовой папки другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="553f5-103">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="553f5-104">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="553f5-104">If the app has application permissions, or,</span></span>
* <span data-ttu-id="553f5-105">Если приложение имеет соответствующий делегированных [разрешений](#permissions) от одного пользователя и другой пользователь доступ к папке почты с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="553f5-105">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="553f5-106">В разделе [сведения и примеры](../../../concepts/outlook-share-messages-folders.md).</span><span class="sxs-lookup"><span data-stu-id="553f5-106">See [details and an example](../../../concepts/outlook-share-messages-folders.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="553f5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="553f5-107">Permissions</span></span>
<span data-ttu-id="553f5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="553f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="553f5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="553f5-110">Permission type</span></span>      | <span data-ttu-id="553f5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="553f5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="553f5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="553f5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="553f5-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="553f5-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="553f5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="553f5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="553f5-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="553f5-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="553f5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="553f5-116">Application</span></span> | <span data-ttu-id="553f5-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="553f5-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="553f5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="553f5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="553f5-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="553f5-119">Optional query parameters</span></span>
<span data-ttu-id="553f5-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="553f5-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="553f5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="553f5-121">Request headers</span></span>
| <span data-ttu-id="553f5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="553f5-122">Name</span></span>       | <span data-ttu-id="553f5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="553f5-123">Type</span></span> | <span data-ttu-id="553f5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="553f5-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="553f5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="553f5-125">Authorization</span></span>  | <span data-ttu-id="553f5-126">string</span><span class="sxs-lookup"><span data-stu-id="553f5-126">string</span></span>  | <span data-ttu-id="553f5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="553f5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="553f5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="553f5-129">Request body</span></span>
<span data-ttu-id="553f5-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="553f5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="553f5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="553f5-131">Response</span></span>

<span data-ttu-id="553f5-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="553f5-132">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="553f5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="553f5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="553f5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="553f5-134">Request</span></span>
<span data-ttu-id="553f5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="553f5-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="553f5-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="553f5-136">Response</span></span>
<span data-ttu-id="553f5-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="553f5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
