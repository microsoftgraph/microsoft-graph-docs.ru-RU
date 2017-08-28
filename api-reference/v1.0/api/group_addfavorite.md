# <a name="group-addfavorite"></a><span data-ttu-id="1c9dd-101">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="1c9dd-101">group: addFavorite</span></span>
<span data-ttu-id="1c9dd-p101">Добавление группы в список избранных групп текущего пользователя. Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="1c9dd-p101">Add the group to the list of the current user's favorite groups. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c9dd-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c9dd-104">Permissions</span></span>
<span data-ttu-id="1c9dd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1c9dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1c9dd-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c9dd-107">Permission type</span></span>      | <span data-ttu-id="1c9dd-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c9dd-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c9dd-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c9dd-109">Delegated (work or school account)</span></span> | <span data-ttu-id="1c9dd-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c9dd-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1c9dd-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c9dd-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c9dd-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c9dd-112">Not supported.</span></span>    |
|<span data-ttu-id="1c9dd-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c9dd-113">Application</span></span> | <span data-ttu-id="1c9dd-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c9dd-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c9dd-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c9dd-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```
## <a name="request-headers"></a><span data-ttu-id="1c9dd-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c9dd-116">Request headers</span></span>
| <span data-ttu-id="1c9dd-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c9dd-117">Header</span></span>       | <span data-ttu-id="1c9dd-118">Значение</span><span class="sxs-lookup"><span data-stu-id="1c9dd-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1c9dd-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c9dd-119">Authorization</span></span>  | <span data-ttu-id="1c9dd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c9dd-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1c9dd-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c9dd-122">Request body</span></span>
<span data-ttu-id="1c9dd-123">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c9dd-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c9dd-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c9dd-124">Response</span></span>

<span data-ttu-id="1c9dd-p104">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1c9dd-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c9dd-127">Пример</span><span class="sxs-lookup"><span data-stu-id="1c9dd-127">Example</span></span>
<span data-ttu-id="1c9dd-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1c9dd-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1c9dd-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c9dd-129">Request</span></span>
<span data-ttu-id="1c9dd-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c9dd-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/addFavorite
```

##### <a name="response"></a><span data-ttu-id="1c9dd-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c9dd-131">Response</span></span>
<span data-ttu-id="1c9dd-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1c9dd-132">Here is an example of the response.</span></span>
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
  "description": "group: addFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->