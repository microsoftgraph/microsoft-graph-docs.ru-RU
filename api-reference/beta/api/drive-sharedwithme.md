---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Создание списка файлов, к которым мне предоставлен доступ
localization_priority: Normal
ms.openlocfilehash: 9144c906a3f363ba10564dde36ca11c352a4fdcf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881510"
---
# <a name="list-items-shared-with-the-signed-in-user"></a><span data-ttu-id="2933a-102">Создание списка элементов, к которым предоставлен доступ пользователю, выполнившему вход в систему</span><span class="sxs-lookup"><span data-stu-id="2933a-102">List items shared with the signed-in user</span></span>

> <span data-ttu-id="2933a-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2933a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2933a-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2933a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2933a-105">Получение коллекции ресурсов [DriveItem](../resources/driveitem.md), к которым предоставлен общий доступ для владельца ресурса [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="2933a-105">Retrieve a collection of [DriveItem](../resources/driveitem.md) resources that have been shared with the owner of the [Drive](../resources/drive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2933a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2933a-106">Permissions</span></span>

<span data-ttu-id="2933a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2933a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2933a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2933a-109">Permission type</span></span>      | <span data-ttu-id="2933a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2933a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2933a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2933a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2933a-112">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2933a-112">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2933a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2933a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2933a-114">Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2933a-114">Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2933a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2933a-115">Application</span></span> | <span data-ttu-id="2933a-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2933a-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

<span data-ttu-id="2933a-117">**Примечание.** Несмотря на то что при наличии разрешений Files.Read или Files.ReadWrite запрос /sharedWithMe будет успешно выполнен, могут отсутствовать некоторые свойства.</span><span class="sxs-lookup"><span data-stu-id="2933a-117">**Note:** while the /sharedWithMe request will succeed with Files.Read or Files.ReadWrite permissions, some properties may be missing.</span></span>
<span data-ttu-id="2933a-118">Кроме того, если отсутствует одно из разрешений **All**, общие элементы, возвращаемые этим API, будут недоступны.</span><span class="sxs-lookup"><span data-stu-id="2933a-118">Additionally, without one of the  **All** permissions, shared items returned from this API will not be accessible.</span></span>

## <a name="http-request"></a><span data-ttu-id="2933a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2933a-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "shared-with-me", "scopes": "files.read", "target": "action" } -->

```http
GET /me/drive/sharedWithMe
```

## <a name="response"></a><span data-ttu-id="2933a-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="2933a-120">Response</span></span>

<span data-ttu-id="2933a-p104">Возвращает коллекцию ресурсов [DriveItem](../resources/driveitem.md), содержащую ресурсы DriveItem, к которым предоставлен общий доступ для владельца диска. В этом примере, так как указан диск по умолчанию пользователя, запрос возвращает элементы, к которым предоставлен общий доступ для пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="2933a-p104">This returns a collection of [DriveItem](../resources/driveitem.md) resources which contain the DriveItem resources shared with the owner of the drive. In this example, since the drive is the user's default drive, this returns items shared with the signed in user.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="2933a-123">Заметки</span><span class="sxs-lookup"><span data-stu-id="2933a-123">Remarks</span></span>

<span data-ttu-id="2933a-p105">Элементы DriveItem, возвращенные действием **sharedWithMe**, будут всегда содержать аспект [**remoteItem**](../resources/remoteitem.md), который указывает, что это элементы с другого диска. Чтобы получить доступ к общему ресурсу DriveItem, следует отправить запрос, используя указанные в **remoteItem** данные, в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="2933a-p105">DriveItems returned from the **sharedWithMe** action will always include the [**remoteItem**](../resources/remoteitem.md) facet which indicates they are items from a different drive. To access the shared DriveItem resource, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!-- {
  "type": "#page.annotation",
  "description": "List the items shared with the owner of a drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Sharing/Shared with me"
} -->
