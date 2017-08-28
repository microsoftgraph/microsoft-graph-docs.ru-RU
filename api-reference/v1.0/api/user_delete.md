# <a name="delete-a-user"></a><span data-ttu-id="4fc7a-101">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="4fc7a-101">Delete a user</span></span>

<span data-ttu-id="4fc7a-102">Удаление пользователя.</span><span class="sxs-lookup"><span data-stu-id="4fc7a-102">Delete user.</span></span>
## <a name="permissions"></a><span data-ttu-id="4fc7a-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4fc7a-103">Permissions</span></span>
<span data-ttu-id="4fc7a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4fc7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4fc7a-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fc7a-106">Permission type</span></span>      | <span data-ttu-id="4fc7a-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fc7a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4fc7a-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fc7a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4fc7a-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4fc7a-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4fc7a-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fc7a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fc7a-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fc7a-111">Not supported.</span></span>    |
|<span data-ttu-id="4fc7a-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fc7a-112">Application</span></span> | <span data-ttu-id="4fc7a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fc7a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fc7a-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fc7a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="4fc7a-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4fc7a-115">Request headers</span></span>
| <span data-ttu-id="4fc7a-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4fc7a-116">Header</span></span>       | <span data-ttu-id="4fc7a-117">Значение</span><span class="sxs-lookup"><span data-stu-id="4fc7a-117">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="4fc7a-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4fc7a-118">Authorization</span></span>  | <span data-ttu-id="4fc7a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fc7a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4fc7a-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4fc7a-121">Request body</span></span>
<span data-ttu-id="4fc7a-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4fc7a-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fc7a-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fc7a-123">Response</span></span>

<span data-ttu-id="4fc7a-p103">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4fc7a-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fc7a-126">Пример</span><span class="sxs-lookup"><span data-stu-id="4fc7a-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4fc7a-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fc7a-127">Request</span></span>
<span data-ttu-id="4fc7a-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fc7a-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/mba9a3254-9f18-4209-aeb3-9e42a35b5be4
```
##### <a name="response"></a><span data-ttu-id="4fc7a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fc7a-129">Response</span></span>
<span data-ttu-id="4fc7a-130">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4fc7a-130">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->