# <a name="delete-event"></a><span data-ttu-id="b1ce9-101">Удаление события</span><span class="sxs-lookup"><span data-stu-id="b1ce9-101">Delete event</span></span>

<span data-ttu-id="b1ce9-102">Удаление события.</span><span class="sxs-lookup"><span data-stu-id="b1ce9-102">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="b1ce9-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1ce9-103">Permissions</span></span>
<span data-ttu-id="b1ce9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b1ce9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b1ce9-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1ce9-106">Permission type</span></span>      | <span data-ttu-id="b1ce9-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1ce9-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="b1ce9-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1ce9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b1ce9-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1ce9-109">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="b1ce9-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1ce9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1ce9-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1ce9-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="b1ce9-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1ce9-112">Application</span></span> | <span data-ttu-id="b1ce9-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1ce9-113">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b1ce9-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1ce9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}
DELETE /users/{id | userPrincipalName}/events/{id}
DELETE /groups/{id}/events/{id}

DELETE /me/calendar/events/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}
DELETE /groups/{id}/calendar/events/{id}/

DELETE /me/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b1ce9-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1ce9-115">Request headers</span></span>
| <span data-ttu-id="b1ce9-116">Имя</span><span class="sxs-lookup"><span data-stu-id="b1ce9-116">Name</span></span>       | <span data-ttu-id="b1ce9-117">Тип</span><span class="sxs-lookup"><span data-stu-id="b1ce9-117">Type</span></span> | <span data-ttu-id="b1ce9-118">Описание</span><span class="sxs-lookup"><span data-stu-id="b1ce9-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b1ce9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1ce9-119">Authorization</span></span>  | <span data-ttu-id="b1ce9-120">string</span><span class="sxs-lookup"><span data-stu-id="b1ce9-120">string</span></span>  | <span data-ttu-id="b1ce9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1ce9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1ce9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1ce9-123">Request body</span></span>
<span data-ttu-id="b1ce9-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1ce9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1ce9-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1ce9-125">Response</span></span>

<span data-ttu-id="b1ce9-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b1ce9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1ce9-128">Пример</span><span class="sxs-lookup"><span data-stu-id="b1ce9-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1ce9-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1ce9-129">Request</span></span>
<span data-ttu-id="b1ce9-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1ce9-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}
```
##### <a name="response"></a><span data-ttu-id="b1ce9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1ce9-131">Response</span></span>
<span data-ttu-id="b1ce9-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b1ce9-132">Here is an example of the response.</span></span> 
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
