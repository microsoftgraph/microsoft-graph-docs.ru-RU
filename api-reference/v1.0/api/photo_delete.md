# <a name="delete-photo"></a><span data-ttu-id="1d273-101">Удаление фотографии</span><span class="sxs-lookup"><span data-stu-id="1d273-101">Delete photo</span></span>

<span data-ttu-id="1d273-102">Удаление фотографии.</span><span class="sxs-lookup"><span data-stu-id="1d273-102">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d273-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d273-103">Permissions</span></span>
<span data-ttu-id="1d273-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1d273-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1d273-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d273-106">Permission type</span></span>      | <span data-ttu-id="1d273-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d273-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d273-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d273-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1d273-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d273-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1d273-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d273-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d273-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d273-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1d273-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d273-112">Application</span></span> | <span data-ttu-id="1d273-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d273-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d273-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d273-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="1d273-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d273-115">Request headers</span></span>
| <span data-ttu-id="1d273-116">Имя</span><span class="sxs-lookup"><span data-stu-id="1d273-116">Name</span></span>       | <span data-ttu-id="1d273-117">Тип</span><span class="sxs-lookup"><span data-stu-id="1d273-117">Type</span></span> | <span data-ttu-id="1d273-118">Описание</span><span class="sxs-lookup"><span data-stu-id="1d273-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1d273-119">if-match</span><span class="sxs-lookup"><span data-stu-id="1d273-119">if-match</span></span>  | <span data-ttu-id="1d273-120">string</span><span class="sxs-lookup"><span data-stu-id="1d273-120">string</span></span>  | <span data-ttu-id="1d273-121">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="1d273-121">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="1d273-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d273-122">Authorization</span></span>  | <span data-ttu-id="1d273-123">string</span><span class="sxs-lookup"><span data-stu-id="1d273-123">string</span></span>  | <span data-ttu-id="1d273-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d273-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d273-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d273-126">Request body</span></span>
<span data-ttu-id="1d273-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d273-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d273-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d273-128">Response</span></span>

<span data-ttu-id="1d273-p103">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1d273-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d273-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1d273-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d273-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d273-132">Request</span></span>
<span data-ttu-id="1d273-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d273-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="1d273-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d273-134">Response</span></span>
<span data-ttu-id="1d273-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1d273-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
