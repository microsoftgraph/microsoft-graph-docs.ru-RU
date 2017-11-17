---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "Отправка небольших файлов"
ms.openlocfilehash: 44d3d3033014067af968720d24e87ec5047416ae
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="95918-102">Отправка или замена содержимого элемента DriveItem</span><span class="sxs-lookup"><span data-stu-id="95918-102">Upload or replace the contents of a driveItem</span></span>

<span data-ttu-id="95918-p101">Используя простой API отправки, вы можете отправлять содержимое нового файла или обновлять содержимое существующего файла с помощью одного вызова API. Этот метод поддерживает файлы размером не более 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="95918-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="95918-105">Сведения о том, как отправлять большие файлы, см. в разделе [Отправка больших файлов с помощью сеанса отправки](driveitem_createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="95918-105">To upload large files see [Upload large files with an upload session](driveitem_createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="95918-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95918-106">Permissions</span></span>

<span data-ttu-id="95918-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="95918-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="95918-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95918-109">Permission type</span></span>      | <span data-ttu-id="95918-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95918-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95918-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95918-111">Delegated (work or school account)</span></span> | <span data-ttu-id="95918-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95918-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="95918-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95918-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95918-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95918-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="95918-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95918-115">Application</span></span> | <span data-ttu-id="95918-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95918-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request-to-replace-an-existing-item"></a><span data-ttu-id="95918-117">HTTP-запрос (для замены существующего элемента)</span><span class="sxs-lookup"><span data-stu-id="95918-117">HTTP request (to replace an existing item)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a><span data-ttu-id="95918-118">HTTP-запрос (для отправки нового файла)</span><span class="sxs-lookup"><span data-stu-id="95918-118">HTTP request (to upload a new file)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a><span data-ttu-id="95918-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="95918-119">Request body</span></span>

<span data-ttu-id="95918-120">Содержимое текста запроса должно представлять собой двоичный поток файла, который необходимо отправить.</span><span class="sxs-lookup"><span data-stu-id="95918-120">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="95918-121">Ответ</span><span class="sxs-lookup"><span data-stu-id="95918-121">Response</span></span>

<span data-ttu-id="95918-122">При успешном выполнении этот метод возвращает объект [driveItem](../resources/driveitem.md) для вновь созданного или обновленного файла в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="95918-122">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created file.</span></span>

## <a name="example-upload-a-new-file"></a><span data-ttu-id="95918-123">Пример (отправка нового файла)</span><span class="sxs-lookup"><span data-stu-id="95918-123">Example (upload a new file)</span></span>

<span data-ttu-id="95918-124">В этом примере показано, как отправить строку "The contents of the file goes here." (Здесь начинается содержимое файла.)</span><span class="sxs-lookup"><span data-stu-id="95918-124">This example uploads the string "The contents of the file goes here."</span></span> <span data-ttu-id="95918-125">в файл FileB.txt в папке FolderA на диске пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="95918-125">to a file in the signed-in user's drive under FolderA named FileB.txt.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="95918-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="95918-126">Response</span></span>

<span data-ttu-id="95918-127">При успешном выполнении этот метод возвращает ресурс [driveItem][item-resource] для созданного файла в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="95918-127">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="example-updating-an-existing-file"></a><span data-ttu-id="95918-128">Пример (обновление существующего файла)</span><span class="sxs-lookup"><span data-stu-id="95918-128">Example (updating an existing file)</span></span>

<span data-ttu-id="95918-129">В этом примере показано, как заменить содержимое файла с известным идентификатором.</span><span class="sxs-lookup"><span data-stu-id="95918-129">This example replaces the contents of a file with a known ID.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="95918-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="95918-130">Response</span></span>

<span data-ttu-id="95918-131">При успешном выполнении этот метод возвращает ресурс [driveItem][item-resource] для созданного файла в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="95918-131">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="95918-132">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="95918-132">Error responses</span></span>

<span data-ttu-id="95918-133">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="95918-133">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation"
} -->
