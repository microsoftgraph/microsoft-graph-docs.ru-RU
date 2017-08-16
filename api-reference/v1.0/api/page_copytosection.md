# <a name="page-copytosection"></a><span data-ttu-id="7caa6-101">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="7caa6-101">page: copyToSection</span></span>
<span data-ttu-id="7caa6-102">Копирование страницы в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="7caa6-102">Copies a page to a specific section.</span></span>

<span data-ttu-id="7caa6-103">Для операций Copy необходимо использовать модель асинхронного вызова.  То есть сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="7caa6-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7caa6-104">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="7caa6-104">Prerequisites</span></span>
<span data-ttu-id="7caa6-105">Для выполнения этого API требуется одно из следующих **разрешений**:</span><span class="sxs-lookup"><span data-stu-id="7caa6-105">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="7caa6-106">Notes.Create, Notes.ReadWrite или Notes.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="7caa6-106">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>  

## <a name="http-request"></a><span data-ttu-id="7caa6-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7caa6-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="7caa6-108">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7caa6-108">Request headers</span></span>
| <span data-ttu-id="7caa6-109">Имя</span><span class="sxs-lookup"><span data-stu-id="7caa6-109">Name</span></span>       | <span data-ttu-id="7caa6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7caa6-110">Type</span></span> | <span data-ttu-id="7caa6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7caa6-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7caa6-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="7caa6-112">Authorization</span></span>  | <span data-ttu-id="7caa6-113">string</span><span class="sxs-lookup"><span data-stu-id="7caa6-113">string</span></span>  | <span data-ttu-id="7caa6-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7caa6-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7caa6-116">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7caa6-116">Content-Type</span></span> | <span data-ttu-id="7caa6-117">строка</span><span class="sxs-lookup"><span data-stu-id="7caa6-117">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="7caa6-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7caa6-118">Request body</span></span>
<span data-ttu-id="7caa6-119">В тексте запроса укажите объект JSON, который содержит параметры, требуемые операцией.</span><span class="sxs-lookup"><span data-stu-id="7caa6-119">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="7caa6-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="7caa6-120">Parameter</span></span>    | <span data-ttu-id="7caa6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="7caa6-121">Type</span></span>   |<span data-ttu-id="7caa6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7caa6-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7caa6-123">groupId</span><span class="sxs-lookup"><span data-stu-id="7caa6-123">groupId</span></span>|<span data-ttu-id="7caa6-124">String</span><span class="sxs-lookup"><span data-stu-id="7caa6-124">String</span></span>|<span data-ttu-id="7caa6-p102">Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="7caa6-p102">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="7caa6-127">id</span><span class="sxs-lookup"><span data-stu-id="7caa6-127">id</span></span>|<span data-ttu-id="7caa6-128">String</span><span class="sxs-lookup"><span data-stu-id="7caa6-128">String</span></span>|<span data-ttu-id="7caa6-p103">Обязательный. Идентификатор целевого раздела.</span><span class="sxs-lookup"><span data-stu-id="7caa6-p103">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="7caa6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7caa6-131">Response</span></span>

<span data-ttu-id="7caa6-p104">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation_get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="7caa6-p104">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="7caa6-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7caa6-134">Example</span></span>
<span data-ttu-id="7caa6-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7caa6-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7caa6-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="7caa6-136">Request</span></span>
<span data-ttu-id="7caa6-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7caa6-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <a name="response"></a><span data-ttu-id="7caa6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7caa6-138">Response</span></span>
<span data-ttu-id="7caa6-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7caa6-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->