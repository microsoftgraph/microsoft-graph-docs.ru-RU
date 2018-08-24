# <a name="delete-message"></a><span data-ttu-id="4ab90-101">Удалить сообщение</span><span class="sxs-lookup"><span data-stu-id="4ab90-101">Delete message</span></span>

<span data-ttu-id="4ab90-102">Удалите сообщение в почтовом ящике указанного пользователя либо связь сообщения.</span><span class="sxs-lookup"><span data-stu-id="4ab90-102">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="4ab90-103">**Примечание:** Возможно, вы не сможете удалить элементы в папке удаления восстанавливаемых элементов (представленной [хорошо известным названием папки](../resources/mailfolder.md) `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="4ab90-103">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="4ab90-104">Подробнее см. статьи [Хранение удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) и [Очистка удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items).</span><span class="sxs-lookup"><span data-stu-id="4ab90-104">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ab90-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ab90-105">Permissions</span></span>
<span data-ttu-id="4ab90-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4ab90-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4ab90-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ab90-108">Permission type</span></span>      | <span data-ttu-id="4ab90-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ab90-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ab90-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ab90-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4ab90-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ab90-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4ab90-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ab90-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ab90-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ab90-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4ab90-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ab90-114">Application</span></span> | <span data-ttu-id="4ab90-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ab90-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ab90-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ab90-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4ab90-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ab90-117">Request headers</span></span>
| <span data-ttu-id="4ab90-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4ab90-118">Name</span></span>       | <span data-ttu-id="4ab90-119">Тип</span><span class="sxs-lookup"><span data-stu-id="4ab90-119">Type</span></span> | <span data-ttu-id="4ab90-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4ab90-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4ab90-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ab90-121">Authorization</span></span>  | <span data-ttu-id="4ab90-122">строка</span><span class="sxs-lookup"><span data-stu-id="4ab90-122">string</span></span>  | <span data-ttu-id="4ab90-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ab90-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ab90-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ab90-125">Request body</span></span>
<span data-ttu-id="4ab90-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ab90-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ab90-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ab90-127">Response</span></span>

<span data-ttu-id="4ab90-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4ab90-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ab90-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4ab90-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ab90-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ab90-131">Request</span></span>
<span data-ttu-id="4ab90-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ab90-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="4ab90-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ab90-133">Response</span></span>
<span data-ttu-id="4ab90-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4ab90-134">Here is an example of the response.</span></span> 
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
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->