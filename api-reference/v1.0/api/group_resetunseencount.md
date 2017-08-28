# <a name="group-resetunseencount"></a><span data-ttu-id="9ea75-101">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="9ea75-101">group: resetUnseenCount</span></span>

<span data-ttu-id="9ea75-p101">Сброс свойства unseenCount всех записей, которые пользователь не просматривал со своего предыдущего посещения. Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="9ea75-p101">Reset the unseenCount of all the posts that the current user has not seen since their last visit. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ea75-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ea75-104">Permissions</span></span>
<span data-ttu-id="9ea75-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ea75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9ea75-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ea75-107">Permission type</span></span>      | <span data-ttu-id="9ea75-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ea75-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ea75-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ea75-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9ea75-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ea75-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9ea75-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ea75-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ea75-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ea75-112">Not supported.</span></span>    |
|<span data-ttu-id="9ea75-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ea75-113">Application</span></span> | <span data-ttu-id="9ea75-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ea75-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ea75-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ea75-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="9ea75-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ea75-116">Request headers</span></span>
| <span data-ttu-id="9ea75-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ea75-117">Header</span></span>       | <span data-ttu-id="9ea75-118">Значение</span><span class="sxs-lookup"><span data-stu-id="9ea75-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ea75-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ea75-119">Authorization</span></span>  | <span data-ttu-id="9ea75-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ea75-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9ea75-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ea75-122">Request body</span></span>
<span data-ttu-id="9ea75-123">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ea75-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ea75-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ea75-124">Response</span></span>

<span data-ttu-id="9ea75-p104">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9ea75-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ea75-127">Пример</span><span class="sxs-lookup"><span data-stu-id="9ea75-127">Example</span></span>
<span data-ttu-id="9ea75-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9ea75-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9ea75-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ea75-129">Request</span></span>
<span data-ttu-id="9ea75-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ea75-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```

##### <a name="response"></a><span data-ttu-id="9ea75-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ea75-131">Response</span></span>
<span data-ttu-id="9ea75-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9ea75-132">Here is an example of the response.</span></span> 
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
