# <a name="get-contactfolder"></a><span data-ttu-id="8e4cb-101">Получение объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="8e4cb-101">Get contactFolder</span></span>

<span data-ttu-id="8e4cb-102">Получение папки контактов с помощью ее идентификатора.</span><span class="sxs-lookup"><span data-stu-id="8e4cb-102">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="8e4cb-103">Существует два сценария, где приложение может получить папке контактов другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e4cb-103">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="8e4cb-104">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="8e4cb-104">If the app has application permissions, or,</span></span>
* <span data-ttu-id="8e4cb-105">Если приложение имеет соответствующей делегированных [разрешений](#permissions) от одного пользователя, и другой пользователь общей папке контактов с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="8e4cb-105">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="8e4cb-106">В разделе [сведения и примеры](../../../concepts/outlook-get-shared-contacts-folders.md).</span><span class="sxs-lookup"><span data-stu-id="8e4cb-106">See [details and an example](../../../concepts/outlook-get-shared-contacts-folders.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="8e4cb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e4cb-107">Permissions</span></span>
<span data-ttu-id="8e4cb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8e4cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8e4cb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e4cb-110">Permission type</span></span>      | <span data-ttu-id="8e4cb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e4cb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e4cb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e4cb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8e4cb-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e4cb-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8e4cb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e4cb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e4cb-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e4cb-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8e4cb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e4cb-116">Application</span></span> | <span data-ttu-id="8e4cb-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e4cb-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e4cb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e4cb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8e4cb-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8e4cb-119">Optional query parameters</span></span>
<span data-ttu-id="8e4cb-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8e4cb-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8e4cb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e4cb-121">Request headers</span></span>
| <span data-ttu-id="8e4cb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8e4cb-122">Name</span></span>       | <span data-ttu-id="8e4cb-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8e4cb-123">Type</span></span> | <span data-ttu-id="8e4cb-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8e4cb-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8e4cb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e4cb-125">Authorization</span></span>  | <span data-ttu-id="8e4cb-126">string</span><span class="sxs-lookup"><span data-stu-id="8e4cb-126">string</span></span>  | <span data-ttu-id="8e4cb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e4cb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e4cb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e4cb-129">Request body</span></span>
<span data-ttu-id="8e4cb-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e4cb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e4cb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e4cb-131">Response</span></span>

<span data-ttu-id="8e4cb-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e4cb-132">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e4cb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8e4cb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e4cb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e4cb-134">Request</span></span>
<span data-ttu-id="8e4cb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e4cb-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="8e4cb-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e4cb-136">Response</span></span>
<span data-ttu-id="8e4cb-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8e4cb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
