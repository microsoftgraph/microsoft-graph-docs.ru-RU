---
title: Работа с действиями, выполняющимися длительное время (бета-версия)
description: В этой статье описаны принципы работы с действиями, выполняющимися длительное время.
localization_priority: Normal
author: daspek
ms.openlocfilehash: 273299b13be423cf3e6ae625226efff5fef40f8f8ba06f787d0ba9ab29ba5211
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146239"
---
# <a name="working-with-long-running-actions-beta"></a>Работа с действиями, выполняющимися длительное время (бета-версия)


Для выполнения некоторых запросов API требуется неопределенное время.
Вместо того чтобы ожидать завершения действия перед возвращением ответа, Microsoft Graph может использовать шаблон действий, выполняющихся длительное время.
Этот шаблон предоставляет вашему приложению способ опроса обновлений состояния при длительном действии без ожидания выполнения действия.

В стандартном шаблоне выполняются следующие действия:

1. Ваше приложение запрашивает действие, выполняющееся длительное время, через API. API принимает действие и возвращает ответ `202 Accepted` вместе с заголовком Location для URL-адреса API, чтобы можно было получать отчеты о состоянии действия.
2. Ваше приложение запрашивает URL-адрес отчета о состоянии действия и получает ответ [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) со сведениями о ходе выполнения действия, выполняющегося длительное время.
3. Действие, выполняющееся длительное время, завершается. 
4. Приложение еще раз запрашивает URL-адрес отчета о состоянии действия и получает ответ [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta), в котором сообщается о завершении действия.

## <a name="initial-action-request"></a>Начальный запрос действия

Давайте по шагам рассмотрим пример сценария [копирования ресурса DriveItem](/graph/api/driveitem-copy?view=graph-rest-beta).
В этом сценарии приложение запрашивает операцию копирования папки, в которой содержится большое количество данных.
На выполнение этого запроса, вероятно, потребуется несколько секунд, так как необходимо передать большой объем данных.


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "lro-copy-item-example", "scopes": "files.readwrite" } -->

```http
POST https://graph.microsoft.com/beta/me/drive/items/{folder-item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "Copy of LargeFolder1"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/lro-copy-item-example-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/lro-copy-item-example-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/lro-copy-item-example-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


API отправляет ответ о том, что действие принято, и URL-адрес для получения сведений о состоянии действия, выполняющегося длительное время.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

**Примечание.** Возвращаемый URL-адрес расположения, возможно, не будет соответствовать конечной точке API Microsoft Graph.

Во многих случаях это может быть завершением запроса, так как действие копирования будет выполняться без каких-либо дополнительных действий со стороны приложения.
Тем не менее если вашему приложению необходимо отображать состояние действия копирования или убедиться, что действие выполнено без ошибок, приложение может сделать это, используя URL-адрес для отслеживания.

## <a name="retrieve-a-status-report-from-the-monitor-url"></a>Получение отчета о состоянии с URL-адреса для отслеживания

Чтобы проверить состояние действия копирования, приложение отправляет запрос на URL-адрес, указанный в предыдущем ответе. *Примечание.* Для этого запроса не нужно выполнять аутентификацию, так как этот URL-адрес действует в течение небольшого времени и является уникальным для исходного вызывающего объекта. 

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

Служба возвращает ответ со сведениями о том, что действие, выполняющееся длительное время, еще не завершено:

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
  "operation": "ItemCopy",
  "percentageComplete": 27.8,
  "status": "inProgress"
}
```

Эти сведения можно использовать для обновления информации о ходе копирования для пользователя. Приложение может опрашивать URL-адрес для отслеживания и получать обновленные сведения о ходе выполнения действия.

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a>Получение отчета о выполнении действия с URL-адреса для отслеживания

Через несколько секунд операция копирования завершается. На этот раз, когда приложение отправляет запрос на URL-для отслеживания, ответом будет перенаправление на результат выполненного действия.

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

По завершении действия в отклике службы отслеживания будет возвращен идентификатор ресурса для результатов.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "percentageComplete": 100.0,
    "resourceId": "01MOWKYVJML57KN2ANMBA3JZJS2MBGC7KM",
    "status": "completed"
}
```

## <a name="retrieve-the-results-of-the-completed-operation"></a>Получение результатов выполненной операции

После завершения задания URL-адрес для отслеживания возвращает идентификатор ресурса результата (в данном случае новую копию исходного элемента).
Вы можете обратиться к этому новому элементу с использованием идентификатора ресурса, например:


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "lro-copy-item-example-complete",
  "scopes": "files.readwrite"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/lro-copy-item-example-complete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/lro-copy-item-example-complete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/lro-copy-item-example-complete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "",
    "name": "Copy of LargeFolder1",
    "folder": { },
    "size": 12019
}
```

## <a name="supported-resources"></a>Поддерживаемые ресурсы

Действия, выполняющиеся длительное время, поддерживаются в указанных ниже методах API

| **Ресурс** | **API** |
|:------ | :------ |
| DriveItem | [Copy](/graph/api/driveitem-copy?view=graph-rest-beta) |

## <a name="prerequisites"></a>Необходимые компоненты

Для запроса сведений о состоянии действия, выполняющегося длительное время, необходимы такие же [разрешения](./permissions-reference.md), что и для самого действия, выполняющегося длительное время.




<!-- {
  "type": "#page.annotation",
  "description": "Monitor the progress of long-running actions in the API.",
  "keywords": "monitor,long,running,operation,action",
  "section": "documentation",
  "suppressions": [
    "Error: lro-check-status:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus",
    "Error: lro-check-status-complete:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus"
  ],
  "tocPath": "Concepts/Long running actions"
} -->
