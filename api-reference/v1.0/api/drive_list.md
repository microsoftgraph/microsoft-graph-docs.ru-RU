# <a name="list-available-drives"></a><span data-ttu-id="25452-101">Список доступных дисков</span><span class="sxs-lookup"><span data-stu-id="25452-101">List available drives</span></span>

<span data-ttu-id="25452-p101">Получение списка ресурсов [Drive](../resources/drive.md), доступных целевому объекту [User](../resources/user.md) или [Group](../resources/group.md). Приложение также может запросить набор библиотек документов на корневом сайте SharePoint.</span><span class="sxs-lookup"><span data-stu-id="25452-p101">Retrieve the list of [Drive](../resources/drive.md) resources available for a target [User](../resources/user.md) or [Group](../resources/group.md). Your app can also request the set of document libraries on the SharePoint root site.</span></span>

## <a name="permissions"></a><span data-ttu-id="25452-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25452-104">Permissions</span></span>

<span data-ttu-id="25452-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="25452-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="25452-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25452-107">Permission type</span></span>      | <span data-ttu-id="25452-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25452-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="25452-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25452-109">Delegated (work or school account)</span></span> | <span data-ttu-id="25452-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25452-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="25452-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25452-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25452-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25452-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="25452-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25452-113">Application</span></span> | <span data-ttu-id="25452-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25452-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="25452-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25452-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives
GET /me/drives
GET /sites/{site-id}/drives
```

## <a name="optional-query-parameters"></a><span data-ttu-id="25452-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="25452-116">Optional query parameters</span></span>

<span data-ttu-id="25452-117">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="25452-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="25452-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="25452-118">Request body</span></span>

<span data-ttu-id="25452-119">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25452-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25452-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="25452-120">Response</span></span>

<span data-ttu-id="25452-121">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Drive](../resources/drive.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="25452-121">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25452-122">Пример</span><span class="sxs-lookup"><span data-stu-id="25452-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="25452-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="25452-123">Request</span></span>

<span data-ttu-id="25452-124">Ниже приведен пример запроса на получение списка дисков пользователя.</span><span class="sxs-lookup"><span data-stu-id="25452-124">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drives"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/drives
```

##### <a name="response"></a><span data-ttu-id="25452-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="25452-125">Response</span></span>

<span data-ttu-id="25452-126">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="25452-126">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.drive",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 579

{
  "value": [
    {
      "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
      "driveType": "business",
      "owner": {
          "user": {
              "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
              "displayName": "Ryan Gregg"
          }
      },
      "quota": {
          "deleted": 256938,
          "remaining": 1099447353539,
          "state": "normal",
          "total": 1099511627776
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="25452-127">Заметки</span><span class="sxs-lookup"><span data-stu-id="25452-127">Remarks</span></span>

<span data-ttu-id="25452-p103">У большинства пользователей есть только ресурс Drive. Для групп и некоторых пользователей может быть доступно несколько дисков.</span><span class="sxs-lookup"><span data-stu-id="25452-p103">Most users will only have a single Drive resource. Groups and some users may have multiple drive available.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/List Drives"
}-->
