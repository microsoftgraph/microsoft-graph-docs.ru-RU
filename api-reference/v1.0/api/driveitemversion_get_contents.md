# <a name="download-contents-of-a-driveitemversion-resource"></a><span data-ttu-id="f8722-101">Загрузка содержимого ресурса DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="f8722-101">Download contents of a DriveItemVersion resource (preview)</span></span>

<span data-ttu-id="f8722-102">Получение содержимого определенной версии ресурса [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f8722-102">Retrieve the contents of a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8722-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8722-103">Permissions</span></span>

<span data-ttu-id="f8722-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f8722-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f8722-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8722-106">Permission type</span></span>      | <span data-ttu-id="f8722-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8722-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8722-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8722-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f8722-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8722-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f8722-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8722-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8722-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8722-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f8722-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8722-112">Application</span></span> | <span data-ttu-id="f8722-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8722-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="f8722-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8722-114">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="f8722-115">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8722-115">Response</span></span>

<span data-ttu-id="f8722-116">Возвращает отклик `302 Found`, который выполняет перенаправление на URL-адрес, прошедший предварительную проверку подлинности и предназначенный для скачивания байтов файла.</span><span class="sxs-lookup"><span data-stu-id="f8722-116">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="f8722-p102">Чтобы загрузить содержимое файла, приложению необходимо будет следовать заголовку `Location` в отклике. Многие библиотеки клиентов HTTP будут автоматически следовать перенаправлению 302 и немедленно начинать загрузку файла.</span><span class="sxs-lookup"><span data-stu-id="f8722-p102">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="f8722-119">URL-адреса загрузки, прошедшие предварительную проверку подлинности, действуют только в течение короткого периода времени (несколько минут), и для их скачивания не требуется заголовок `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f8722-119">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="f8722-120">Пример</span><span class="sxs-lookup"><span data-stu-id="f8722-120">Example</span></span>

<span data-ttu-id="f8722-121">В этом примере показано, как получить версию файла в объекте drive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="f8722-121">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="f8722-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8722-122">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```

### <a name="response"></a><span data-ttu-id="f8722-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8722-123">Response</span></span>

<span data-ttu-id="f8722-124">Возвращает перенаправление на расположение, из которого можно скачать содержимое версии.</span><span class="sxs-lookup"><span data-stu-id="f8722-124">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Found
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="f8722-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="f8722-125">Remarks</span></span>

<span data-ttu-id="f8722-126">OneDrive не сохраняет полные метаданные для предыдущих версий файла.</span><span class="sxs-lookup"><span data-stu-id="f8722-126">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="f8722-127">Когда ваше приложение получает список доступных версий для файла, возвращается ресурс [DriveItemVersion](../resources/driveItemVersion.md), в котором представлены доступные сведения об определенной версии.</span><span class="sxs-lookup"><span data-stu-id="f8722-127">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveItemVersion.md) resource is returned that provides the available information about the specific version.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
