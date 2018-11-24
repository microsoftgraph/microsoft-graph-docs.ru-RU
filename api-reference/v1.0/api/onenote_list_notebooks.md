# <a name="list-notebooks"></a><span data-ttu-id="4a270-101">Перечисление записных книжек</span><span class="sxs-lookup"><span data-stu-id="4a270-101">List notebooks</span></span>

<span data-ttu-id="4a270-102">Получение списка объектов [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="4a270-102">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a270-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a270-103">Permissions</span></span>
<span data-ttu-id="4a270-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a270-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4a270-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a270-106">Permission type</span></span>      | <span data-ttu-id="4a270-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a270-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a270-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a270-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4a270-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a270-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4a270-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a270-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a270-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a270-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4a270-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a270-112">Application</span></span> | <span data-ttu-id="4a270-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a270-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a270-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a270-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4a270-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4a270-115">Optional query parameters</span></span>
<span data-ttu-id="4a270-116">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4a270-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="4a270-117">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="4a270-117">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="4a270-118">Допустимые значения `expand` для записных книжек: `sections` и `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="4a270-118">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a270-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a270-119">Request headers</span></span>
| <span data-ttu-id="4a270-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4a270-120">Name</span></span>       | <span data-ttu-id="4a270-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4a270-121">Type</span></span> | <span data-ttu-id="4a270-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4a270-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4a270-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a270-123">Authorization</span></span>  | <span data-ttu-id="4a270-124">string</span><span class="sxs-lookup"><span data-stu-id="4a270-124">string</span></span>  | <span data-ttu-id="4a270-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a270-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a270-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4a270-127">Accept</span></span> | <span data-ttu-id="4a270-128">строка</span><span class="sxs-lookup"><span data-stu-id="4a270-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4a270-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a270-129">Request body</span></span>
<span data-ttu-id="4a270-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a270-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a270-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a270-131">Response</span></span>

<span data-ttu-id="4a270-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4a270-132">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a270-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4a270-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a270-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a270-134">Request</span></span>
<span data-ttu-id="4a270-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a270-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="4a270-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a270-136">Response</span></span>
<span data-ttu-id="4a270-p103">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a270-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 369

{
  "value": [
    {
      "isDefault": true,
      "userRole": {
      },
      "isShared": true,
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
      "links": {
        "oneNoteClientUrl": {
          "href": "href-value"
        },
        "oneNoteWebUrl": {
          "href": "href-value"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->