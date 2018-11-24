# <a name="list-registeredowners"></a><span data-ttu-id="58bad-101">Список registeredOwners</span><span class="sxs-lookup"><span data-stu-id="58bad-101">List registeredOwners</span></span>

<span data-ttu-id="58bad-102">Получение списка пользователей, являющихся зарегистрированными владельцами устройства.</span><span class="sxs-lookup"><span data-stu-id="58bad-102">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="58bad-103">Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство.</span><span class="sxs-lookup"><span data-stu-id="58bad-103">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="58bad-104">Зарегистрированный владелец задается при регистрации.</span><span class="sxs-lookup"><span data-stu-id="58bad-104">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="58bad-105">Сейчас можно настроить лишь одного такого владельца.</span><span class="sxs-lookup"><span data-stu-id="58bad-105">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="58bad-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58bad-106">Permissions</span></span>
<span data-ttu-id="58bad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="58bad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="58bad-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58bad-109">Permission type</span></span>      | <span data-ttu-id="58bad-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58bad-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58bad-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58bad-111">Delegated (work or school account)</span></span> | <span data-ttu-id="58bad-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="58bad-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="58bad-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58bad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58bad-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58bad-114">Not supported.</span></span>    |
|<span data-ttu-id="58bad-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="58bad-115">Application</span></span> | <span data-ttu-id="58bad-116">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58bad-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58bad-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58bad-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="58bad-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="58bad-118">Optional query parameters</span></span>
<span data-ttu-id="58bad-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="58bad-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="58bad-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58bad-120">Request headers</span></span>
| <span data-ttu-id="58bad-121">Имя</span><span class="sxs-lookup"><span data-stu-id="58bad-121">Name</span></span>       | <span data-ttu-id="58bad-122">Тип</span><span class="sxs-lookup"><span data-stu-id="58bad-122">Type</span></span> | <span data-ttu-id="58bad-123">Описание</span><span class="sxs-lookup"><span data-stu-id="58bad-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="58bad-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="58bad-124">Authorization</span></span>  | <span data-ttu-id="58bad-125">string</span><span class="sxs-lookup"><span data-stu-id="58bad-125">string</span></span>  | <span data-ttu-id="58bad-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58bad-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58bad-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58bad-128">Request body</span></span>
<span data-ttu-id="58bad-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="58bad-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58bad-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="58bad-130">Response</span></span>

<span data-ttu-id="58bad-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58bad-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="58bad-132">Пример</span><span class="sxs-lookup"><span data-stu-id="58bad-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58bad-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="58bad-133">Request</span></span>
<span data-ttu-id="58bad-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58bad-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="58bad-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="58bad-135">Response</span></span>
<span data-ttu-id="58bad-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="58bad-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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