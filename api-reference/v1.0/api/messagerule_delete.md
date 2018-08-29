# <a name="delete-messagerule"></a><span data-ttu-id="e1dc4-101">Удаление messageRule</span><span class="sxs-lookup"><span data-stu-id="e1dc4-101">Delete messageRule</span></span>


<span data-ttu-id="e1dc4-102">Удаление указанного объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="e1dc4-102">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1dc4-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1dc4-103">Permissions</span></span>
<span data-ttu-id="e1dc4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e1dc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e1dc4-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1dc4-106">Permission type</span></span>      | <span data-ttu-id="e1dc4-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1dc4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1dc4-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1dc4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e1dc4-109">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1dc4-109">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e1dc4-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1dc4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1dc4-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1dc4-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e1dc4-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1dc4-112">Application</span></span> | <span data-ttu-id="e1dc4-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1dc4-113">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1dc4-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1dc4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e1dc4-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1dc4-115">Request headers</span></span>
| <span data-ttu-id="e1dc4-116">Имя</span><span class="sxs-lookup"><span data-stu-id="e1dc4-116">Name</span></span>       | <span data-ttu-id="e1dc4-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e1dc4-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e1dc4-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1dc4-118">Authorization</span></span>  | <span data-ttu-id="e1dc4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1dc4-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e1dc4-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1dc4-121">Request body</span></span>
<span data-ttu-id="e1dc4-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1dc4-122">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e1dc4-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1dc4-123">Response</span></span>
<span data-ttu-id="e1dc4-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e1dc4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1dc4-126">Пример</span><span class="sxs-lookup"><span data-stu-id="e1dc4-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1dc4-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1dc4-127">Request</span></span>
<span data-ttu-id="e1dc4-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1dc4-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
##### <a name="response"></a><span data-ttu-id="e1dc4-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1dc4-129">Response</span></span>
<span data-ttu-id="e1dc4-130">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e1dc4-130">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->