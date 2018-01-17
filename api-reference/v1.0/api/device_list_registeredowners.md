# <a name="list-registeredowners"></a><span data-ttu-id="01f2f-101">Список registeredOwners</span><span class="sxs-lookup"><span data-stu-id="01f2f-101">List registeredOwners</span></span>

<span data-ttu-id="01f2f-102">Получение списка пользователей, являющихся зарегистрированными владельцами устройства.</span><span class="sxs-lookup"><span data-stu-id="01f2f-102">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="01f2f-103">Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство.</span><span class="sxs-lookup"><span data-stu-id="01f2f-103">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="01f2f-104">Зарегистрированный владелец задается при регистрации.</span><span class="sxs-lookup"><span data-stu-id="01f2f-104">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="01f2f-105">Сейчас можно настроить лишь одного такого владельца.</span><span class="sxs-lookup"><span data-stu-id="01f2f-105">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="01f2f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01f2f-106">Permissions</span></span>
<span data-ttu-id="01f2f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="01f2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="01f2f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01f2f-109">Permission type</span></span>      | <span data-ttu-id="01f2f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01f2f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01f2f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01f2f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="01f2f-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="01f2f-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="01f2f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01f2f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01f2f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01f2f-114">Not supported.</span></span>    |
|<span data-ttu-id="01f2f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01f2f-115">Application</span></span> | <span data-ttu-id="01f2f-116">Device.ReadWrite.All и User.ReadBasic.All или Directory.Read.All либо Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01f2f-116">Device.ReadWrite.All and User.ReadBasic.All or Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01f2f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01f2f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01f2f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="01f2f-118">Optional query parameters</span></span>
<span data-ttu-id="01f2f-119">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="01f2f-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="01f2f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01f2f-120">Request headers</span></span>
| <span data-ttu-id="01f2f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="01f2f-121">Name</span></span>       | <span data-ttu-id="01f2f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="01f2f-122">Type</span></span> | <span data-ttu-id="01f2f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="01f2f-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="01f2f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="01f2f-124">Authorization</span></span>  | <span data-ttu-id="01f2f-125">string</span><span class="sxs-lookup"><span data-stu-id="01f2f-125">string</span></span>  | <span data-ttu-id="01f2f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01f2f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01f2f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01f2f-128">Request body</span></span>
<span data-ttu-id="01f2f-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01f2f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01f2f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="01f2f-130">Response</span></span>

<span data-ttu-id="01f2f-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01f2f-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01f2f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="01f2f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01f2f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="01f2f-133">Request</span></span>
<span data-ttu-id="01f2f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01f2f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="01f2f-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="01f2f-135">Response</span></span>
<span data-ttu-id="01f2f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="01f2f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->