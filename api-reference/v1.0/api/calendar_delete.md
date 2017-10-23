# <a name="delete-calendar"></a><span data-ttu-id="336b5-101">Удаление календаря</span><span class="sxs-lookup"><span data-stu-id="336b5-101">Delete calendar</span></span>

<span data-ttu-id="336b5-102">Удаление календаря, отличного от календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="336b5-102">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="336b5-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="336b5-103">Permissions</span></span>
<span data-ttu-id="336b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="336b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="336b5-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="336b5-106">Permission type</span></span>      | <span data-ttu-id="336b5-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="336b5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="336b5-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="336b5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="336b5-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="336b5-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="336b5-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="336b5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="336b5-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="336b5-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="336b5-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="336b5-112">Application</span></span> | <span data-ttu-id="336b5-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="336b5-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="336b5-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="336b5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="336b5-115">[Календарь](../resources/calendar.md) пользователя, отличный от календаря по умолчанию, в группе [calendarGroup](../resources/calendargroup.md) по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="336b5-115">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="336b5-116">[Календарь](../resources/calendar.md), отличный от календаря по умолчанию, в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="336b5-116">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="336b5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="336b5-117">Request headers</span></span>
| <span data-ttu-id="336b5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="336b5-118">Name</span></span>           |  <span data-ttu-id="336b5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="336b5-119">Type</span></span>    | <span data-ttu-id="336b5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="336b5-120">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="336b5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="336b5-121">Authorization</span></span>  |  <span data-ttu-id="336b5-122">string</span><span class="sxs-lookup"><span data-stu-id="336b5-122">string</span></span>  | <span data-ttu-id="336b5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="336b5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="336b5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="336b5-125">Request body</span></span>
<span data-ttu-id="336b5-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="336b5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="336b5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="336b5-127">Response</span></span>

<span data-ttu-id="336b5-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="336b5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="336b5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="336b5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="336b5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="336b5-131">Request</span></span>
<span data-ttu-id="336b5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="336b5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="336b5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="336b5-133">Response</span></span>
<span data-ttu-id="336b5-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="336b5-134">Here is an example of the response.</span></span> 
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
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
