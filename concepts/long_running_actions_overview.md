---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
ms.topic: conceptual
ms.openlocfilehash: 30f98afa7b75784b0ee2b9ec446c6389cc876949
ms.sourcegitcommit: af8fdd5ea762fb54b7fbebb9a70bd942a56c6b7a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2018
ms.locfileid: "19473155"
---
# <a name="working-with-long-running-actions-beta"></a>Работа с действиями, выполняющимися длительное время (бета-версия)

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Для выполнения некоторых запросов API требуется неопределенное время.
Вместо того чтобы ожидать завершения действия перед возвращением ответа, Microsoft Graph может использовать шаблон действий, выполняющихся длительное время.
При использовании этого шаблона вашему приложению предоставляется время для выполнения опроса об изменениях состояния для действия, выполняющегося длительное время, и запросу не нужно ожидать завершения действия.

В стандартном шаблоне выполняются следующие действия:

1. Ваше приложение запрашивает действие, выполняющееся длительное время, через API. API принимает действие и возвращает ответ `202 Accepted` вместе с заголовком Location для URL-адреса API, чтобы можно было получать отчеты о состоянии действия.
2. Ваше приложение запрашивает URL-адрес отчета о состоянии действия и получает ответ [AsyncJobStatus](../api-reference/beta/resources/asyncjobstatus.md) со сведениями о ходе выполнения действия, выполняющегося длительное время.
3. Действие, выполняющееся длительное время, завершается. 
4. Приложение еще раз запрашивает URL-адрес отчета о состоянии действия и получает ответ [AsyncJobStatus](../api-reference/beta/resources/asyncjobstatus.md), в котором сообщается о завершении действия.

## <a name="initial-action-request"></a>Начальный запрос действия

Давайте по шагам рассмотрим пример сценария [копирования ресурса DriveItem](../api-reference/beta/api/driveitem_copy.md).
В этом сценарии приложение запрашивает операцию копирования папки, в которой содержится большое количество данных.
На выполнение этого запроса, вероятно, потребуется несколько секунд, так как необходимо передать большой объем данных.

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

Чтобы проверить состояние действия копирования, приложение отправляет запрос на URL-адрес, указанный в предыдущем ответе.
*Примечание.* Для этого запроса не нужно выполнять аутентификацию, так как этот URL-адрес действует в течение небольшого времени и является уникальным для исходного вызывающего объекта. 

<!-- { "blockType": "request", "name": "lro-check-status", "scopes": "files.readwrite" } -->

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

Эти сведения можно использовать для обновления информации о ходе копирования для пользователя.
Приложение может продолжить опрашивать URL-адрес для отслеживания, чтобы получать обновленные сведения о ходе выполнения действия.

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a>Получение отчета о выполнении действия с URL-адреса для отслеживания

Через несколько секунд операция копирования завершается.
На этот раз, когда приложение отправляет запрос на URL-для отслеживания, ответом будет перенаправление на результат выполненного действия.

<!-- { "blockType": "request", "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

По завершении действия в ответе службы отслеживания будет возвращен идентификатор ресурса для результатов.

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

<!-- { "blockType": "request", "name": "lro-copy-item-example-complete", "scopes": "files.readwrite" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/01MOWKYVJML57KN2ANMBA3JZJS2MBGC7KM
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem" } -->

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
| DriveItem | [Copy](../api-reference/beta/api/driveitem_copy.md) |

## <a name="prerequisites"></a>Необходимые компоненты

Для запроса сведений о состоянии действия, выполняющегося длительное время, необходимы такие же [разрешения](./permissions_reference.md), что и для самого действия, выполняющегося длительное время.




<!-- {
  "type": "#page.annotation",
  "description": "Monitor the progress of long-running actions in the API.",
  "keywords": "monitor,long,running,operation,action",
  "section": "documentation",
  "tocPath": "Concepts/Long running actions"
} -->
