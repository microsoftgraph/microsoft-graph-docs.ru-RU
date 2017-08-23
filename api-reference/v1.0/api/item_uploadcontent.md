# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="bd00d-101">Отправка или замена содержимого элемента driveItem</span><span class="sxs-lookup"><span data-stu-id="bd00d-101">Upload or replace the contents of a driveItem</span></span>

<span data-ttu-id="bd00d-p101">Используя простой API отправки, вы можете отправлять содержимое нового файла или обновлять содержимое существующего файла с помощью одного вызова API. Этот метод поддерживает файлы размером не более 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="bd00d-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="bd00d-104">Сведения о том, как отправлять большие файлы, см. в разделе [Отправка больших файлов с помощью сеанса отправки](item_createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="bd00d-104">To upload large files see [Upload large files with an upload session](item_createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bd00d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd00d-105">Permissions</span></span>
<span data-ttu-id="bd00d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bd00d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bd00d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd00d-108">Permission type</span></span>      | <span data-ttu-id="bd00d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd00d-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="bd00d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd00d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bd00d-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd00d-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="bd00d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd00d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd00d-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd00d-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="bd00d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd00d-114">Application</span></span> | <span data-ttu-id="bd00d-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd00d-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bd00d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd00d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/root:/{parent-path}/{filename}:/content
PUT /me/drive/items/{parent-id}/children/{filename}/content
PUT /groups/{id}/drive/items/{parent-id}/children/{filename}/content
```

## <a name="request-body"></a><span data-ttu-id="bd00d-117">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd00d-117">Request body</span></span>
<span data-ttu-id="bd00d-118">Содержимое текста запроса должно представлять собой двоичный поток файла, который необходимо отправить.</span><span class="sxs-lookup"><span data-stu-id="bd00d-118">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="bd00d-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd00d-119">Response</span></span>

<span data-ttu-id="bd00d-120">При успешном выполнении этот метод возвращает объект [driveItem](../resources/driveitem.md) в тексте отклика для вновь созданного файла.</span><span class="sxs-lookup"><span data-stu-id="bd00d-120">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created file.</span></span>

## <a name="example"></a><span data-ttu-id="bd00d-121">Пример</span><span class="sxs-lookup"><span data-stu-id="bd00d-121">Example</span></span>
<span data-ttu-id="bd00d-122">В этом примере показано, как отправить файл с указанием пути в хранилище OneDrive пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="bd00d-122">This example uploads a file by path to the signed-in user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "upload_item"
}-->
```http
PUT /me/drive/root:/{item-path}:/content
Content-type: text/plain

The contents of the file goes here.
```

##### <a name="response"></a><span data-ttu-id="bd00d-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd00d-123">Response</span></span>

<span data-ttu-id="bd00d-124">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd00d-124">The following example shows the response.</span></span>

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
