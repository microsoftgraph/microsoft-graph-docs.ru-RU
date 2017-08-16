# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="601d4-101">Отправка или замена содержимого элемента driveItem</span><span class="sxs-lookup"><span data-stu-id="601d4-101">Upload or replace the contents of a driveItem</span></span>

<span data-ttu-id="601d4-p101">Используя простой API отправки, вы можете отправлять содержимое нового файла или обновлять содержимое существующего файла с помощью одного вызова API. Этот метод поддерживает файлы размером не более 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="601d4-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="601d4-104">Сведения о том, как отправлять большие файлы, см. в разделе [Отправка больших файлов с помощью сеанса отправки](item_createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="601d4-104">To upload large files see [Upload large files with an upload session](item_createuploadsession.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="601d4-105">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="601d4-105">Prerequisites</span></span>
<span data-ttu-id="601d4-106">Для применения этого API требуется одна из указанных **областей**:</span><span class="sxs-lookup"><span data-stu-id="601d4-106">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="601d4-107">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="601d4-107">Files.ReadWrite</span></span>
* <span data-ttu-id="601d4-108">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="601d4-108">Files.ReadWrite.All</span></span>
* <span data-ttu-id="601d4-109">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="601d4-109">Sites.ReadWrite.All</span></span>


## <a name="http-request"></a><span data-ttu-id="601d4-110">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="601d4-110">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/root:/{parent-path}/{filename}:/content
PUT /me/drive/items/{parent-id}/children/{filename}/content
PUT /groups/{id}/drive/items/{parent-id}/children/{filename}/content
```

## <a name="request-body"></a><span data-ttu-id="601d4-111">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="601d4-111">Request body</span></span>
<span data-ttu-id="601d4-112">Содержимое текста запроса должно представлять собой двоичный поток файла, который необходимо отправить.</span><span class="sxs-lookup"><span data-stu-id="601d4-112">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="601d4-113">Отклик</span><span class="sxs-lookup"><span data-stu-id="601d4-113">Response</span></span>

<span data-ttu-id="601d4-114">При успешном выполнении этот метод возвращает объект [driveItem](../resources/driveitem.md) в тексте отклика для вновь созданного файла.</span><span class="sxs-lookup"><span data-stu-id="601d4-114">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created file.</span></span>

## <a name="example"></a><span data-ttu-id="601d4-115">Пример</span><span class="sxs-lookup"><span data-stu-id="601d4-115">Example</span></span>
<span data-ttu-id="601d4-116">В этом примере показано, как отправить файл с указанием пути в хранилище OneDrive пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="601d4-116">This example uploads a file by path to the signed-in user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "upload_item"
}-->
```http
PUT /me/drive/root:/{item-path}:/content
Content-type: text/plain

The contents of the file goes here.
```

##### <a name="response"></a><span data-ttu-id="601d4-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="601d4-117">Response</span></span>

<span data-ttu-id="601d4-118">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="601d4-118">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "myfile.jpg",
  "size": 10191,
  "file": { }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upload item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
