# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="a2333-101">Восстановление предыдущей версии ресурса ListItem</span><span class="sxs-lookup"><span data-stu-id="a2333-101">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="a2333-102">Восстановление предыдущей версии ресурса ListItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="a2333-102">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="a2333-103">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии элемента.</span><span class="sxs-lookup"><span data-stu-id="a2333-103">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2333-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2333-104">Permissions</span></span>

<span data-ttu-id="a2333-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a2333-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|            <span data-ttu-id="a2333-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2333-107">Permission type</span></span>             |         <span data-ttu-id="a2333-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2333-108">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="a2333-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2333-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2333-110">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a2333-110">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="a2333-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2333-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2333-112">Н/д</span><span class="sxs-lookup"><span data-stu-id="a2333-112">n/a</span></span>                                                          |
| <span data-ttu-id="a2333-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2333-113">Application</span></span>                            | <span data-ttu-id="a2333-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a2333-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2333-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2333-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="a2333-116">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a2333-116">Request body</span></span>

<span data-ttu-id="a2333-117">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="a2333-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="a2333-118">Пример</span><span class="sxs-lookup"><span data-stu-id="a2333-118">Example</span></span>

<span data-ttu-id="a2333-119">В этом примере восстанавливается версия ресурса listItem, указанная пр `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="a2333-119">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="a2333-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2333-120">Response</span></span>

<span data-ttu-id="a2333-121">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a2333-121">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
