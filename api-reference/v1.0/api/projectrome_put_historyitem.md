# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="10ab1-101">Создать или заменить historyItem</span><span class="sxs-lookup"><span data-stu-id="10ab1-101">Create or replace a history item</span></span>

<span data-ttu-id="10ab1-102">Создание нового или замена существующего элемента журнала для действия существующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="10ab1-102">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="10ab1-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10ab1-103">Permissions</span></span>

<span data-ttu-id="10ab1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="10ab1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="10ab1-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10ab1-106">Permission type</span></span>      | <span data-ttu-id="10ab1-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10ab1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10ab1-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10ab1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="10ab1-109">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="10ab1-109">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="10ab1-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10ab1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10ab1-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="10ab1-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="10ab1-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="10ab1-112">Application</span></span> | <span data-ttu-id="10ab1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10ab1-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="10ab1-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10ab1-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="10ab1-115">ИД должен быть идентификатором GUID.</span><span class="sxs-lookup"><span data-stu-id="10ab1-115">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10ab1-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10ab1-116">Request headers</span></span>

|<span data-ttu-id="10ab1-117">Имя</span><span class="sxs-lookup"><span data-stu-id="10ab1-117">Name</span></span> | <span data-ttu-id="10ab1-118">Тип</span><span class="sxs-lookup"><span data-stu-id="10ab1-118">Type</span></span> | <span data-ttu-id="10ab1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="10ab1-119">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="10ab1-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10ab1-120">Authorization</span></span> | <span data-ttu-id="10ab1-121">строка</span><span class="sxs-lookup"><span data-stu-id="10ab1-121">string</span></span> | <span data-ttu-id="10ab1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10ab1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="10ab1-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10ab1-124">Request body</span></span>

<span data-ttu-id="10ab1-125">В тексте запроса укажите представление JSON объекта [historyItem](../resources/projectrome_historyitem.md) .</span><span class="sxs-lookup"><span data-stu-id="10ab1-125">In the request body, supply a JSON representation of [directoryObject](../resources/projectrome_historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="10ab1-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ab1-126">Response</span></span>

<span data-ttu-id="10ab1-127">При успешном выполнении этот метод возвращает код отклика , если объект historyItem был создан, или  если объект historyItem был заменен.`201 Created` `200 OK`</span><span class="sxs-lookup"><span data-stu-id="10ab1-127">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="10ab1-128">Пример</span><span class="sxs-lookup"><span data-stu-id="10ab1-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="10ab1-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="10ab1-129">Request</span></span>

<span data-ttu-id="10ab1-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10ab1-130">Here is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_historyItem"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
Content-type: application/json
Content-length: 364

{
    "startedDateTime": "2015-02-11T20:54:04.3457274+00:00",
    "userTimezone": "Africa/Casablanca",
    "lastActiveDateTime": "2015-02-11T20:54:04.3457274+00:00"
}
```

#### <a name="response"></a><span data-ttu-id="10ab1-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="10ab1-131">Response</span></span>

<span data-ttu-id="10ab1-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10ab1-132">Here is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activityHistoryItem"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('user%40contoso.com')/activities('13881113971988980728')/historyItems/$entity",
    "status": "updated",
    "userTimezone": "Africa/Casablanca",
    "createdDateTime": "2018-02-26T20:28:22.14Z",
    "lastModifiedDateTime": "2018-02-26T20:28:22.155Z",
    "id": "9d0b74e4-4b41-43ea-b34d-f9c1bf9f809c",
    "startedDateTime": "2018-02-26T20:54:04.345Z",
    "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
    "expirationDateTime": "2018-03-28T20:28:22.14Z",
    "activeDurationSeconds": 20
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->