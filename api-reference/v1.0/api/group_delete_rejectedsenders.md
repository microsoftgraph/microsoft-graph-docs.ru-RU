# <a name="remove-rejectedsender"></a><span data-ttu-id="97125-101">Удаление объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="97125-101">Remove rejectedSender</span></span>

<span data-ttu-id="97125-102">Удаление пользователя или группы из списка rejectedSenders.</span><span class="sxs-lookup"><span data-stu-id="97125-102">Remove a user or group from the rejectedSenders list.</span></span>
## <a name="permissions"></a><span data-ttu-id="97125-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97125-103">Permissions</span></span>
<span data-ttu-id="97125-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="97125-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="97125-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97125-106">Permission type</span></span>      | <span data-ttu-id="97125-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97125-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97125-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97125-108">Delegated (work or school account)</span></span> | <span data-ttu-id="97125-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97125-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="97125-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97125-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97125-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97125-111">Not supported.</span></span>    |
|<span data-ttu-id="97125-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97125-112">Application</span></span> | <span data-ttu-id="97125-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97125-113">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97125-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97125-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id=<id>

```
## <a name="request-headers"></a><span data-ttu-id="97125-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97125-115">Request headers</span></span>
| <span data-ttu-id="97125-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97125-116">Header</span></span>       | <span data-ttu-id="97125-117">Значение</span><span class="sxs-lookup"><span data-stu-id="97125-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="97125-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97125-118">Authorization</span></span>  | <span data-ttu-id="97125-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97125-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97125-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97125-121">Request body</span></span>
<span data-ttu-id="97125-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97125-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97125-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="97125-123">Response</span></span>

<span data-ttu-id="97125-p103">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="97125-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97125-126">Пример</span><span class="sxs-lookup"><span data-stu-id="97125-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97125-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="97125-127">Request</span></span>
<span data-ttu-id="97125-128">Ниже представлено несколько примеров запроса.</span><span class="sxs-lookup"><span data-stu-id="97125-128">Here are a couple of examples of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id="users/{id}"

DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id="groups/{id}"
```

##### <a name="response"></a><span data-ttu-id="97125-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="97125-129">Response</span></span>
<span data-ttu-id="97125-130">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="97125-130">Here is an example of the response.</span></span> 
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
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->