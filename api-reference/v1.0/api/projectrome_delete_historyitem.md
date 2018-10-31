# <a name="delete-a-historyitem"></a><span data-ttu-id="b00d4-101">Удалить historyItem</span><span class="sxs-lookup"><span data-stu-id="b00d4-101">Delete a historyItem</span></span>

<span data-ttu-id="b00d4-102">Удаление существующего элемента журнала для действия существующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="b00d4-102">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="b00d4-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b00d4-103">Permissions</span></span>

<span data-ttu-id="b00d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b00d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="b00d4-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b00d4-106">Permission type</span></span>      | <span data-ttu-id="b00d4-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b00d4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b00d4-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b00d4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b00d4-109">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="b00d4-109">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="b00d4-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b00d4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b00d4-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="b00d4-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="b00d4-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="b00d4-112">Application</span></span> | <span data-ttu-id="b00d4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b00d4-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b00d4-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b00d4-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b00d4-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b00d4-115">Request headers</span></span>

|<span data-ttu-id="b00d4-116">Имя</span><span class="sxs-lookup"><span data-stu-id="b00d4-116">Name</span></span> | <span data-ttu-id="b00d4-117">Тип</span><span class="sxs-lookup"><span data-stu-id="b00d4-117">Type</span></span> | <span data-ttu-id="b00d4-118">Описание</span><span class="sxs-lookup"><span data-stu-id="b00d4-118">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="b00d4-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b00d4-119">Authorization</span></span> | <span data-ttu-id="b00d4-120">строка</span><span class="sxs-lookup"><span data-stu-id="b00d4-120">string</span></span> | <span data-ttu-id="b00d4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b00d4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b00d4-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b00d4-123">Request body</span></span>

<span data-ttu-id="b00d4-124">Нет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="b00d4-124">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="b00d4-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b00d4-125">Response</span></span>

<span data-ttu-id="b00d4-126">В случае успешного выполнения этот метод возвращает код отклика , если элемент журнала был удален.`204 No Content`</span><span class="sxs-lookup"><span data-stu-id="b00d4-126">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="b00d4-127">Пример</span><span class="sxs-lookup"><span data-stu-id="b00d4-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b00d4-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="b00d4-128">Request</span></span>

<span data-ttu-id="b00d4-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b00d4-129">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
```

##### <a name="response"></a><span data-ttu-id="b00d4-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b00d4-130">Response</span></span>

<span data-ttu-id="b00d4-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b00d4-131">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->