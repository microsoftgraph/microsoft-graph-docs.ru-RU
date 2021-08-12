---
title: тип ресурса printJob
description: Представляет задание печати, которое выстроилось в очередь для принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 39c3ab6cbbf83773a28c5ce374322846e08fc43958eb0103640b080fa94b6e5a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237588"
---
# <a name="printjob-resource-type"></a>тип ресурса printJob

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет задание печати, которое выстроилось в очередь для принтера.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение](../api/printjob-get.md) | [printJob](printjob.md) | Чтение свойств и связей объекта printJob. |
| [Создание](../api/printer-post-jobs.md) | [printJob](printjob.md) | Создание нового объекта задания печати. |
| [Обновление](../api/printjob-update.md) | [printJob](printjob.md) | Обновление объекта задания печати. |
| [Start](../api/printjob-start.md)|Нет|Запустите задание печати.|
| [Cancel](../api/printjob-cancel.md)|Нет|Отмена задания печати.|
| [Прервать](../api/printjob-abort.md)|Нет|Прервать задание печати.|
| [Перенаправление (на другой принтер)](../api/printjob-redirect.md) | [printJob](printjob.md) | Задание печати, которое находится в очереди для принтера назначения. |


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID принтера. Только для чтения.|
|createdDateTime|DateTimeOffset|DateTimeOffset, когда задание было создано. Только для чтения.|
|status|[printJobStatus](printjobstatus.md)|Состояние задания печати. Только для чтения.|
|configuration|[printJobConfiguration](printJobConfiguration.md)|Группа параметров, которые принтер должен использовать для печати задания.|
|isFetchable|Edm.Boolean|Если это так, документ можно получить на принтере.|
|redirectedFrom|Edm.String|Содержит URL-адрес задания источника, если задание было перенаправлено с другого принтера.|
|redirectedTo|Edm.String|Содержит URL-адрес задания назначения, если задание было перенаправлено на другой принтер.|
|createdBy|[userIdentity](useridentity.md)| Только для чтения. Допускается значение null.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|документы|[коллекция printDocument](printdocument.md)| Только для чтения.|
|tasks|[printTask](printtask.md) collection|Список [printTasks,](printtask.md) которые были вызваны этим заданием печати.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printJob",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJob",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "status": {
    "@odata.type": "microsoft.graph.printJobStatus"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "configuration": {
    "@odata.type": "microsoft.graph.printJobConfiguration"
  },
  "redirectedTo": "String",
  "redirectedFrom": "String",
  "isFetchable": "Boolean"
}
```

