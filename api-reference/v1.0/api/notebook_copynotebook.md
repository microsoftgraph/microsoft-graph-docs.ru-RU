# <a name="notebook-copynotebook"></a><span data-ttu-id="18bb3-101">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="18bb3-101">notebook: copyNotebook</span></span>
<span data-ttu-id="18bb3-p101">Копирование записной книжки в папку Notebooks в целевой библиотеке документов. Если такой папки нет, она будет создана.</span><span class="sxs-lookup"><span data-stu-id="18bb3-p101">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="18bb3-104">Для операций Copy необходимо использовать модель асинхронного вызова.  То есть сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="18bb3-104">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18bb3-105">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="18bb3-105">Prerequisites</span></span>
<span data-ttu-id="18bb3-106">Для выполнения этого API требуется одно из следующих **разрешений**:</span><span class="sxs-lookup"><span data-stu-id="18bb3-106">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="18bb3-107">Notes.Create, Notes.ReadWrite или Notes.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="18bb3-107">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="18bb3-108">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18bb3-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="18bb3-109">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18bb3-109">Request headers</span></span>
| <span data-ttu-id="18bb3-110">Имя</span><span class="sxs-lookup"><span data-stu-id="18bb3-110">Name</span></span>       | <span data-ttu-id="18bb3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="18bb3-111">Type</span></span> | <span data-ttu-id="18bb3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="18bb3-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18bb3-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="18bb3-113">Authorization</span></span>  | <span data-ttu-id="18bb3-114">string</span><span class="sxs-lookup"><span data-stu-id="18bb3-114">string</span></span>  | <span data-ttu-id="18bb3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18bb3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18bb3-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18bb3-117">Content-Type</span></span> | <span data-ttu-id="18bb3-118">строка</span><span class="sxs-lookup"><span data-stu-id="18bb3-118">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="18bb3-119">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18bb3-119">Request body</span></span>
<span data-ttu-id="18bb3-p103">В теле запроса укажите объект JSON, который содержит параметры, требуемые операцией. Если тело не нужно, можно отправить пустое тело.</span><span class="sxs-lookup"><span data-stu-id="18bb3-p103">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="18bb3-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="18bb3-122">Parameter</span></span>    | <span data-ttu-id="18bb3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="18bb3-123">Type</span></span>   |<span data-ttu-id="18bb3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="18bb3-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18bb3-125">groupId</span><span class="sxs-lookup"><span data-stu-id="18bb3-125">groupId</span></span>|<span data-ttu-id="18bb3-126">String</span><span class="sxs-lookup"><span data-stu-id="18bb3-126">String</span></span>|<span data-ttu-id="18bb3-p104">Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="18bb3-p104">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="18bb3-129">renameAs</span><span class="sxs-lookup"><span data-stu-id="18bb3-129">renameAs</span></span>|<span data-ttu-id="18bb3-130">String</span><span class="sxs-lookup"><span data-stu-id="18bb3-130">String</span></span>|<span data-ttu-id="18bb3-p105">Имя копии. По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="18bb3-p105">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="18bb3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="18bb3-133">Response</span></span>

<span data-ttu-id="18bb3-p106">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteOperation_get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="18bb3-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteOperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="18bb3-136">Пример</span><span class="sxs-lookup"><span data-stu-id="18bb3-136">Example</span></span>
<span data-ttu-id="18bb3-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="18bb3-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="18bb3-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="18bb3-138">Request</span></span>
<span data-ttu-id="18bb3-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18bb3-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="18bb3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="18bb3-140">Response</span></span>
<span data-ttu-id="18bb3-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="18bb3-141">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
