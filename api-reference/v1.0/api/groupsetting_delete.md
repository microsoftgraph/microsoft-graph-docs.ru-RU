# <a name="delete-a-group-setting"></a><span data-ttu-id="11af2-101">Удаление параметра группы</span><span class="sxs-lookup"><span data-stu-id="11af2-101">Delete a group setting</span></span>

<span data-ttu-id="11af2-102">Удаление параметра группы.</span><span class="sxs-lookup"><span data-stu-id="11af2-102">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="11af2-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11af2-103">Permissions</span></span>

<span data-ttu-id="11af2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="11af2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="11af2-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11af2-106">Permission type</span></span>      | <span data-ttu-id="11af2-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11af2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11af2-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11af2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="11af2-109">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="11af2-109">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="11af2-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11af2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11af2-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11af2-111">Not supported.</span></span>    |
|<span data-ttu-id="11af2-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11af2-112">Application</span></span> | <span data-ttu-id="11af2-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11af2-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11af2-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11af2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="11af2-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11af2-115">Request headers</span></span>

| <span data-ttu-id="11af2-116">Имя</span><span class="sxs-lookup"><span data-stu-id="11af2-116">Name</span></span> | <span data-ttu-id="11af2-117">Описание</span><span class="sxs-lookup"><span data-stu-id="11af2-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="11af2-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11af2-118">Authorization</span></span>  | <span data-ttu-id="11af2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11af2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="11af2-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11af2-121">Content-Type</span></span>  | <span data-ttu-id="11af2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="11af2-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="11af2-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11af2-123">Request body</span></span>
<span data-ttu-id="11af2-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="11af2-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11af2-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="11af2-125">Response</span></span>

<span data-ttu-id="11af2-p103">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="11af2-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11af2-128">Пример</span><span class="sxs-lookup"><span data-stu-id="11af2-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11af2-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="11af2-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="11af2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="11af2-130">Response</span></span>
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
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->