# <a name="group-removefavorite"></a><span data-ttu-id="ce06f-101">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="ce06f-101">group: removeFavorite</span></span>
<span data-ttu-id="ce06f-p101">Удаление группы из списка избранных групп текущего пользователя. Поддерживается только для Групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="ce06f-p101">Remove the group from the list of the current user's favorite groups. Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce06f-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce06f-104">Permissions</span></span>
<span data-ttu-id="ce06f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ce06f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ce06f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce06f-107">Permission type</span></span>      | <span data-ttu-id="ce06f-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce06f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce06f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce06f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ce06f-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce06f-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce06f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce06f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce06f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce06f-112">Not supported.</span></span>    |
|<span data-ttu-id="ce06f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce06f-113">Application</span></span> | <span data-ttu-id="ce06f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce06f-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce06f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce06f-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```
## <a name="request-headers"></a><span data-ttu-id="ce06f-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce06f-116">Request headers</span></span>
| <span data-ttu-id="ce06f-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce06f-117">Header</span></span>       | <span data-ttu-id="ce06f-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ce06f-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ce06f-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce06f-119">Authorization</span></span>  | <span data-ttu-id="ce06f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce06f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ce06f-122">Prefer</span><span class="sxs-lookup"><span data-stu-id="ce06f-122">Prefer</span></span> | <span data-ttu-id="ce06f-123">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="ce06f-123">return=minimal.</span></span> <span data-ttu-id="ce06f-124">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ce06f-124">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="ce06f-125">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ce06f-125">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="ce06f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ce06f-126">Request body</span></span>
<span data-ttu-id="ce06f-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce06f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce06f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce06f-128">Response</span></span>
<span data-ttu-id="ce06f-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ce06f-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce06f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ce06f-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ce06f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce06f-132">Request</span></span>
<span data-ttu-id="ce06f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce06f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/removeFavorite
```

#### <a name="response"></a><span data-ttu-id="ce06f-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ce06f-134">Response</span></span>
<span data-ttu-id="ce06f-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ce06f-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->