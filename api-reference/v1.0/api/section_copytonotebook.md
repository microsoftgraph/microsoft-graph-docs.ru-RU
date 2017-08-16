# <a name="section-copytonotebook"></a><span data-ttu-id="99218-101">section: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="99218-101">section: copyToNotebook</span></span>
<span data-ttu-id="99218-102">Копирование раздела в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="99218-102">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="99218-103">Для операций Copy необходимо использовать модель асинхронного вызова:  сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="99218-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="99218-104">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="99218-104">Prerequisites</span></span>
<span data-ttu-id="99218-105">Для выполнения этого API требуется одно из следующих **разрешений**:</span><span class="sxs-lookup"><span data-stu-id="99218-105">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="99218-106">Notes.Create, Notes.ReadWrite или Notes.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="99218-106">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="99218-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99218-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="99218-108">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99218-108">Request headers</span></span>
| <span data-ttu-id="99218-109">Имя</span><span class="sxs-lookup"><span data-stu-id="99218-109">Name</span></span>       | <span data-ttu-id="99218-110">Тип</span><span class="sxs-lookup"><span data-stu-id="99218-110">Type</span></span> | <span data-ttu-id="99218-111">Описание</span><span class="sxs-lookup"><span data-stu-id="99218-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="99218-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="99218-112">Authorization</span></span>  | <span data-ttu-id="99218-113">string</span><span class="sxs-lookup"><span data-stu-id="99218-113">string</span></span>  | <span data-ttu-id="99218-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99218-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="99218-116">Content-Type</span><span class="sxs-lookup"><span data-stu-id="99218-116">Content-Type</span></span> | <span data-ttu-id="99218-117">строка</span><span class="sxs-lookup"><span data-stu-id="99218-117">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="99218-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99218-118">Request body</span></span>
<span data-ttu-id="99218-119">В тексте запроса укажите объект JSON, который содержит параметры, требуемые операцией.</span><span class="sxs-lookup"><span data-stu-id="99218-119">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="99218-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="99218-120">Parameter</span></span>    | <span data-ttu-id="99218-121">Тип</span><span class="sxs-lookup"><span data-stu-id="99218-121">Type</span></span>   |<span data-ttu-id="99218-122">Описание</span><span class="sxs-lookup"><span data-stu-id="99218-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99218-123">groupId</span><span class="sxs-lookup"><span data-stu-id="99218-123">groupId</span></span>|<span data-ttu-id="99218-124">String</span><span class="sxs-lookup"><span data-stu-id="99218-124">String</span></span>|<span data-ttu-id="99218-p102">Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="99218-p102">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="99218-127">id</span><span class="sxs-lookup"><span data-stu-id="99218-127">id</span></span>|<span data-ttu-id="99218-128">Строка</span><span class="sxs-lookup"><span data-stu-id="99218-128">String</span></span>|<span data-ttu-id="99218-p103">Обязательный. Идентификатор целевой записной книжки.</span><span class="sxs-lookup"><span data-stu-id="99218-p103">Required. The id of the destination notebook.</span></span> |
|<span data-ttu-id="99218-131">renameAs</span><span class="sxs-lookup"><span data-stu-id="99218-131">renameAs</span></span>|<span data-ttu-id="99218-132">String</span><span class="sxs-lookup"><span data-stu-id="99218-132">String</span></span>|<span data-ttu-id="99218-p104">Имя копии. По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="99218-p104">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="99218-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="99218-135">Response</span></span>

<span data-ttu-id="99218-p105">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation_get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="99218-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="99218-138">Пример</span><span class="sxs-lookup"><span data-stu-id="99218-138">Example</span></span>
<span data-ttu-id="99218-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="99218-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="99218-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="99218-140">Request</span></span>
<span data-ttu-id="99218-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99218-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="99218-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="99218-142">Response</span></span>
<span data-ttu-id="99218-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="99218-143">Here is an example of the response.</span></span>
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
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->