---
title: тип ресурса printerShare
description: Представляет принтер, который предназначен для обнаружения пользователями и приложениями печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: fdd0cccd4be8e65718a118cbd7b0b344dc74c05c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518073"
---
# <a name="printershare-resource-type"></a>тип ресурса printerShare

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет принтер, который предназначен для обнаружения пользователями и приложениями печати.

Наследует от [printerBase](../resources/printerbase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Список](../api/print-list-shares.md) | [коллекция printerShare](printershare.md) | Получите список акций принтера в клиенте. |
| [получение](../api/printershare-get.md); | [printerShare](printershare.md) | Чтение свойств и связей объекта **printerShare.** |
| [обновление](../api/printershare-update.md). | [printerShare](printershare.md) | Обновление **объекта printerShare.** |
| [удаление](../api/printershare-delete.md); | Нет | Размыть принтер. |
| [Список заданий](../api/printershare-list-jobs.md) | [коллекция printJob](printjob.md) | Получите список заданий печати, которые стоят в очереди для обработки принтеромShare. |
| [Создание задания](../api/printershare-post-jobs.md) | [printJob](printjob.md) | Создайте новое задание печати для принтераShare. Чтобы приступить к печати задания, используйте [start](../api/printjob-start.md). |
| [Список allowedUsers](../api/printershare-list-allowedusers.md) | Коллекция объектов [user](user.md) | Извлечение списка пользователей, которым был предоставлен доступ для отправки заданий печати в связанную долю принтера. |
| [Добавление allowedUser](../api/printershare-post-allowedusers.md) | Нет | Предоставление указанному пользователю доступа к отправке заданий печати в связанную долю принтера. |
| [Удаление allowedUser](../api/printershare-delete-alloweduser.md) | Нет | Отзовет доступ принтера к совместному доступу указанному пользователю. |
| [Список allowedGroups](../api/printershare-list-allowedgroups.md) | Коллекция [group](group.md) | Извлечение списка групп, которые получили доступ для отправки заданий печати в связанную долю принтера. |
| [Добавление allowedGroup](../api/printershare-post-allowedgroups.md) | Нет | Предоставление указанной группе доступа для отправки заданий печати в связанную долю принтера. |
| [Удаление allowedGroup](../api/printershare-delete-allowedgroup.md) | Нет | Отзовет доступ к принтеру для обмена данными из указанной группы. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка| Идентификатор printerShare. Унаследованный от [printerBase](../resources/printerbase.md). Только для чтения.|
|displayName|Строка|Имя доли принтера, которую должны отображать клиенты печати. Унаследованный от [printerBase](../resources/printerbase.md).|
|createdDateTime|DateTimeOffset|DateTimeOffset, когда была создана доля принтера. Только для чтения.|
|manufacturer|String|Производитель сообщил на принтере, связанном с этой долей принтера. Унаследованный от [printerBase](../resources/printerbase.md). Только для чтения.|
|model|String|Имя модели, которое сообщается на принтере, связанном с этим разделом принтера. Унаследованный от [printerBase](../resources/printerbase.md). Только для чтения.|
|isAcceptingJobs|Логический|Принимает ли принтер, связанный с этой долей принтера, новые задания печати. Унаследованный от [printerBase](../resources/printerbase.md).|
|defaults|[printerDefaults](printerdefaults.md)|Параметры печати принтера по умолчанию, связанные с этим разделом принтера. Унаследованный от [printerBase](../resources/printerbase.md).|
|capabilities|[printerCapabilities](printercapabilities.md)|Возможности принтера, связанного с этим разделом принтера. Унаследованный от [printerBase](../resources/printerbase.md).|
|location|[printerLocation](printerlocation.md)|Физическое и/или организационное расположение принтера, связанного с этим разделом принтера. Унаследованный от [printerBase](../resources/printerbase.md).|
|status|[printerStatus](printerstatus.md)|Состояние обработки, включая все ошибки, принтера, связанного с этим разделом принтера. Унаследованный от [printerBase](../resources/printerbase.md). Только для чтения.|
|allowAllUsers|Логический|Если это так, всем пользователям и группам будет предоставлен доступ к этой совместной печати. Это замещеет списки разрешенных объектов, определенные **свойствами allowedUsers** и **allowedGroups.**|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|printer|[printer](printer.md)|Принтер, с который связан этот принтер. |
|allowedUsers|Коллекция объектов [user](user.md)|Пользователи, которые имеют доступ к печати с помощью принтера.|
|allowedGroups|[group](group.md)|Группы, пользователи которых имеют доступ к печати с помощью принтера.|
|jobs|[коллекция printJob](printjob.md)| Список заданий, которые выстроились в очередь для печати на принтере, связанном с этой долей принтера.|
## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerShare",
  "baseType": "microsoft.graph.printerBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerShare",
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isAcceptingJobs": "Boolean",
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults"
  },
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "capabilities": {
    "@odata.type": "microsoft.graph.printerCapabilities"
  },
  "status": {
    "@odata.type": "microsoft.graph.printerStatus"
  },
  "allowAllUsers": "Boolean",
  "createdDateTime": "String (timestamp)"
}
```

