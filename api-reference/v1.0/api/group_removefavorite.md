# <a name="group-removefavorite"></a><span data-ttu-id="f6ac7-101">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="f6ac7-101">group: removeFavorite</span></span>
<span data-ttu-id="f6ac7-p101">Удаление группы из списка избранных групп текущего пользователя. Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="f6ac7-p101">Remove the group from the list of the current user's favorite groups. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6ac7-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6ac7-104">Permissions</span></span>
<span data-ttu-id="f6ac7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f6ac7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f6ac7-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6ac7-107">Permission type</span></span>      | <span data-ttu-id="f6ac7-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6ac7-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6ac7-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6ac7-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f6ac7-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6ac7-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f6ac7-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6ac7-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6ac7-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6ac7-112">Not supported.</span></span>    |
|<span data-ttu-id="f6ac7-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6ac7-113">Application</span></span> | <span data-ttu-id="f6ac7-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6ac7-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6ac7-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6ac7-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```
## <a name="request-headers"></a><span data-ttu-id="f6ac7-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6ac7-116">Request headers</span></span>
| <span data-ttu-id="f6ac7-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6ac7-117">Header</span></span>       | <span data-ttu-id="f6ac7-118">Значение</span><span class="sxs-lookup"><span data-stu-id="f6ac7-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f6ac7-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6ac7-119">Authorization</span></span>  | <span data-ttu-id="f6ac7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6ac7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f6ac7-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6ac7-122">Request body</span></span>
<span data-ttu-id="f6ac7-123">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6ac7-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6ac7-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6ac7-124">Response</span></span>

<span data-ttu-id="f6ac7-p104">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f6ac7-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6ac7-127">Пример</span><span class="sxs-lookup"><span data-stu-id="f6ac7-127">Example</span></span>
<span data-ttu-id="f6ac7-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f6ac7-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f6ac7-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6ac7-129">Request</span></span>
<span data-ttu-id="f6ac7-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6ac7-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/removeFavorite
```

##### <a name="response"></a><span data-ttu-id="f6ac7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6ac7-131">Response</span></span>
<span data-ttu-id="f6ac7-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f6ac7-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
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