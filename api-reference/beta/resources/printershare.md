---
title: Тип ресурса Принтершаре
description: Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4fc729a41105340cc4066ee238c8d1ace3490765
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848233"
---
# <a name="printershare-resource-type"></a>Тип ресурса Принтершаре

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/print-list-shares.md) | Коллекция [принтершаре](printershare.md) | Получение списка общих принтеров в клиенте. |
| [получение](../api/printershare-get.md); | [принтершаре](printershare.md) | Чтение свойств и связей объекта **принтершаре** . |
| [обновление](../api/printershare-update.md). | [принтершаре](printershare.md) | Обновление объекта **принтершаре** . |
| [удаление](../api/printershare-delete.md); | Нет | Отменяет общий доступ к принтеру. |
| [Список заданий](../api/printershare-list-jobs.md) | Коллекция [printJob](printjob.md) | Получение списка заданий печати, помещенных в очередь для обработки с помощью Принтершаре. |
| [Создание задания](../api/printershare-post-jobs.md) | [printJob](printjob.md) | Создайте новое задание печати для Принтершаре. Чтобы начать печать задания, используйте [Start](../api/printjob-start.md). |
| [Список allowedUsers](../api/printershare-list-allowedusers.md) | Коллекция [принтусеридентити](printuseridentity.md) | Получение списка пользователей, которым предоставлен доступ к отправку заданий печати на связанный общий принтер. |
| [Добавление allowedUser](../api/printershare-post-allowedusers.md) | Нет | Предоставьте заданному пользователю доступ на отправку заданий печати в соответствующую общую папку принтера. |
| [Удаление allowedUser](../api/printershare-delete-alloweduser.md) | Нет | Отозвать доступ к общему принтеру для указанного пользователя. |
| [Список allowedGroups](../api/printershare-list-allowedgroups.md) | Коллекция [принтидентити](printidentity.md) | Получение списка групп, которым предоставлен доступ на отправку заданий печати на связанный общий принтер. |
| [Добавление allowedGroup](../api/printershare-post-allowedgroups.md) | Нет | Предоставление указанному групповому доступу на отправку заданий печати на связанный общий принтер. |
| [Удаление allowedGroup](../api/printershare-delete-allowedgroup.md) | Нет | Отзыв доступа к общему принтеру из указанной группы. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Идентификатор Принтершаре. Только для чтения.|
|displayName|String|Имя общего принтера, который должен отображаться клиентами печати.|
|createdDateTime|DateTimeOffset|Значение DateTimeOffset при создании общего ресурса принтера. Только для чтения.|
|manufacturer|String|Производитель, сообщаемый принтером, связанным с этим общим принтером. Только для чтения.|
|model|String|Имя модели, сообщаемое принтером, связанным с этим общим принтером. Только для чтения.|
|isAcceptingJobs|Логический|Принимает ли принтер, связанный с этим общим принтером, новые задания печати.|
|defaults|[принтердефаултс](printerdefaults.md)|Параметры печати по умолчанию для принтера, связанного с этим общим принтером.|
|capabilities|[принтеркапабилитиес](printercapabilities.md)|Возможности принтера, связанного с этим общим принтером.|
|location|[принтерлокатион](printerlocation.md)|Физическое и/или организационное расположение принтера, связанного с общим ресурсом принтера.|
|status|[принтерстатус](printerstatus.md)|Состояние обработки (включая ошибки) принтера, связанного с этим общим ресурсом принтера. Только для чтения.|
|алловаллусерс|Логический|Если этот параметр имеет значение true, всем пользователям и группам будет предоставлен доступ к этому общему ресурсу принтера. Этот параметр заменяет списки разрешений, определенные свойствами навигации **алловедусерс** и **алловедграупс** .|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|Printer|[Printer](printer.md)|Принтер, с которым связан этот общий принтер. |
|алловедусерс|Коллекция [принтусеридентити](printuseridentity.md)|Пользователи, у которых есть доступ к печати с помощью принтера.|
|алловедграупс|[принтидентити](printidentity.md)|Группы, у которых пользователи имеют доступ к печати с помощью принтера.|
|jobs|Коллекция [printJob](printjob.md)| Список заданий, помещенных в очередь для печати принтером, связанным с этим общим принтером.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerShare",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "createdDateTime": "String (timestamp)",
  "isAcceptingJobs": true,
  "allowAllUsers": false,
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"},
  "capabilities": {"@odata.type": "microsoft.graph.printerCapabilities"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerShare resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


