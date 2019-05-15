---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Отправка небольших файлов
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 28c3076c351755cf65ae1cbd83a6cc2c36c1544b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33960888"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="bb9ec-102">Отправка или замена содержимого элемента DriveItem</span><span class="sxs-lookup"><span data-stu-id="bb9ec-102">Upload or replace the contents of a DriveItem</span></span>

<span data-ttu-id="bb9ec-p101">Используя простой API отправки, вы можете отправлять содержимое нового файла или обновлять содержимое существующего файла с помощью одного вызова API. Этот метод поддерживает файлы размером не более 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="bb9ec-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="bb9ec-105">Сведения о том, как отправлять большие файлы, см. в разделе [Отправка больших файлов с помощью сеанса отправки](driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="bb9ec-105">To upload large files see [Upload large files with an upload session](driveitem-createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bb9ec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb9ec-106">Permissions</span></span>

<span data-ttu-id="bb9ec-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb9ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb9ec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb9ec-109">Permission type</span></span>      | <span data-ttu-id="bb9ec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb9ec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb9ec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb9ec-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bb9ec-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb9ec-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bb9ec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb9ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb9ec-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb9ec-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="bb9ec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb9ec-115">Application</span></span> | <span data-ttu-id="bb9ec-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb9ec-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request-to-replace-an-existing-item"></a><span data-ttu-id="bb9ec-117">HTTP-запрос (для замены существующего элемента)</span><span class="sxs-lookup"><span data-stu-id="bb9ec-117">HTTP request (to replace an existing item)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a><span data-ttu-id="bb9ec-118">HTTP-запрос (для отправки нового файла)</span><span class="sxs-lookup"><span data-stu-id="bb9ec-118">HTTP request (to upload a new file)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a><span data-ttu-id="bb9ec-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bb9ec-119">Request body</span></span>

<span data-ttu-id="bb9ec-120">Содержимое текста запроса должно представлять собой двоичный поток файла, который необходимо отправить.</span><span class="sxs-lookup"><span data-stu-id="bb9ec-120">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="bb9ec-121">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb9ec-121">Response</span></span>

<span data-ttu-id="bb9ec-122">При успешном выполнении этот метод возвращает объект [driveItem](../resources/driveitem.md) для вновь созданного или обновленного файла в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bb9ec-122">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created or updated file.</span></span>

## <a name="example-upload-a-new-file"></a><span data-ttu-id="bb9ec-123">Пример (отправка нового файла)</span><span class="sxs-lookup"><span data-stu-id="bb9ec-123">Example (upload a new file)</span></span>

<span data-ttu-id="bb9ec-124">В этом примере показано, как отправить строку "The contents of the file goes here." (Здесь начинается содержимое файла.)</span><span class="sxs-lookup"><span data-stu-id="bb9ec-124">This example uploads the string "The contents of the file goes here."</span></span> <span data-ttu-id="bb9ec-125">в файл FileB.txt в папке FolderA на диске пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="bb9ec-125">to a file in the signed-in user's drive under FolderA named FileB.txt.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="bb9ec-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb9ec-126">Response</span></span>

<span data-ttu-id="bb9ec-127">При успешном выполнении этот метод возвращает ресурс [driveItem][item-resource] для созданного файла в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bb9ec-127">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```

## <a name="example-updating-an-existing-file"></a><span data-ttu-id="bb9ec-128">Пример (обновление существующего файла)</span><span class="sxs-lookup"><span data-stu-id="bb9ec-128">Example (updating an existing file)</span></span>

<span data-ttu-id="bb9ec-129">В этом примере показано, как заменить содержимое файла с известным идентификатором.</span><span class="sxs-lookup"><span data-stu-id="bb9ec-129">This example replaces the contents of a file with a known ID.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="bb9ec-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb9ec-130">Response</span></span>

<span data-ttu-id="bb9ec-131">При успешном выполнении этот метод возвращает ресурс [driveItem][item-resource] для созданного файла в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bb9ec-131">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bb9ec-132">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="bb9ec-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bb9ec-133">C#</span><span class="sxs-lookup"><span data-stu-id="bb9ec-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/upload-via-put-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb9ec-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb9ec-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/upload-via-put-id-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="error-responses"></a><span data-ttu-id="bb9ec-135">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="bb9ec-135">Error responses</span></span>

<span data-ttu-id="bb9ec-136">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="bb9ec-136">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitem-put-content.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-put-content.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
