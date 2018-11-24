# <a name="get-directoryobject"></a><span data-ttu-id="ae3ff-101">Получение объекта DirectoryObject</span><span class="sxs-lookup"><span data-stu-id="ae3ff-101">Get directoryObject</span></span>

<span data-ttu-id="ae3ff-102">Получение свойств и связей объекта directoryObject.</span><span class="sxs-lookup"><span data-stu-id="ae3ff-102">Retrieve the properties and relationships of directoryObject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae3ff-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae3ff-103">Permissions</span></span>
<span data-ttu-id="ae3ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae3ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ae3ff-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae3ff-106">Permission type</span></span>      | <span data-ttu-id="ae3ff-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae3ff-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae3ff-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae3ff-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ae3ff-109">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae3ff-109">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae3ff-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae3ff-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae3ff-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae3ff-111">Not supported.</span></span>    |
|<span data-ttu-id="ae3ff-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae3ff-112">Application</span></span> | <span data-ttu-id="ae3ff-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae3ff-113">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae3ff-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae3ff-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae3ff-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ae3ff-115">Optional query parameters</span></span>
<span data-ttu-id="ae3ff-116">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ae3ff-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ae3ff-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae3ff-117">Request headers</span></span>
| <span data-ttu-id="ae3ff-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ae3ff-118">Name</span></span>       | <span data-ttu-id="ae3ff-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ae3ff-119">Type</span></span> | <span data-ttu-id="ae3ff-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ae3ff-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ae3ff-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae3ff-121">Authorization</span></span>  | <span data-ttu-id="ae3ff-122">string</span><span class="sxs-lookup"><span data-stu-id="ae3ff-122">string</span></span>  | <span data-ttu-id="ae3ff-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae3ff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae3ff-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae3ff-125">Request body</span></span>
<span data-ttu-id="ae3ff-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae3ff-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae3ff-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae3ff-127">Response</span></span>

<span data-ttu-id="ae3ff-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ae3ff-128">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae3ff-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ae3ff-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae3ff-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae3ff-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="ae3ff-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae3ff-131">Response</span></span>
<span data-ttu-id="ae3ff-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae3ff-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
