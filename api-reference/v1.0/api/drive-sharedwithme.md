---
author: JeremyKelley
ms.date: 09/10/2017
title: Создание списка файлов, к которым мне предоставлен доступ
localization_priority: Priority
ms.prod: sharepoint
description: Получение коллекции ресурсов DriveItem, доступ к которым предоставлен владельцу ресурса Drive.
doc_type: apiPageType
ms.openlocfilehash: 77f2be110d57e77cc95eaa781fbe447563e6db72
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239837"
---
# <a name="list-items-shared-with-the-signed-in-user"></a>Создание списка элементов, к которым предоставлен доступ пользователю, выполнившему вход в систему

Пространство имен: microsoft.graph

Получение коллекции ресурсов [DriveItem](../resources/driveitem.md), к которым предоставлен общий доступ для владельца ресурса [Drive](../resources/drive.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Files.Read.All, Files.ReadWrite.All    |
|Для приложений | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

**Примечание.** Несмотря на то что при наличии разрешений Files.Read или Files.ReadWrite запрос /sharedWithMe будет успешно выполнен, могут отсутствовать некоторые свойства.
Кроме того, если отсутствует одно из разрешений **All**, общие элементы, возвращаемые этим API, будут недоступны.

## <a name="http-request"></a>HTTP-запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "shared-with-me", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```msgraph-interactive
GET /me/drive/sharedWithMe
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shared-with-me-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shared-with-me-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shared-with-me-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shared-with-me-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a>Отклик

Возвращает коллекцию ресурсов [DriveItem](../resources/driveitem.md), содержащую ресурсы DriveItem, к которым предоставлен общий доступ для владельца диска. В этом примере, так как указан диск по умолчанию пользователя, запрос возвращает элементы, к которым предоставлен общий доступ для пользователя, выполнившего вход.

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

## <a name="remarks"></a>Заметки

Элементы DriveItem, возвращенные действием **sharedWithMe**, будут всегда содержать аспект [**remoteItem**](../resources/remoteitem.md), который указывает, что это элементы с другого диска. Чтобы получить доступ к общему ресурсу DriveItem, следует отправить запрос, используя указанные в **remoteItem** данные, в следующем формате:

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

По умолчанию **sharedWithMe** возвращает элементы, к которым предоставлен общий доступ в вашем клиенте. Чтобы включить общие элементы из внешних клиентов, добавьте `?allowexternal=true` в запрос GET.



<!-- {
  "type": "#page.annotation",
  "description": "List the items shared with the owner of a drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Sharing/Shared with me",
  "suppressions": [
  ]
} -->

