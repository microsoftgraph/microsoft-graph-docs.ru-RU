# <a name="list-registeredusers"></a><span data-ttu-id="92901-101">Список registeredUsers</span><span class="sxs-lookup"><span data-stu-id="92901-101">List registeredUsers</span></span>

<span data-ttu-id="92901-102">Получение списка пользователей, являющихся зарегистрированными пользователями устройства.</span><span class="sxs-lookup"><span data-stu-id="92901-102">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="92901-103">В случае зарегистрированных личных устройств или устройств, присоединенных через облако, при регистрации для обычных пользователей задается то же значение, что и для владельцев.</span><span class="sxs-lookup"><span data-stu-id="92901-103">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="92901-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="92901-104">Permissions</span></span>
<span data-ttu-id="92901-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="92901-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="92901-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92901-107">Permission type</span></span>      | <span data-ttu-id="92901-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92901-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92901-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92901-109">Delegated (work or school account)</span></span> | <span data-ttu-id="92901-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="92901-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="92901-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92901-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92901-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92901-112">Not supported.</span></span>    |
|<span data-ttu-id="92901-113">Для приложения</span><span class="sxs-lookup"><span data-stu-id="92901-113">Application</span></span> | <span data-ttu-id="92901-114">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92901-114">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="92901-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92901-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="92901-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="92901-116">Optional query parameters</span></span>
<span data-ttu-id="92901-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="92901-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="92901-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92901-118">Request headers</span></span>
| <span data-ttu-id="92901-119">Имя</span><span class="sxs-lookup"><span data-stu-id="92901-119">Name</span></span>       | <span data-ttu-id="92901-120">Тип</span><span class="sxs-lookup"><span data-stu-id="92901-120">Type</span></span> | <span data-ttu-id="92901-121">Описание</span><span class="sxs-lookup"><span data-stu-id="92901-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="92901-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92901-122">Authorization</span></span>  | <span data-ttu-id="92901-123">string</span><span class="sxs-lookup"><span data-stu-id="92901-123">string</span></span>  | <span data-ttu-id="92901-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92901-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92901-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92901-126">Request body</span></span>
<span data-ttu-id="92901-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="92901-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92901-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="92901-128">Response</span></span>

<span data-ttu-id="92901-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="92901-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="92901-130">Пример</span><span class="sxs-lookup"><span data-stu-id="92901-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92901-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="92901-131">Request</span></span>
<span data-ttu-id="92901-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92901-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="92901-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="92901-133">Response</span></span>
<span data-ttu-id="92901-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="92901-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->