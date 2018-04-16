# <a name="delete-messagerule"></a><span data-ttu-id="5181f-101">Удаление messageRule</span><span class="sxs-lookup"><span data-stu-id="5181f-101">Delete messageRule</span></span>


<span data-ttu-id="5181f-102">Удаление указанного объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="5181f-102">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5181f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5181f-103">Permissions</span></span>
<span data-ttu-id="5181f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5181f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5181f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5181f-106">Permission type</span></span>      | <span data-ttu-id="5181f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5181f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5181f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5181f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5181f-109">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5181f-109">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="5181f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5181f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5181f-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5181f-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="5181f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5181f-112">Application</span></span> | <span data-ttu-id="5181f-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5181f-113">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5181f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5181f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messagerules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5181f-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5181f-115">Request headers</span></span>
| <span data-ttu-id="5181f-116">Имя</span><span class="sxs-lookup"><span data-stu-id="5181f-116">Name</span></span>       | <span data-ttu-id="5181f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="5181f-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5181f-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5181f-118">Authorization</span></span>  | <span data-ttu-id="5181f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5181f-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5181f-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5181f-121">Request body</span></span>
<span data-ttu-id="5181f-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5181f-122">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5181f-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="5181f-123">Response</span></span>
<span data-ttu-id="5181f-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5181f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5181f-126">Пример</span><span class="sxs-lookup"><span data-stu-id="5181f-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5181f-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="5181f-127">Request</span></span>
<span data-ttu-id="5181f-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5181f-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')

```
##### <a name="response"></a><span data-ttu-id="5181f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5181f-129">Response</span></span>
<span data-ttu-id="5181f-130">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5181f-130">Here is an example of the response.</span></span> 
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