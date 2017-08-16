# <a name="group-resetunseencount"></a><span data-ttu-id="027c4-101">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="027c4-101">group: resetUnseenCount</span></span>

<span data-ttu-id="027c4-p101">Сброс свойства unseenCount всех записей, которые пользователь не просматривал со своего предыдущего посещения. Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="027c4-p101">Reset the unseenCount of all the posts that the current user has not seen since their last visit. Supported for only Office 365 groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="027c4-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="027c4-104">Prerequisites</span></span>
<span data-ttu-id="027c4-105">Для применения этого API требуется одна из указанных **областей**: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="027c4-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span> 
## <a name="http-request"></a><span data-ttu-id="027c4-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="027c4-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="027c4-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="027c4-107">Request headers</span></span>
| <span data-ttu-id="027c4-108">Заголовок</span><span class="sxs-lookup"><span data-stu-id="027c4-108">Header</span></span>       | <span data-ttu-id="027c4-109">Значение</span><span class="sxs-lookup"><span data-stu-id="027c4-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="027c4-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="027c4-110">Authorization</span></span>  | <span data-ttu-id="027c4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="027c4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="027c4-113">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="027c4-113">Request body</span></span>
<span data-ttu-id="027c4-114">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="027c4-114">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="027c4-115">Отклик</span><span class="sxs-lookup"><span data-stu-id="027c4-115">Response</span></span>

<span data-ttu-id="027c4-p103">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="027c4-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="027c4-118">Пример</span><span class="sxs-lookup"><span data-stu-id="027c4-118">Example</span></span>
<span data-ttu-id="027c4-119">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="027c4-119">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="027c4-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="027c4-120">Request</span></span>
<span data-ttu-id="027c4-121">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="027c4-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```

##### <a name="response"></a><span data-ttu-id="027c4-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="027c4-122">Response</span></span>
<span data-ttu-id="027c4-123">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="027c4-123">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
