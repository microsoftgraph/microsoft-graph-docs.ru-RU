---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Отправка небольших файлов
localization_priority: Priority
ms.prod: sharepoint
description: 'API простой отправки позволяет отправить содержимое нового файла или обновить содержимое существующего файла с помощью одного вызова API. '
doc_type: apiPageType
ms.openlocfilehash: fbaa34ad2669a565f87074408dea49179063d878
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982042"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="f818e-103">Отправка или замена содержимого элемента DriveItem</span><span class="sxs-lookup"><span data-stu-id="f818e-103">Upload or replace the contents of a DriveItem</span></span>

<span data-ttu-id="f818e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f818e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f818e-p101">Используя простой API отправки, вы можете отправлять содержимое нового файла или обновлять содержимое существующего файла с помощью одного вызова API. Этот метод поддерживает файлы размером не более 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="f818e-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="f818e-107">Сведения о том, как отправлять большие файлы, см. в разделе [Отправка больших файлов с помощью сеанса отправки](driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="f818e-107">To upload large files see [Upload large files with an upload session](driveitem-createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f818e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f818e-108">Permissions</span></span>

<span data-ttu-id="f818e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f818e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f818e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f818e-111">Permission type</span></span>      | <span data-ttu-id="f818e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f818e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f818e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f818e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f818e-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f818e-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f818e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f818e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f818e-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f818e-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f818e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f818e-117">Application</span></span> | <span data-ttu-id="f818e-118">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f818e-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request-to-replace-an-existing-item"></a><span data-ttu-id="f818e-119">HTTP-запрос (для замены существующего элемента)</span><span class="sxs-lookup"><span data-stu-id="f818e-119">HTTP request (to replace an existing item)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a><span data-ttu-id="f818e-120">HTTP-запрос (для отправки нового файла)</span><span class="sxs-lookup"><span data-stu-id="f818e-120">HTTP request (to upload a new file)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a><span data-ttu-id="f818e-121">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f818e-121">Request body</span></span>

<span data-ttu-id="f818e-122">Содержимое текста запроса должно представлять собой двоичный поток файла, который необходимо отправить.</span><span class="sxs-lookup"><span data-stu-id="f818e-122">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="f818e-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="f818e-123">Response</span></span>

<span data-ttu-id="f818e-124">При успешном выполнении этот метод возвращает объект [driveItem](../resources/driveitem.md) для вновь созданного или обновленного файла в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f818e-124">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created or updated file.</span></span>

## <a name="example-upload-a-new-file"></a><span data-ttu-id="f818e-125">Пример (отправка нового файла)</span><span class="sxs-lookup"><span data-stu-id="f818e-125">Example (upload a new file)</span></span>

<span data-ttu-id="f818e-126">В этом примере показано, как отправить строку "The contents of the file goes here." (Здесь начинается содержимое файла.)</span><span class="sxs-lookup"><span data-stu-id="f818e-126">This example uploads the string "The contents of the file goes here."</span></span> <span data-ttu-id="f818e-127">в файл FileB.txt в папке FolderA на диске пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="f818e-127">to a file in the signed-in user's drive under FolderA named FileB.txt.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="f818e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f818e-128">Response</span></span>

<span data-ttu-id="f818e-129">В случае успешного выполнения этот метод возвращает в тексте отклика ресурс [driveItem][item-resource] для созданного файла.</span><span class="sxs-lookup"><span data-stu-id="f818e-129">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="example-updating-an-existing-file"></a><span data-ttu-id="f818e-130">Пример (обновление существующего файла)</span><span class="sxs-lookup"><span data-stu-id="f818e-130">Example (updating an existing file)</span></span>

<span data-ttu-id="f818e-131">В этом примере показано, как заменить содержимое файла с известным идентификатором.</span><span class="sxs-lookup"><span data-stu-id="f818e-131">This example replaces the contents of a file with a known ID.</span></span>


# <a name="http"></a>[<span data-ttu-id="f818e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f818e-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```
# <a name="c"></a>[<span data-ttu-id="f818e-133">C#</span><span class="sxs-lookup"><span data-stu-id="f818e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upload-via-put-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f818e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f818e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upload-via-put-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f818e-135">Java</span><span class="sxs-lookup"><span data-stu-id="f818e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/upload-via-put-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f818e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f818e-136">Response</span></span>

<span data-ttu-id="f818e-137">В случае успешного выполнения этот метод возвращает в тексте отклика ресурс [driveItem][item-resource] для созданного файла.</span><span class="sxs-lookup"><span data-stu-id="f818e-137">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="f818e-138">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="f818e-138">Error responses</span></span>

<span data-ttu-id="f818e-139">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="f818e-139">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation",
  "suppressions": [
  ]
} -->

