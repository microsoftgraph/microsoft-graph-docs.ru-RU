# <a name="get-entity"></a><span data-ttu-id="66435-101">Получение сущности</span><span class="sxs-lookup"><span data-stu-id="66435-101">Get entity</span></span>

<span data-ttu-id="66435-102">Получение свойств и связей объекта сущности.</span><span class="sxs-lookup"><span data-stu-id="66435-102">Retrieve the properties and relationships of entity object.</span></span>
## <a name="permissions"></a><span data-ttu-id="66435-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66435-103">Permissions</span></span>
<span data-ttu-id="66435-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="66435-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="66435-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66435-106">Permission type</span></span>      | <span data-ttu-id="66435-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66435-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66435-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66435-108">Delegated (work or school account)</span></span> | <span data-ttu-id="66435-109">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66435-109">Not supported.</span></span>    |
|<span data-ttu-id="66435-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66435-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66435-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66435-111">Not supported.</span></span>    |
|<span data-ttu-id="66435-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66435-112">Application</span></span> | <span data-ttu-id="66435-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66435-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66435-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66435-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http

```
## <a name="optional-query-parameters"></a><span data-ttu-id="66435-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="66435-115">Optional query parameters</span></span>
<span data-ttu-id="66435-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="66435-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="66435-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66435-117">Request headers</span></span>
| <span data-ttu-id="66435-118">Имя</span><span class="sxs-lookup"><span data-stu-id="66435-118">Name</span></span>       | <span data-ttu-id="66435-119">Тип</span><span class="sxs-lookup"><span data-stu-id="66435-119">Type</span></span> | <span data-ttu-id="66435-120">Описание</span><span class="sxs-lookup"><span data-stu-id="66435-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="66435-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="66435-121">Authorization</span></span>  | <span data-ttu-id="66435-122">string</span><span class="sxs-lookup"><span data-stu-id="66435-122">string</span></span>  | <span data-ttu-id="66435-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66435-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66435-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66435-125">Request body</span></span>
<span data-ttu-id="66435-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="66435-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66435-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="66435-127">Response</span></span>

<span data-ttu-id="66435-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [entity](../resources/entity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66435-128">If successful, this method returns a `200 OK` response code and [entity](../resources/entity.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="66435-129">Пример</span><span class="sxs-lookup"><span data-stu-id="66435-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66435-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="66435-130">Request</span></span>
<span data-ttu-id="66435-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66435-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_entity"
}-->
```http

```
##### <a name="response"></a><span data-ttu-id="66435-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="66435-132">Response</span></span>
<span data-ttu-id="66435-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="66435-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 22

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get entity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
