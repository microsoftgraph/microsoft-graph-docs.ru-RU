# <a name="notebook-copynotebook"></a><span data-ttu-id="9545b-101">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="9545b-101">notebook: copyNotebook</span></span>
<span data-ttu-id="9545b-p101">Копирование записной книжки в папку Notebooks в целевой библиотеке документов. Если такой папки нет, она будет создана.</span><span class="sxs-lookup"><span data-stu-id="9545b-p101">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="9545b-104">Для операций Copy необходимо использовать модель асинхронного вызова:  сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="9545b-104">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="9545b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9545b-105">Permissions</span></span>
<span data-ttu-id="9545b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9545b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9545b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9545b-108">Permission type</span></span>      | <span data-ttu-id="9545b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9545b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9545b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9545b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9545b-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9545b-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="9545b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9545b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9545b-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9545b-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="9545b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9545b-114">Application</span></span> | <span data-ttu-id="9545b-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9545b-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9545b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9545b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="9545b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9545b-117">Request headers</span></span>
| <span data-ttu-id="9545b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9545b-118">Name</span></span>       | <span data-ttu-id="9545b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9545b-119">Type</span></span> | <span data-ttu-id="9545b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9545b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9545b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9545b-121">Authorization</span></span>  | <span data-ttu-id="9545b-122">string</span><span class="sxs-lookup"><span data-stu-id="9545b-122">string</span></span>  | <span data-ttu-id="9545b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9545b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9545b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9545b-125">Content-Type</span></span> | <span data-ttu-id="9545b-126">строка</span><span class="sxs-lookup"><span data-stu-id="9545b-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="9545b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9545b-127">Request body</span></span>
<span data-ttu-id="9545b-p104">В теле запроса укажите объект JSON, который содержит параметры, требуемые операцией. Если тело не нужно, можно отправить пустое тело.</span><span class="sxs-lookup"><span data-stu-id="9545b-p104">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="9545b-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="9545b-130">Parameter</span></span>    | <span data-ttu-id="9545b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9545b-131">Type</span></span>   |<span data-ttu-id="9545b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9545b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9545b-133">groupId</span><span class="sxs-lookup"><span data-stu-id="9545b-133">groupId</span></span>|<span data-ttu-id="9545b-134">String</span><span class="sxs-lookup"><span data-stu-id="9545b-134">String</span></span>|<span data-ttu-id="9545b-p105">Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="9545b-p105">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="9545b-137">renameAs</span><span class="sxs-lookup"><span data-stu-id="9545b-137">renameAs</span></span>|<span data-ttu-id="9545b-138">String</span><span class="sxs-lookup"><span data-stu-id="9545b-138">String</span></span>|<span data-ttu-id="9545b-p106">Имя копии. По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="9545b-p106">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="9545b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9545b-141">Response</span></span>

<span data-ttu-id="9545b-p107">В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteOperation_get.md), опросите конечную точку Operation-Location.</span><span class="sxs-lookup"><span data-stu-id="9545b-p107">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteOperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="9545b-144">Пример</span><span class="sxs-lookup"><span data-stu-id="9545b-144">Example</span></span>
<span data-ttu-id="9545b-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9545b-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9545b-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="9545b-146">Request</span></span>
<span data-ttu-id="9545b-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9545b-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9545b-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="9545b-148">Response</span></span>
<span data-ttu-id="9545b-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9545b-149">Here is an example of the response.</span></span>
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
