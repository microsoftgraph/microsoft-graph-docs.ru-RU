# <a name="get-calendar"></a><span data-ttu-id="c3270-101">Получение календаря</span><span class="sxs-lookup"><span data-stu-id="c3270-101">Get calendar</span></span>

<span data-ttu-id="c3270-102">Получение свойств и связей объекта [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="c3270-102">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="c3270-103">Это может быть календарь для ресурса [user](../resources/user.md) или стандартный календарь для ресурса [group](../resources/group.md), представляющего группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="c3270-103">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>


### <a name="get-another-users-calendar"></a><span data-ttu-id="c3270-104">Получение календаря другого пользователя</span><span class="sxs-lookup"><span data-stu-id="c3270-104">Get another user's calendar</span></span>

<span data-ttu-id="c3270-105">Если у вас есть разрешения приложения или соответствующие делегированные [разрешения](#permissions) от одного пользователя, вы можете получить календарь другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c3270-105">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get a calendar of another user's.</span></span> <span data-ttu-id="c3270-106">В этом разделе основное внимание уделено сценариям, в которых используются делегированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="c3270-106">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="c3270-107">Например, ваше приложение получило делегированные разрешения от пользователя с именем Никита.</span><span class="sxs-lookup"><span data-stu-id="c3270-107">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="c3270-108">Предположим, что другой пользователь (Garth) поделился своим календарем с Никитой.</span><span class="sxs-lookup"><span data-stu-id="c3270-108">Suppose another user, Garth, has shared a calendar with John.</span></span> <span data-ttu-id="c3270-109">Вы можете получить этот общий календарь, указав идентификатор пользователя (или имя участника-пользователя) Garth в показанном ниже примере запроса.</span><span class="sxs-lookup"><span data-stu-id="c3270-109">You can get that shared calendar by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="c3270-110">Эта возможность применяется для всех поддерживаемых операций GET над календарем для отдельного пользователя, как показано в разделе [HTTP-запрос](#http-request) ниже.</span><span class="sxs-lookup"><span data-stu-id="c3270-110">This capability applies to all the supported GET calendar operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="c3270-111">Она также применяется, если пользователь Garth делегировал разрешения на доступ ко всему своему почтовому ящику пользователю с именем Никита.</span><span class="sxs-lookup"><span data-stu-id="c3270-111">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="c3270-112">Если пользователь Garth не поделился своим календарем с Никитой и не делегировал свой почтовый ящик этому пользователю, указав идентификатор пользователя или имя участника-пользователя Garth в операциях GET, будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="c3270-112">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="c3270-113">В таких случаях, указав идентификатор пользователя или имя участника-пользователя, можно только получить календарь пользователя, выполнившего вход в систему, а запрос будет эквивалентен использованию ярлыка /me:</span><span class="sxs-lookup"><span data-stu-id="c3270-113">In such cases, specifying a user ID or user principal name only works for getting a calendar of the signed-in user’s, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar
```

<span data-ttu-id="c3270-114">Эта возможность доступна только в операциях GET для следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="c3270-114">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="c3270-115">общие папки контактов, календари и папки сообщений;</span><span class="sxs-lookup"><span data-stu-id="c3270-115">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="c3270-116">контакты, события и сообщения в общих папках;</span><span class="sxs-lookup"><span data-stu-id="c3270-116">Contacts and events in shared folders</span></span>
- <span data-ttu-id="c3270-117">указанные выше ресурсы в тех почтовых ящиках, разрешения на доступ к которым делегированы.</span><span class="sxs-lookup"><span data-stu-id="c3270-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="c3270-118">Эта возможность недоступна для других операций над контактами, событиями, сообщениями и их папками.</span><span class="sxs-lookup"><span data-stu-id="c3270-118">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="c3270-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3270-119">Permissions</span></span>
<span data-ttu-id="c3270-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c3270-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c3270-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3270-122">Permission type</span></span>      | <span data-ttu-id="c3270-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3270-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3270-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3270-124">Delegated (work or school account)</span></span> | <span data-ttu-id="c3270-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c3270-125">Calendars.Read</span></span>    |
|<span data-ttu-id="c3270-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3270-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3270-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c3270-127">Calendars.Read</span></span>    |
|<span data-ttu-id="c3270-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3270-128">Application</span></span> | <span data-ttu-id="c3270-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c3270-129">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3270-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3270-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c3270-131">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c3270-131">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="c3270-132">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="c3270-132">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="c3270-133">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="c3270-133">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c3270-134">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c3270-134">Optional query parameters</span></span>
<span data-ttu-id="c3270-135">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c3270-135">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c3270-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3270-136">Request headers</span></span>
| <span data-ttu-id="c3270-137">Имя</span><span class="sxs-lookup"><span data-stu-id="c3270-137">Name</span></span>       | <span data-ttu-id="c3270-138">Тип</span><span class="sxs-lookup"><span data-stu-id="c3270-138">Type</span></span> | <span data-ttu-id="c3270-139">Описание</span><span class="sxs-lookup"><span data-stu-id="c3270-139">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c3270-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3270-140">Authorization</span></span>  | <span data-ttu-id="c3270-141">string</span><span class="sxs-lookup"><span data-stu-id="c3270-141">string</span></span>  | <span data-ttu-id="c3270-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3270-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3270-144">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3270-144">Request body</span></span>
<span data-ttu-id="c3270-145">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3270-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3270-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3270-146">Response</span></span>

<span data-ttu-id="c3270-147">В случае успеха этот метод возвращает код отклика `200 OK` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3270-147">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3270-148">Пример</span><span class="sxs-lookup"><span data-stu-id="c3270-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3270-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3270-149">Request</span></span>
<span data-ttu-id="c3270-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3270-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="c3270-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3270-151">Response</span></span>
<span data-ttu-id="c3270-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c3270-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
    "id": "AAMkAGI2TGuLAAA=",
    "name": "Calendar",
    "color": "auto",
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
    "canShare":true,
    "canViewPrivateItems":true,
    "canEdit":true,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
