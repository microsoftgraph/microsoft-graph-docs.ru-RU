# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="a535d-101">Восстановление предыдущей версии ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="a535d-101">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="a535d-102">Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="a535d-102">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="a535d-103">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.</span><span class="sxs-lookup"><span data-stu-id="a535d-103">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="a535d-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a535d-104">Permissions</span></span>

<span data-ttu-id="a535d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a535d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a535d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a535d-107">Permission type</span></span>      | <span data-ttu-id="a535d-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a535d-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a535d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a535d-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a535d-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a535d-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a535d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a535d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a535d-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a535d-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a535d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a535d-113">Application</span></span> | <span data-ttu-id="a535d-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a535d-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a535d-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a535d-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="a535d-116">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a535d-116">Request body</span></span>

<span data-ttu-id="a535d-117">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="a535d-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="a535d-118">Пример</span><span class="sxs-lookup"><span data-stu-id="a535d-118">Example</span></span>

<span data-ttu-id="a535d-119">В этом примере восстанавливается версия файла, указанная по `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="a535d-119">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="a535d-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="a535d-120">Response</span></span>

<span data-ttu-id="a535d-121">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a535d-121">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
