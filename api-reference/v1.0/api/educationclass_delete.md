# <a name="delete-educationclass"></a><span data-ttu-id="0994d-101">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="0994d-101">Delete educationClass</span></span>

<span data-ttu-id="0994d-102">Удаление класса.</span><span class="sxs-lookup"><span data-stu-id="0994d-102">Delete a class.</span></span> <span data-ttu-id="0994d-103">Так как класс также является универсальной группой, удаление класса приводит к удалению группы.</span><span class="sxs-lookup"><span data-stu-id="0994d-103">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="0994d-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0994d-104">Permissions</span></span>
<span data-ttu-id="0994d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0994d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0994d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0994d-107">Permission type</span></span>      | <span data-ttu-id="0994d-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0994d-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0994d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0994d-109">Delegated (work or school account)</span></span> |  <span data-ttu-id="0994d-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0994d-110">Not supported.</span></span>  |
|<span data-ttu-id="0994d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0994d-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0994d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0994d-112">Not supported.</span></span>  |
|<span data-ttu-id="0994d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0994d-113">Application</span></span> | <span data-ttu-id="0994d-114">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0994d-114">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0994d-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0994d-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="0994d-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0994d-116">Request headers</span></span>
| <span data-ttu-id="0994d-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0994d-117">Header</span></span>       | <span data-ttu-id="0994d-118">Значение</span><span class="sxs-lookup"><span data-stu-id="0994d-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0994d-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0994d-119">Authorization</span></span>  | <span data-ttu-id="0994d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0994d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0994d-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0994d-122">Request body</span></span>
<span data-ttu-id="0994d-123">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0994d-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0994d-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="0994d-124">Response</span></span>
<span data-ttu-id="0994d-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0994d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0994d-127">Пример</span><span class="sxs-lookup"><span data-stu-id="0994d-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0994d-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="0994d-128">Request</span></span>
<span data-ttu-id="0994d-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0994d-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/11022
```
##### <a name="response"></a><span data-ttu-id="0994d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0994d-130">Response</span></span>
<span data-ttu-id="0994d-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0994d-131">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->