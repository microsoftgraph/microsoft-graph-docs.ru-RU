# <a name="update-page"></a><span data-ttu-id="d8278-101">Обновление страницы</span><span class="sxs-lookup"><span data-stu-id="d8278-101">Update page</span></span>

<span data-ttu-id="d8278-102">Обновление содержимого страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="d8278-102">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="d8278-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8278-103">Permissions</span></span>
<span data-ttu-id="d8278-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d8278-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d8278-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8278-106">Permission type</span></span>      | <span data-ttu-id="d8278-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8278-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="d8278-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8278-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d8278-109">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8278-109">Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="d8278-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8278-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8278-111">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8278-111">Notes.ReadWrite</span></span>    | 
|<span data-ttu-id="d8278-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8278-112">Application</span></span> | <span data-ttu-id="d8278-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8278-113">Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d8278-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8278-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="d8278-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8278-115">Request headers</span></span>
| <span data-ttu-id="d8278-116">Имя</span><span class="sxs-lookup"><span data-stu-id="d8278-116">Name</span></span>       | <span data-ttu-id="d8278-117">Тип</span><span class="sxs-lookup"><span data-stu-id="d8278-117">Type</span></span> | <span data-ttu-id="d8278-118">Описание</span><span class="sxs-lookup"><span data-stu-id="d8278-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d8278-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8278-119">Authorization</span></span>  | <span data-ttu-id="d8278-120">string</span><span class="sxs-lookup"><span data-stu-id="d8278-120">string</span></span>  | <span data-ttu-id="d8278-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8278-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d8278-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8278-123">Content-Type</span></span> | <span data-ttu-id="d8278-124">строка</span><span class="sxs-lookup"><span data-stu-id="d8278-124">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d8278-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8278-125">Request body</span></span>
<span data-ttu-id="d8278-p103">В теле запроса укажите массив объектов [patchContentCommand](../resources/patchcontentcommand.md), представляющих изменения, вносимые в страницу. Дополнительные сведения и примеры см. в статье <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Обновление страниц OneNote</a>.</span><span class="sxs-lookup"><span data-stu-id="d8278-p103">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page. For more information and examples, see <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="d8278-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8278-128">Response</span></span>

<span data-ttu-id="d8278-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`.  Для запроса PATCH не возвращается никаких данных JSON.</span><span class="sxs-lookup"><span data-stu-id="d8278-p104">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="d8278-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d8278-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8278-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8278-132">Request</span></span>
<span data-ttu-id="d8278-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8278-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
##### <a name="response"></a><span data-ttu-id="d8278-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8278-134">Response</span></span>
<span data-ttu-id="d8278-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d8278-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
