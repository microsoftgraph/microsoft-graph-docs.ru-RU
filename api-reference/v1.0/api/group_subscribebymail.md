# <a name="group-subscribebymail"></a><span data-ttu-id="cc8d3-101">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="cc8d3-101">group: subscribeByMail</span></span>

<span data-ttu-id="cc8d3-p101">С помощью этого метода можно разрешить текущему пользователю получать уведомления электронной почты о новых записях, событиях и файлов в этой группе. Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="cc8d3-p101">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc8d3-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cc8d3-104">Prerequisites</span></span>
<span data-ttu-id="cc8d3-105">Для применения этого API требуется одна из указанных **областей**: *Group.ReadWrite.All* 
*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="cc8d3-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* 
*Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="cc8d3-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc8d3-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="cc8d3-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc8d3-107">Request headers</span></span>
| <span data-ttu-id="cc8d3-108">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc8d3-108">Header</span></span>       | <span data-ttu-id="cc8d3-109">Значение</span><span class="sxs-lookup"><span data-stu-id="cc8d3-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc8d3-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc8d3-110">Authorization</span></span>  | <span data-ttu-id="cc8d3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc8d3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc8d3-113">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc8d3-113">Request body</span></span>

## <a name="response"></a><span data-ttu-id="cc8d3-114">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc8d3-114">Response</span></span>

<span data-ttu-id="cc8d3-p103">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cc8d3-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc8d3-117">Пример</span><span class="sxs-lookup"><span data-stu-id="cc8d3-117">Example</span></span>
<span data-ttu-id="cc8d3-118">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cc8d3-118">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cc8d3-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc8d3-119">Request</span></span>
<span data-ttu-id="cc8d3-120">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc8d3-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```

##### <a name="response"></a><span data-ttu-id="cc8d3-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc8d3-121">Response</span></span>
<span data-ttu-id="cc8d3-122">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cc8d3-122">Here is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->