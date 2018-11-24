# <a name="get-sectiongroup"></a><span data-ttu-id="1e7ea-101">Получение объекта sectionGroup</span><span class="sxs-lookup"><span data-stu-id="1e7ea-101">Get sectionGroup</span></span>

<span data-ttu-id="1e7ea-102">Получение свойств и связей объекта [sectionGroup](../resources/sectiongroup.md).</span><span class="sxs-lookup"><span data-stu-id="1e7ea-102">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e7ea-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e7ea-103">Permissions</span></span>
<span data-ttu-id="1e7ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1e7ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1e7ea-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e7ea-106">Permission type</span></span>      | <span data-ttu-id="1e7ea-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e7ea-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e7ea-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e7ea-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1e7ea-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e7ea-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1e7ea-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e7ea-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e7ea-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e7ea-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1e7ea-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e7ea-112">Application</span></span> | <span data-ttu-id="1e7ea-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e7ea-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e7ea-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e7ea-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1e7ea-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1e7ea-115">Optional query parameters</span></span>
<span data-ttu-id="1e7ea-116">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1e7ea-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1e7ea-p102">Запрос по умолчанию разворачивает `parentNotebook` и выбирает соответствующие свойства `id`, `name` и `self`. Допустимые значения `expand` для групп разделов: `parentNotebook` и `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="1e7ea-p102">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties. Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e7ea-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e7ea-119">Request headers</span></span>
| <span data-ttu-id="1e7ea-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1e7ea-120">Name</span></span>       | <span data-ttu-id="1e7ea-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1e7ea-121">Type</span></span> | <span data-ttu-id="1e7ea-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1e7ea-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1e7ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e7ea-123">Authorization</span></span>  | <span data-ttu-id="1e7ea-124">string</span><span class="sxs-lookup"><span data-stu-id="1e7ea-124">string</span></span>  | <span data-ttu-id="1e7ea-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e7ea-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1e7ea-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1e7ea-127">Accept</span></span> | <span data-ttu-id="1e7ea-128">строка</span><span class="sxs-lookup"><span data-stu-id="1e7ea-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1e7ea-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e7ea-129">Request body</span></span>
<span data-ttu-id="1e7ea-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1e7ea-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e7ea-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="1e7ea-131">Response</span></span>

<span data-ttu-id="1e7ea-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [sectionGroup](../resources/sectiongroup.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1e7ea-132">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1e7ea-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1e7ea-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e7ea-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e7ea-134">Request</span></span>
<span data-ttu-id="1e7ea-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e7ea-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="1e7ea-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e7ea-136">Response</span></span>
<span data-ttu-id="1e7ea-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e7ea-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "displayName": "name-value",  
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get sectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->