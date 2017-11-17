# <a name="delete-attachment"></a><span data-ttu-id="192ae-101">Удаление вложения</span><span class="sxs-lookup"><span data-stu-id="192ae-101">Delete attachment</span></span>

<span data-ttu-id="192ae-102">Удаление вложения из данных календаря о событии, сообщения почты или записи группы.</span><span class="sxs-lookup"><span data-stu-id="192ae-102">Delete an attachment from a calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="192ae-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="192ae-103">Permissions</span></span>
<span data-ttu-id="192ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="192ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

* <span data-ttu-id="192ae-106">При доступе к вложениям в сообщениях: Mail.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="192ae-106">If accessing attachments in Messages: Mail.ReadWrite.</span></span>
* <span data-ttu-id="192ae-107">При доступе к вложениям в данных о событиях: Calendars.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="192ae-107">If accessing attachments in Events: Calendars.ReadWrite.</span></span>
* <span data-ttu-id="192ae-108">При доступе к вложениям в записях или данных о событиях групп: Group.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="192ae-108">If accessing attachments in Group Events or Posts: Group.ReadWrite.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="192ae-109">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="192ae-109">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="192ae-110">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md) по умолчанию для пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="192ae-110">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
DELETE /groups/{id}/events/{id}/attachments/{id}

DELETE /me/calendar/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
```
<span data-ttu-id="192ae-111">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="192ae-111">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="192ae-112">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="192ae-112">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="192ae-113">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="192ae-113">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="192ae-114">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="192ae-114">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="192ae-p102">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д.</span><span class="sxs-lookup"><span data-stu-id="192ae-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="192ae-117">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="192ae-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="192ae-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="192ae-118">Request headers</span></span>
| <span data-ttu-id="192ae-119">Имя</span><span class="sxs-lookup"><span data-stu-id="192ae-119">Name</span></span>       | <span data-ttu-id="192ae-120">Тип</span><span class="sxs-lookup"><span data-stu-id="192ae-120">Type</span></span> | <span data-ttu-id="192ae-121">Описание</span><span class="sxs-lookup"><span data-stu-id="192ae-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="192ae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="192ae-122">Authorization</span></span>  | <span data-ttu-id="192ae-123">string</span><span class="sxs-lookup"><span data-stu-id="192ae-123">string</span></span>  | <span data-ttu-id="192ae-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="192ae-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="192ae-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="192ae-126">Request body</span></span>
<span data-ttu-id="192ae-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="192ae-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="192ae-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="192ae-128">Response</span></span>

<span data-ttu-id="192ae-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="192ae-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="192ae-131">Пример</span><span class="sxs-lookup"><span data-stu-id="192ae-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="192ae-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="192ae-132">Request</span></span>
<span data-ttu-id="192ae-133">Ниже приведен пример запроса на удаление вложения из данных, касающихся события.</span><span class="sxs-lookup"><span data-stu-id="192ae-133">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="192ae-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="192ae-134">Response</span></span>
<span data-ttu-id="192ae-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="192ae-135">Here is an example of the response.</span></span>
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
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
