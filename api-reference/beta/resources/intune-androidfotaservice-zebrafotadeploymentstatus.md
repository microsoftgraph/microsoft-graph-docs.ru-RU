---
title: Тип ресурса zebraFotaDeploymentStatus
description: Описывает состояние одного развертывания FOTA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bcc9c905c580b8d20d1bd43ed818e339aaa7ff93
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213566"
---
# <a name="zebrafotadeploymentstatus-resource-type"></a>Тип ресурса zebraFotaDeploymentStatus

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает состояние одного развертывания FOTA.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|state|[zebraFotaDeploymentState](../resources/intune-androidfotaservice-zebrafotadeploymentstate.md)|Возможные значения см. в перечислении zebraFotaDeploymentState. Возможные значения: `pendingCreation`, `createFailed`, `created`, `inProgress`, `completed`, `pendingCancel`, `canceled`, `unknownFutureValue`.|
|totalDevices|Int32|Целое число, указывающее общее количество устройств в развертывании.|
|totalCreated|Int32|Целое число, указывающее общее количество устройств с заданием в состоянии CREATED. Обычно указывает задания, которые не достигли устройств. |
|totalScheduled|Int32|Целое число, указывающее общее количество устройств, которые получили JSON и запланированы. |
|totalDownloading|Int32|Целое число, указывающее общее количество устройств, на которых установка прошла успешно.|
|totalАitingInstall|Int32|Целое число, указывающее общее количество устройств, на которых установка прошла успешно.|
|totalSucceededInstall|Int32|Целое число, указывающее общее количество устройств, на которых установка прошла успешно.|
|totalCanceled|Int32|Целое число, указывающее общее количество устройств, на которых была отменена установка.|
|totalUnknown|Int32|Целое число, указывающее общее количество устройств, на которых не получено состояние развертывания или конечное состояние, даже после запланированной даты окончания.|
|totalFailedDownload|Int32|Целое число, указывающее общее количество устройств, на которых не удалось скачать новый файл ОС.|
|totalFailedInstall|Int32|Целое число, указывающее общее количество устройств, на которых не удалось установить новый файл ОС.|
|completeOrCanceledDateTime|DateTimeOffset|Дата и время завершения или отмены развертывания. Фактическое время даты определяется значением состояния. Если состояние отменено, это свойство содержит дату и время отмены. Если состояние завершено, это свойство содержит дату и время завершения. Если развертывание не завершено до даты окончания развертывания, то дата и время завершения и дата и время завершения совпадают. Он всегда находится в часовом поясе развертывания. Примечание. Установка, которая выполняется, может продолжаться после даты окончания развертывания.|
|cancelRequested|Логическое|Логическое значение, указывающее, была ли запрошена отмена при развертывании. ПРИМЕЧАНИЕ. Запрос на отмену не гарантирует отмену развертывания.|
|lastUpdatedDateTime|DateTimeOffset| Дата и время обновления состояния развертывания из Zebra|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.zebraFotaDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.zebraFotaDeploymentStatus",
  "state": "String",
  "totalDevices": 1024,
  "totalCreated": 1024,
  "totalScheduled": 1024,
  "totalDownloading": 1024,
  "totalAwaitingInstall": 1024,
  "totalSucceededInstall": 1024,
  "totalCanceled": 1024,
  "totalUnknown": 1024,
  "totalFailedDownload": 1024,
  "totalFailedInstall": 1024,
  "completeOrCanceledDateTime": "String (timestamp)",
  "cancelRequested": true,
  "lastUpdatedDateTime": "String (timestamp)"
}
```




