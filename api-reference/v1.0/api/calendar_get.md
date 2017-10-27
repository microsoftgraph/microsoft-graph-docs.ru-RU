# <a name="get-calendar"></a><span data-ttu-id="bdd79-101">Получение календаря</span><span class="sxs-lookup"><span data-stu-id="bdd79-101">Get calendar</span></span>

<span data-ttu-id="bdd79-102">Получение свойств и связей объекта [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="bdd79-102">Retrieve the properties and relationships of a calendar group object.</span></span> <span data-ttu-id="bdd79-103">Это может быть календарь для ресурса [user](../resources/user.md) или стандартный календарь для ресурса [group](../resources/group.md), представляющего группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="bdd79-103">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>


### <a name="get-another-users-calendar"></a><span data-ttu-id="bdd79-104">Получение календаря другого пользователя</span><span class="sxs-lookup"><span data-stu-id="bdd79-104">Get another user's drive</span></span>

<span data-ttu-id="bdd79-105">Если у вас есть разрешения приложения или соответствующие делегированные [разрешения](#permissions) от одного пользователя, вы можете получить календарь другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="bdd79-105">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get a calendar of another user's.</span></span> <span data-ttu-id="bdd79-106">В этом разделе основное внимание уделено сценариям, в которых используются делегированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="bdd79-106">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="bdd79-107">Например, ваше приложение получило делегированные разрешения от пользователя John.</span><span class="sxs-lookup"><span data-stu-id="bdd79-107">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="bdd79-108">Предположим, что другой пользователь (Garth) поделился своим календарем с пользователем John.</span><span class="sxs-lookup"><span data-stu-id="bdd79-108">Suppose another user, Garth, has shared a calendar with John.</span></span> <span data-ttu-id="bdd79-109">Вы можете получить этот общий календарь, указав идентификатор пользователя (или имя участника-пользователя) Garth в показанном ниже примере запроса.</span><span class="sxs-lookup"><span data-stu-id="bdd79-109">You can get that shared calendar by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="bdd79-110">Эта возможность применяется для всех поддерживаемых операций GET над календарем для отдельного пользователя, как показано в разделе [HTTP-запрос](#http-request) ниже.</span><span class="sxs-lookup"><span data-stu-id="bdd79-110">This capability applies to all the supported GET calendar operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="bdd79-111">Она также применяется, если пользователь Garth делегировал весь свой почтовый ящик пользователю John.</span><span class="sxs-lookup"><span data-stu-id="bdd79-111">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="bdd79-112">Если пользователь Garth не поделился своим календарем с пользователем John и не делегировал свой почтовый ящик этому пользователю, указав идентификатор пользователя или имя участника-пользователя Garth в операциях GET, будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="bdd79-112">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="bdd79-113">В таких случаях, указав идентификатор пользователя или имя участника-пользователя, можно только получить календарь пользователя, выполнившего вход в систему, а запрос будет эквивалентен использованию ярлыка /me:</span><span class="sxs-lookup"><span data-stu-id="bdd79-113">In such cases, specifying a user ID or user principal name only works for getting a calendar of the signed-in user’s, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar
```

<span data-ttu-id="bdd79-114">Эта возможность доступна только в операциях GET для:</span><span class="sxs-lookup"><span data-stu-id="bdd79-114">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="bdd79-115">общих папок контактов;</span><span class="sxs-lookup"><span data-stu-id="bdd79-115">Shared contact folders</span></span>
- <span data-ttu-id="bdd79-116">общих календарей;</span><span class="sxs-lookup"><span data-stu-id="bdd79-116">Shared calendars</span></span>
- <span data-ttu-id="bdd79-117">контактов и событий в общих папках;</span><span class="sxs-lookup"><span data-stu-id="bdd79-117">Contacts and events in shared folders</span></span>
- <span data-ttu-id="bdd79-118">указанных выше ресурсов в делегированных почтовых ящиках.</span><span class="sxs-lookup"><span data-stu-id="bdd79-118">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="bdd79-119">Эта возможность недоступна в других операциях для контактов, событий и их папок.</span><span class="sxs-lookup"><span data-stu-id="bdd79-119">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="bdd79-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bdd79-120">Permissions</span></span>
<span data-ttu-id="bdd79-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bdd79-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bdd79-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdd79-123">Permission type</span></span>      | <span data-ttu-id="bdd79-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdd79-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdd79-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdd79-125">Delegated (work or school account)</span></span> | <span data-ttu-id="bdd79-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bdd79-126">Calendars.Read</span></span>    |
|<span data-ttu-id="bdd79-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdd79-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdd79-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bdd79-128">Calendars.Read</span></span>    |
|<span data-ttu-id="bdd79-129">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdd79-129">Application</span></span> | <span data-ttu-id="bdd79-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bdd79-130">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdd79-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdd79-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="bdd79-132">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bdd79-132">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="bdd79-133">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="bdd79-133">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="bdd79-134">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="bdd79-134">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bdd79-135">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bdd79-135">Optional query parameters</span></span>
<span data-ttu-id="bdd79-136">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bdd79-136">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bdd79-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdd79-137">Request headers</span></span>
| <span data-ttu-id="bdd79-138">Имя</span><span class="sxs-lookup"><span data-stu-id="bdd79-138">Name</span></span>       | <span data-ttu-id="bdd79-139">Тип</span><span class="sxs-lookup"><span data-stu-id="bdd79-139">Type</span></span> | <span data-ttu-id="bdd79-140">Описание</span><span class="sxs-lookup"><span data-stu-id="bdd79-140">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bdd79-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdd79-141">Authorization</span></span>  | <span data-ttu-id="bdd79-142">string</span><span class="sxs-lookup"><span data-stu-id="bdd79-142">string</span></span>  | <span data-ttu-id="bdd79-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdd79-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdd79-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bdd79-145">Request body</span></span>
<span data-ttu-id="bdd79-146">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bdd79-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdd79-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdd79-147">Response</span></span>

<span data-ttu-id="bdd79-148">В случае успеха этот метод возвращает код отклика `200 OK` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bdd79-148">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bdd79-149">Пример</span><span class="sxs-lookup"><span data-stu-id="bdd79-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bdd79-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdd79-150">Request</span></span>
<span data-ttu-id="bdd79-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdd79-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="bdd79-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdd79-152">Response</span></span>
<span data-ttu-id="bdd79-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bdd79-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
