---
author: JeremyKelley
description: Получение коллекции ресурсов DriveItem, доступ к которым предоставлен владельцу ресурса Drive.
ms.date: 09/10/2017
title: Создание списка файлов, к которым мне предоставлен доступ
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 933d8eae7566c3665f149f565d9055ef070033da
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955764"
---
# <a name="list-items-shared-with-the-signed-in-user"></a><span data-ttu-id="d1d10-103">Создание списка элементов, к которым предоставлен доступ пользователю, выполнившему вход в систему</span><span class="sxs-lookup"><span data-stu-id="d1d10-103">List items shared with the signed-in user</span></span>

<span data-ttu-id="d1d10-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1d10-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1d10-105">Получение коллекции ресурсов [DriveItem](../resources/driveitem.md), к которым предоставлен общий доступ для владельца ресурса [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="d1d10-105">Retrieve a collection of [DriveItem](../resources/driveitem.md) resources that have been shared with the owner of the [Drive](../resources/drive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d1d10-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1d10-106">Permissions</span></span>

<span data-ttu-id="d1d10-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1d10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1d10-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1d10-109">Permission type</span></span>      | <span data-ttu-id="d1d10-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1d10-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1d10-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1d10-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d1d10-112">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1d10-112">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d1d10-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1d10-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1d10-114">Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1d10-114">Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d1d10-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1d10-115">Application</span></span> | <span data-ttu-id="d1d10-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1d10-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

<span data-ttu-id="d1d10-117">**Примечание.** Несмотря на то что при наличии разрешений Files.Read или Files.ReadWrite запрос /sharedWithMe будет успешно выполнен, могут отсутствовать некоторые свойства.</span><span class="sxs-lookup"><span data-stu-id="d1d10-117">**Note:** while the /sharedWithMe request will succeed with Files.Read or Files.ReadWrite permissions, some properties may be missing.</span></span>
<span data-ttu-id="d1d10-118">Кроме того, если отсутствует одно из разрешений **All** , общие элементы, возвращаемые этим API, будут недоступны.</span><span class="sxs-lookup"><span data-stu-id="d1d10-118">Additionally, without one of the  **All** permissions, shared items returned from this API will not be accessible.</span></span>

## <a name="http-request"></a><span data-ttu-id="d1d10-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1d10-119">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="d1d10-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1d10-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "shared-with-me", "scopes": "files.read", "target": "action" } -->

```msgraph-interactive
GET /me/drive/sharedWithMe
```
# <a name="c"></a>[<span data-ttu-id="d1d10-121">C#</span><span class="sxs-lookup"><span data-stu-id="d1d10-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shared-with-me-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1d10-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1d10-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shared-with-me-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1d10-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1d10-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shared-with-me-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1d10-124">Java</span><span class="sxs-lookup"><span data-stu-id="d1d10-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shared-with-me-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="d1d10-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1d10-125">Response</span></span>

<span data-ttu-id="d1d10-p103">Возвращает коллекцию ресурсов [DriveItem](../resources/driveitem.md), содержащую ресурсы DriveItem, к которым предоставлен общий доступ для владельца диска. В этом примере, так как указан диск по умолчанию пользователя, запрос возвращает элементы, к которым предоставлен общий доступ для пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="d1d10-p103">This returns a collection of [DriveItem](../resources/driveitem.md) resources which contain the DriveItem resources shared with the owner of the drive. In this example, since the drive is the user's default drive, this returns items shared with the signed in user.</span></span>

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc",
      "remoteItem": {
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
      "id": "1312def",
      "remoteItem": {
        "id": "1991210caf!1991",
        "name": "Team Roster.xlsx",
        "file": { },
        "size": 37619,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="d1d10-128">Заметки</span><span class="sxs-lookup"><span data-stu-id="d1d10-128">Remarks</span></span>

<span data-ttu-id="d1d10-p104">Элементы DriveItem, возвращенные действием **sharedWithMe** , будут всегда содержать аспект [**remoteItem**](../resources/remoteitem.md), который указывает, что это элементы с другого диска. Чтобы получить доступ к общему ресурсу DriveItem, следует отправить запрос, используя указанные в **remoteItem** данные, в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="d1d10-p104">DriveItems returned from the **sharedWithMe** action will always include the [**remoteItem**](../resources/remoteitem.md) facet which indicates they are items from a different drive. To access the shared DriveItem resource, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```
<span data-ttu-id="d1d10-131">По умолчанию **шаредвисме** возвращает элементы, которые используются в вашем клиенте.</span><span class="sxs-lookup"><span data-stu-id="d1d10-131">By default, **sharedWithMe** returns items shared within your own tenant.</span></span> <span data-ttu-id="d1d10-132">Чтобы включить общие элементы из внешних клиентов, добавьте `?allowexternal=true` в запрос GET.</span><span class="sxs-lookup"><span data-stu-id="d1d10-132">To include items shared from external tenants, append `?allowexternal=true` to the GET request.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "List the items shared with the owner of a drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Sharing/Shared with me",
  "suppressions": [
  ]
}
-->


