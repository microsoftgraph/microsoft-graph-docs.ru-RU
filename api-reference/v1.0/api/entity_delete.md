# <a name="delete-entity"></a><span data-ttu-id="1bfaf-101">Удаление сущности</span><span class="sxs-lookup"><span data-stu-id="1bfaf-101">Delete entity</span></span>

<span data-ttu-id="1bfaf-102">Удаление объекта.</span><span class="sxs-lookup"><span data-stu-id="1bfaf-102">Delete entity.</span></span>
## <a name="permissions"></a><span data-ttu-id="1bfaf-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1bfaf-103">Permissions</span></span>
<span data-ttu-id="1bfaf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1bfaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1bfaf-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bfaf-106">Permission type</span></span>      | <span data-ttu-id="1bfaf-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bfaf-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bfaf-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bfaf-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1bfaf-109">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bfaf-109">Not supported.</span></span>    |
|<span data-ttu-id="1bfaf-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bfaf-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bfaf-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bfaf-111">Not supported.</span></span>    |
|<span data-ttu-id="1bfaf-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1bfaf-112">Application</span></span> | <span data-ttu-id="1bfaf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bfaf-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bfaf-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bfaf-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http


```
## <a name="request-headers"></a><span data-ttu-id="1bfaf-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bfaf-115">Request headers</span></span>
| <span data-ttu-id="1bfaf-116">Имя</span><span class="sxs-lookup"><span data-stu-id="1bfaf-116">Name</span></span>       | <span data-ttu-id="1bfaf-117">Тип</span><span class="sxs-lookup"><span data-stu-id="1bfaf-117">Type</span></span> | <span data-ttu-id="1bfaf-118">Описание</span><span class="sxs-lookup"><span data-stu-id="1bfaf-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1bfaf-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bfaf-119">Authorization</span></span>  | <span data-ttu-id="1bfaf-120">string</span><span class="sxs-lookup"><span data-stu-id="1bfaf-120">string</span></span>  | <span data-ttu-id="1bfaf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bfaf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bfaf-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1bfaf-123">Request body</span></span>
<span data-ttu-id="1bfaf-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1bfaf-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bfaf-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bfaf-125">Response</span></span>

<span data-ttu-id="1bfaf-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1bfaf-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bfaf-128">Пример</span><span class="sxs-lookup"><span data-stu-id="1bfaf-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bfaf-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bfaf-129">Request</span></span>
<span data-ttu-id="1bfaf-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bfaf-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "delete_entity"
}-->
```http

```
##### <a name="response"></a><span data-ttu-id="1bfaf-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bfaf-131">Response</span></span>
<span data-ttu-id="1bfaf-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1bfaf-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete entity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
