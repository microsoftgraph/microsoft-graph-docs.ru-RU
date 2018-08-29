# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="cd94b-101">Получение ресурса ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="cd94b-101">Get a ListItemVersion resource (preview)</span></span>

<span data-ttu-id="cd94b-102">В этой статье рассказывается, как получить метаданные для определенной версии ресурса [ListItem](../resources/listitem.md).</span><span class="sxs-lookup"><span data-stu-id="cd94b-102">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cd94b-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd94b-103">Permissions</span></span>

<span data-ttu-id="cd94b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cd94b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|            <span data-ttu-id="cd94b-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd94b-106">Permission type</span></span>             | <span data-ttu-id="cd94b-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd94b-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="cd94b-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd94b-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="cd94b-109">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd94b-109">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="cd94b-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd94b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd94b-111">Н/д</span><span class="sxs-lookup"><span data-stu-id="cd94b-111">n/a</span></span>                                         |
| <span data-ttu-id="cd94b-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd94b-112">Application</span></span>                            | <span data-ttu-id="cd94b-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd94b-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="cd94b-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd94b-114">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="cd94b-115">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd94b-115">Response</span></span>

<span data-ttu-id="cd94b-116">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [ListItemVersion](../resources/listitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cd94b-116">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="cd94b-117">Пример</span><span class="sxs-lookup"><span data-stu-id="cd94b-117">Example</span></span>

<span data-ttu-id="cd94b-118">В этом примере показано, как получить версию объекта listItem и расширить коллекцию полей для запроса значений полей в объекте listItem.</span><span class="sxs-lookup"><span data-stu-id="cd94b-118">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="cd94b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd94b-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="cd94b-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd94b-120">Response</span></span>

<span data-ttu-id="cd94b-121">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="cd94b-121">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
