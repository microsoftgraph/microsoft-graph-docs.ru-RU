# <a name="remove-member"></a><span data-ttu-id="b555d-101">Удаление элемента</span><span class="sxs-lookup"><span data-stu-id="b555d-101">Remove member</span></span>

<span data-ttu-id="b555d-p101">С помощью этого API можно удалить участника из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации **members**. Вы можете удалять пользователей или другие группы.</span><span class="sxs-lookup"><span data-stu-id="b555d-p101">Use this API to remove a member from an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b555d-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b555d-104">Prerequisites</span></span>
<span data-ttu-id="b555d-105">Для применения этого API требуется одна из указанных **областей**: *Group.ReadWrite.All*, *Directory.ReadWrite.All* или *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="b555d-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="b555d-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b555d-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b555d-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b555d-107">Request headers</span></span>
| <span data-ttu-id="b555d-108">Имя</span><span class="sxs-lookup"><span data-stu-id="b555d-108">Name</span></span>       | <span data-ttu-id="b555d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b555d-109">Type</span></span> | <span data-ttu-id="b555d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b555d-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b555d-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="b555d-111">Authorization</span></span>  | <span data-ttu-id="b555d-112">string</span><span class="sxs-lookup"><span data-stu-id="b555d-112">string</span></span>  | <span data-ttu-id="b555d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b555d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b555d-115">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b555d-115">Request body</span></span>
<span data-ttu-id="b555d-116">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b555d-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b555d-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="b555d-117">Response</span></span>

<span data-ttu-id="b555d-p103">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b555d-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b555d-120">Пример</span><span class="sxs-lookup"><span data-stu-id="b555d-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b555d-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="b555d-121">Request</span></span>
<span data-ttu-id="b555d-122">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b555d-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="b555d-123">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="b555d-123">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

##### <a name="response"></a><span data-ttu-id="b555d-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="b555d-124">Response</span></span>
<span data-ttu-id="b555d-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b555d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->