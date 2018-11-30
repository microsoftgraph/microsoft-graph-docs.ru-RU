---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Отправка небольших файлов
ms.openlocfilehash: 8a31454e67b1d502721db83a38c733a5235cb8c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078214"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="cd86e-102">Отправка или замена содержимого элемента DriveItem</span><span class="sxs-lookup"><span data-stu-id="cd86e-102">Upload or replace the contents of a DriveItem</span></span>

> <span data-ttu-id="cd86e-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cd86e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd86e-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd86e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd86e-p102">Используя простой API отправки, вы можете отправлять содержимое нового файла или обновлять содержимое существующего файла с помощью одного вызова API. Этот метод поддерживает файлы размером не более 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="cd86e-p102">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="cd86e-107">Сведения о том, как отправлять большие файлы, см. в разделе [Отправка больших файлов с помощью сеанса отправки](driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="cd86e-107">To upload large files see [Upload large files with an upload session](driveitem-createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cd86e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd86e-108">Permissions</span></span>

<span data-ttu-id="cd86e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd86e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd86e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd86e-111">Permission type</span></span>      | <span data-ttu-id="cd86e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd86e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd86e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd86e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cd86e-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd86e-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cd86e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd86e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd86e-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd86e-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="cd86e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd86e-117">Application</span></span> | <span data-ttu-id="cd86e-118">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd86e-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request-to-replace-an-existing-item"></a><span data-ttu-id="cd86e-119">HTTP-запрос (для замены существующего элемента)</span><span class="sxs-lookup"><span data-stu-id="cd86e-119">HTTP request (to replace an existing item)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a><span data-ttu-id="cd86e-120">HTTP-запрос (для отправки нового файла)</span><span class="sxs-lookup"><span data-stu-id="cd86e-120">HTTP request (to upload a new file)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a><span data-ttu-id="cd86e-121">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cd86e-121">Request body</span></span>

<span data-ttu-id="cd86e-122">Содержимое текста запроса должно представлять собой двоичный поток файла, который необходимо отправить.</span><span class="sxs-lookup"><span data-stu-id="cd86e-122">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="cd86e-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd86e-123">Response</span></span>

<span data-ttu-id="cd86e-124">При успешном выполнении этот метод возвращает объект [driveItem](../resources/driveitem.md) в теле отклика для вновь созданного или обновленного файла.</span><span class="sxs-lookup"><span data-stu-id="cd86e-124">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created or updated file.</span></span>

## <a name="example-upload-a-new-file"></a><span data-ttu-id="cd86e-125">Пример (отправка нового файла)</span><span class="sxs-lookup"><span data-stu-id="cd86e-125">Example (upload a new file)</span></span>

<span data-ttu-id="cd86e-126">В этом примере показано, как отправить строку "The contents of the file goes here" (Здесь начинается содержимое файла.)</span><span class="sxs-lookup"><span data-stu-id="cd86e-126">This example uploads the string "The contents of the file goes here."</span></span> <span data-ttu-id="cd86e-127">в файл FileB.txt в папке FolderA в объекте drive пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="cd86e-127">to a file in the signed-in user's drive under FolderA named FileB.txt.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="cd86e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd86e-128">Response</span></span>

<span data-ttu-id="cd86e-129">При успешном выполнении этот метод возвращает ресурс [driveItem][item-resource] в теле отклика для созданного файла.</span><span class="sxs-lookup"><span data-stu-id="cd86e-129">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="example-updating-an-existing-file"></a><span data-ttu-id="cd86e-130">Пример (обновление существующего файла)</span><span class="sxs-lookup"><span data-stu-id="cd86e-130">Example (updating an existing file)</span></span>

<span data-ttu-id="cd86e-131">В этом примере показано, как заменить содержимое файла известным идентификатором.</span><span class="sxs-lookup"><span data-stu-id="cd86e-131">This example replaces the contents of a file with a known ID.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="cd86e-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd86e-132">Response</span></span>

<span data-ttu-id="cd86e-133">При успешном выполнении этот метод возвращает ресурс [driveItem][item-resource] для созданного файла в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cd86e-133">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="cd86e-134">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="cd86e-134">Error responses</span></span>

<span data-ttu-id="cd86e-135">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="cd86e-135">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation"
} -->
