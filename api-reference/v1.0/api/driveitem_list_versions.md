# <a name="listing-versions-of-a-driveitem"></a><span data-ttu-id="ad62c-101">Перечисление версий ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="ad62c-101">Listing versions of a DriveItem (preview)</span></span>

<span data-ttu-id="ad62c-102">OneDrive и SharePoint можно настроить на хранение журнала для файлов.</span><span class="sxs-lookup"><span data-stu-id="ad62c-102">OneDrive and SharePoint can be configured to retain the history for files.</span></span>
<span data-ttu-id="ad62c-103">В зависимости от того, каковы служба и конфигурация, новую версию можно создавать при каждом изменении или сохранении, создавать вручную или не создавать никогда.</span><span class="sxs-lookup"><span data-stu-id="ad62c-103">Depending on the service and configuration, a new version can be created for each edit, each time the file is saved, manually, or never.</span></span>

<span data-ttu-id="ad62c-104">Предыдущие версии документа могут храниться в течение ограниченного времени в зависимости от того, каковы параметры администратора, которые могут быть уникальными для каждого пользователя или расположения.</span><span class="sxs-lookup"><span data-stu-id="ad62c-104">Previous versions of a document may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad62c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad62c-105">Permissions</span></span>

<span data-ttu-id="ad62c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ad62c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ad62c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad62c-108">Permission type</span></span>      | <span data-ttu-id="ad62c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad62c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad62c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad62c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ad62c-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad62c-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad62c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad62c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad62c-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad62c-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad62c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad62c-114">Application</span></span> | <span data-ttu-id="ad62c-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad62c-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="ad62c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad62c-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="ad62c-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad62c-117">Response</span></span>

<span data-ttu-id="ad62c-118">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [DriveItemVersion](../resources/driveitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ad62c-118">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/driveitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="ad62c-119">Пример</span><span class="sxs-lookup"><span data-stu-id="ad62c-119">Example</span></span>

<span data-ttu-id="ad62c-120">В этом примере показано, как получить версии файла для объекта Drive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="ad62c-120">This example retrieves the versions of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="ad62c-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad62c-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="ad62c-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad62c-122">Response</span></span>

<span data-ttu-id="ad62c-123">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="ad62c-123">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
      "size": 123
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z",
      "size": 62
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z",
      "size": 16
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="ad62c-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="ad62c-124">Remarks</span></span>

<span data-ttu-id="ad62c-125">OneDrive не сохраняет полные метаданные для предыдущих версий файла.</span><span class="sxs-lookup"><span data-stu-id="ad62c-125">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="ad62c-126">Когда ваше приложение получает список доступных версий для файла, возвращается ресурс [DriveItemVersion](../resources/driveItemVersion.md), в котором представлены доступные сведения об определенной версии.</span><span class="sxs-lookup"><span data-stu-id="ad62c-126">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveItemVersion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
