# <a name="list-attachments"></a><span data-ttu-id="5e858-101">Список вложений</span><span class="sxs-lookup"><span data-stu-id="5e858-101">List attachments</span></span>

<span data-ttu-id="5e858-102">Получение списка объектов [attachment](../resources/attachment.md), вложенных в данные о событии.</span><span class="sxs-lookup"><span data-stu-id="5e858-102">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>
## <a name="permissions"></a><span data-ttu-id="5e858-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e858-103">Permissions</span></span>
<span data-ttu-id="5e858-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5e858-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5e858-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e858-106">Permission type</span></span>      | <span data-ttu-id="5e858-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e858-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e858-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e858-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5e858-109">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5e858-109">Calendars.Read</span></span>    |
|<span data-ttu-id="5e858-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e858-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e858-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5e858-111">Calendars.Read</span></span>    |
|<span data-ttu-id="5e858-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e858-112">Application</span></span> | <span data-ttu-id="5e858-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5e858-113">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e858-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e858-114">HTTP request</span></span>
<span data-ttu-id="5e858-115">Вложения в событие ([event](../resources/event.md)) в пользовательском календаре ([calendar](../resources/calendar.md)), установленном по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5e858-115">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->

<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/attachments
GET /users/{id | userPrincipalName}/events/{id}/attachments

GET /me/calendar/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendar/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
GET /groups/{id}/calendar/events/{id}/attachments
-->

<span data-ttu-id="5e858-116">Вложения в событие ([event](../resources/event.md)) в календаре ([calendar](../resources/calendar.md)), который принадлежит установленной по умолчанию группе календарей ([calendarGroup](../resources/calendargroup.md)) пользователя.</span><span class="sxs-lookup"><span data-stu-id="5e858-116">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

GET /me/calendargroup/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="5e858-117">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="5e858-117">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5e858-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5e858-118">Optional query parameters</span></span>
<span data-ttu-id="5e858-119">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5e858-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5e858-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e858-120">Request headers</span></span>
| <span data-ttu-id="5e858-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5e858-121">Name</span></span>       | <span data-ttu-id="5e858-122">Тип</span><span class="sxs-lookup"><span data-stu-id="5e858-122">Type</span></span> | <span data-ttu-id="5e858-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5e858-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5e858-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e858-124">Authorization</span></span>  | <span data-ttu-id="5e858-125">строка</span><span class="sxs-lookup"><span data-stu-id="5e858-125">string</span></span>  | <span data-ttu-id="5e858-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e858-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e858-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e858-128">Request body</span></span>
<span data-ttu-id="5e858-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5e858-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e858-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e858-130">Response</span></span>

<span data-ttu-id="5e858-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e858-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5e858-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5e858-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e858-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e858-133">Request</span></span>
<span data-ttu-id="5e858-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e858-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="5e858-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e858-135">Response</span></span>
<span data-ttu-id="5e858-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e858-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->