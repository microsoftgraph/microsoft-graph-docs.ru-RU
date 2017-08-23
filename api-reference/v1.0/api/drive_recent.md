# <a name="list-recent-files"></a><span data-ttu-id="80397-101">Список последних файлов</span><span class="sxs-lookup"><span data-stu-id="80397-101">List recent files</span></span>

<span data-ttu-id="80397-p101">Указание набора элементов, которые недавно использовались пользователем, вошедшим в свою учетную запись. Эта коллекция содержит элементы, которые находятся на диске пользователя, а также элементы, к которым у него есть доступ с других дисков.</span><span class="sxs-lookup"><span data-stu-id="80397-p101">List a set of items that have been recently used by the signed in user. This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="80397-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80397-104">Permissions</span></span>
<span data-ttu-id="80397-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="80397-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="80397-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80397-107">Permission type</span></span>      | <span data-ttu-id="80397-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80397-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="80397-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80397-109">Delegated (work or school account)</span></span> | <span data-ttu-id="80397-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80397-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="80397-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80397-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80397-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80397-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="80397-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80397-113">Application</span></span> | <span data-ttu-id="80397-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80397-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="80397-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80397-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
GET /me/drive/recent
```

## <a name="request-body"></a><span data-ttu-id="80397-116">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="80397-116">Request body</span></span>
<span data-ttu-id="80397-117">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="80397-117">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="80397-118">Пример</span><span class="sxs-lookup"><span data-stu-id="80397-118">Example</span></span>

<!-- { "blockType": "request", "name": "drive-recent", "scopes": "files.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/recent
```

## <a name="response"></a><span data-ttu-id="80397-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="80397-119">Response</span></span>

<span data-ttu-id="80397-p103">Возвращает коллекцию ресурсов [DriveItem](../resources/driveitem.md) для элементов, к которым владелец диска недавно получал доступ. Элементы не на диске пользователя будут содержать аспект [RemoteItem](../resources/remoteitem.md), который предоставляет данные для доступа к общему элементу.</span><span class="sxs-lookup"><span data-stu-id="80397-p103">This returns a collection of [DriveItem](../resources/driveitem.md) resources for items which the owner of the drive has recently accessed. Items outside of the user's drive will include the [RemoteItem](../resources/remoteitem.md) facet, which provides information to access the shared item.</span></span>


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "remoteItem":
      {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "file": { },
      "size": 37810,
      "parentReference": {
        "driveId": "1312def",
        "id": "1312def!123"
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="80397-122">Заметки</span><span class="sxs-lookup"><span data-stu-id="80397-122">Remarks</span></span>

<span data-ttu-id="80397-p104">Некоторые элементы driveItem, возвращенные **последним** действием, будут содержать аспект **remoteItem**, который указывает, что это элементы с другого диска. Чтобы получить доступ к исходному объекту driveItem, следует отправить запрос, используя данные, указанные в **remoteItem** в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="80397-p104">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- {"blockType": "ignored"} -->
```http
GET https://graph.microsoft.com/v1.0/drives/{remoteItem.driveId}/items/{remoteItem.id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of files shared with the signed-in user.",
  "keywords": "sharedWithMe onedrive shared files",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Shared with me"
} -->
