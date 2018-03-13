# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="934eb-101">Удаление groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="934eb-101">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="934eb-102">Удаление объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="934eb-102">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="934eb-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="934eb-103">Permissions</span></span>

<span data-ttu-id="934eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="934eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="934eb-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="934eb-106">Permission type</span></span>      | <span data-ttu-id="934eb-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="934eb-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="934eb-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="934eb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="934eb-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="934eb-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="934eb-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="934eb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="934eb-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="934eb-111">Not supported.</span></span>    |
|<span data-ttu-id="934eb-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="934eb-112">Application</span></span> | <span data-ttu-id="934eb-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="934eb-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="934eb-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="934eb-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="934eb-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="934eb-115">Request headers</span></span>

| <span data-ttu-id="934eb-116">Имя</span><span class="sxs-lookup"><span data-stu-id="934eb-116">Name</span></span> | <span data-ttu-id="934eb-117">Описание</span><span class="sxs-lookup"><span data-stu-id="934eb-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="934eb-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="934eb-118">Authorization</span></span> | <span data-ttu-id="934eb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="934eb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="934eb-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="934eb-121">Content-Type</span></span>  | <span data-ttu-id="934eb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="934eb-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="934eb-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="934eb-123">Request body</span></span>
<span data-ttu-id="934eb-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="934eb-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="934eb-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="934eb-125">Response</span></span>

<span data-ttu-id="934eb-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="934eb-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="934eb-128">Пример</span><span class="sxs-lookup"><span data-stu-id="934eb-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="934eb-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="934eb-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="934eb-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="934eb-130">Response</span></span>

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
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->