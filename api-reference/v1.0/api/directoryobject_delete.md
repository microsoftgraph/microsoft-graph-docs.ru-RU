# <a name="delete-directoryobject"></a><span data-ttu-id="4b0e1-101">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="4b0e1-101">Delete directoryObject</span></span>

<span data-ttu-id="4b0e1-102">Удаляет directoryObject.</span><span class="sxs-lookup"><span data-stu-id="4b0e1-102">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b0e1-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b0e1-103">Permissions</span></span>
<span data-ttu-id="4b0e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4b0e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="4b0e1-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b0e1-106">Permission type</span></span>      | <span data-ttu-id="4b0e1-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b0e1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b0e1-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b0e1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4b0e1-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4b0e1-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4b0e1-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b0e1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b0e1-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b0e1-111">Not supported.</span></span>    |
|<span data-ttu-id="4b0e1-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b0e1-112">Application</span></span> | <span data-ttu-id="4b0e1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b0e1-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b0e1-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b0e1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="4b0e1-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b0e1-115">Request headers</span></span>
| <span data-ttu-id="4b0e1-116">Имя</span><span class="sxs-lookup"><span data-stu-id="4b0e1-116">Name</span></span>       | <span data-ttu-id="4b0e1-117">Тип</span><span class="sxs-lookup"><span data-stu-id="4b0e1-117">Type</span></span> | <span data-ttu-id="4b0e1-118">Описание</span><span class="sxs-lookup"><span data-stu-id="4b0e1-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4b0e1-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b0e1-119">Authorization</span></span>  | <span data-ttu-id="4b0e1-120">строка</span><span class="sxs-lookup"><span data-stu-id="4b0e1-120">string</span></span>  | <span data-ttu-id="4b0e1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b0e1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b0e1-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b0e1-123">Request body</span></span>
<span data-ttu-id="4b0e1-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4b0e1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b0e1-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b0e1-125">Response</span></span>

<span data-ttu-id="4b0e1-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4b0e1-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b0e1-128">Пример</span><span class="sxs-lookup"><span data-stu-id="4b0e1-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b0e1-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b0e1-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="4b0e1-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b0e1-130">Response</span></span>

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
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->