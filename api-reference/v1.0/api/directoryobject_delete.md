# <a name="delete-directoryobject"></a><span data-ttu-id="e32d3-101">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="e32d3-101">Delete directoryObject</span></span>

<span data-ttu-id="e32d3-102">Удаляет объект directoryObject.</span><span class="sxs-lookup"><span data-stu-id="e32d3-102">Deletes a directoryObject.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e32d3-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="e32d3-103">Prerequisites</span></span>
<span data-ttu-id="e32d3-104">Для применения этого API требуются указанные ниже **области**. _Directory.AccessAsUser.All_</span><span class="sxs-lookup"><span data-stu-id="e32d3-104">The following **scopes** is required to execute this API: _Directory.AccessAsUser.All_</span></span>

<span data-ttu-id="e32d3-p101">**ПРИМЕЧАНИЕ.** Пользователи, группы и контакты являются типами объекта каталога. По этой причине, если вам нужно удалить пользователей, можно и нужно использовать следующую **область**: _User.ReadWrite.All_</span><span class="sxs-lookup"><span data-stu-id="e32d3-p101">**NOTE:** Users, groups, and contacts are types of directory object. As a result,if you need to delete users, the following **scope** can and should be used: _User.ReadWrite.All_</span></span>
## <a name="http-request"></a><span data-ttu-id="e32d3-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e32d3-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e32d3-108">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e32d3-108">Request headers</span></span>
| <span data-ttu-id="e32d3-109">Имя</span><span class="sxs-lookup"><span data-stu-id="e32d3-109">Name</span></span>       | <span data-ttu-id="e32d3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e32d3-110">Type</span></span> | <span data-ttu-id="e32d3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e32d3-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e32d3-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="e32d3-112">Authorization</span></span>  | <span data-ttu-id="e32d3-113">string</span><span class="sxs-lookup"><span data-stu-id="e32d3-113">string</span></span>  | <span data-ttu-id="e32d3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e32d3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e32d3-116">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e32d3-116">Request body</span></span>
<span data-ttu-id="e32d3-117">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e32d3-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e32d3-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="e32d3-118">Response</span></span>

<span data-ttu-id="e32d3-p103">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e32d3-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e32d3-121">Пример</span><span class="sxs-lookup"><span data-stu-id="e32d3-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e32d3-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="e32d3-122">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="e32d3-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="e32d3-123">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->