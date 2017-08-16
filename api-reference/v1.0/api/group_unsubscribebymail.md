# <a name="group-unsubscribebymail"></a><span data-ttu-id="e57a9-101">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="e57a9-101">group: unsubscribeByMail</span></span>

<span data-ttu-id="e57a9-p101">С помощью этого метода можно заблокировать для текущего пользователя получение уведомлений электронной почты о новых записях, событиях и файлов в этой группе. Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="e57a9-p101">Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span> 
## <a name="prerequisites"></a><span data-ttu-id="e57a9-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e57a9-104">Prerequisites</span></span>
<span data-ttu-id="e57a9-105">Для применения этого API требуется одна из указанных **областей**: *Group.ReadWrite.All* 
*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="e57a9-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* 
*Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="e57a9-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e57a9-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="e57a9-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e57a9-107">Request headers</span></span>
| <span data-ttu-id="e57a9-108">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e57a9-108">Header</span></span>       | <span data-ttu-id="e57a9-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e57a9-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e57a9-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e57a9-110">Authorization</span></span>  | <span data-ttu-id="e57a9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e57a9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e57a9-113">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e57a9-113">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e57a9-114">Отклик</span><span class="sxs-lookup"><span data-stu-id="e57a9-114">Response</span></span>

<span data-ttu-id="e57a9-p103">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e57a9-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e57a9-117">Пример</span><span class="sxs-lookup"><span data-stu-id="e57a9-117">Example</span></span>
<span data-ttu-id="e57a9-118">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e57a9-118">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e57a9-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="e57a9-119">Request</span></span>
<span data-ttu-id="e57a9-120">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e57a9-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```

##### <a name="response"></a><span data-ttu-id="e57a9-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="e57a9-121">Response</span></span>
<span data-ttu-id="e57a9-122">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e57a9-122">Here is an example of the response.</span></span> 
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
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
