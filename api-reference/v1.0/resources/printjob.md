---
title: тип ресурса printJob
description: Представляет задание печати, которое выстроилось в очередь для принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 3115164fcc15ef6c2133ef3616624af9141da1af
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518068"
---
# <a name="printjob-resource-type"></a>тип ресурса printJob

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет задание печати, которое выстроилось в очередь для принтера.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/printjob-get.md); | [printJob](printjob.md) | Чтение свойств и связей объекта printJob. |
| [Создание](../api/printer-post-jobs.md) | [printJob](printjob.md) | Создание нового объекта задания печати. |
| [обновление](../api/printjob-update.md). | [printJob](printjob.md) | Обновление объекта задания печати. |
| [Начало](../api/printjob-start.md)|Нет|Запустите задание печати.|
| [Отмена](../api/printjob-cancel.md)|Нет|Отмена задания печати.|
| [Прервать](../api/printjob-abort.md)|Нет|Прервать задание печати.|
| [Перенаправление (на другой принтер)](../api/printjob-redirect.md) | [printJob](printjob.md) | Задание печати, которое находится в очереди для принтера назначения. |


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID принтера. Только для чтения.|
|createdDateTime|DateTimeOffset|DateTimeOffset, когда задание было создано. Только для чтения.|
|status|[printJobStatus](printjobstatus.md)|Состояние задания печати. Только для чтения.|
|configuration|[printJobConfiguration](printJobConfiguration.md)|Группа параметров, которые принтер должен использовать для печати задания.|
|isFetchable|Edm.Boolean|Если это так, документ можно получить на принтере.|
|redirectedFrom|Edm.String|Содержит URL-адрес задания источника, если задание было перенаправлено с другого принтера.|
|redirectedTo|Edm.String|Содержит URL-адрес задания назначения, если задание было перенаправлено на другой принтер.|
|createdBy|[userIdentity](useridentity.md)| Только для чтения. Допускается значение null.|

## <a name="relationships"></a>Отношения
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

