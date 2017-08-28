# <a name="get-contactfolder"></a><span data-ttu-id="9c47d-101">Получение объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="9c47d-101">Get contactFolder</span></span>

<span data-ttu-id="9c47d-102">Получение папки с контактами с использованием идентификатора.</span><span class="sxs-lookup"><span data-stu-id="9c47d-102">Get a contact folder by using the contact folder ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="9c47d-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c47d-103">Permissions</span></span>
<span data-ttu-id="9c47d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9c47d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9c47d-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c47d-106">Permission type</span></span>      | <span data-ttu-id="9c47d-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c47d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c47d-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c47d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9c47d-109">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c47d-109">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9c47d-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c47d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c47d-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c47d-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9c47d-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c47d-112">Application</span></span> | <span data-ttu-id="9c47d-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c47d-113">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c47d-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c47d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9c47d-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9c47d-115">Optional query parameters</span></span>
<span data-ttu-id="9c47d-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9c47d-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9c47d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c47d-117">Request headers</span></span>
| <span data-ttu-id="9c47d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9c47d-118">Name</span></span>       | <span data-ttu-id="9c47d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9c47d-119">Type</span></span> | <span data-ttu-id="9c47d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9c47d-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9c47d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c47d-121">Authorization</span></span>  | <span data-ttu-id="9c47d-122">string</span><span class="sxs-lookup"><span data-stu-id="9c47d-122">string</span></span>  | <span data-ttu-id="9c47d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c47d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c47d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c47d-125">Request body</span></span>
<span data-ttu-id="9c47d-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c47d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c47d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c47d-127">Response</span></span>

<span data-ttu-id="9c47d-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9c47d-128">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9c47d-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9c47d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c47d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c47d-130">Request</span></span>
<span data-ttu-id="9c47d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c47d-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="9c47d-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c47d-132">Response</span></span>
<span data-ttu-id="9c47d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9c47d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
