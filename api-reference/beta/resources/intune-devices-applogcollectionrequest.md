---
title: Тип ресурса appLogCollectionRequest
description: Объект AppLogCollectionRequest.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24d6ee782dc50935cffddc9916b04121bf3a1cb1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943202"
---
# <a name="applogcollectionrequest-resource-type"></a>Тип ресурса appLogCollectionRequest

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект AppLogCollectionRequest.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Апплогколлектионрекуестс](../api/intune-devices-applogcollectionrequest-list.md)|Коллекция [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Список свойств и связей объектов [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .|
|[Получение appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-get.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Чтение свойств и связей объекта [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .|
|[Создание appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-create.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Создание нового объекта [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .|
|[Удаление appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-delete.md)|Нет|Удаляет объект [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).|
|[Обновление appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-update.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Обновление свойств объекта [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .|
|[Действие createDownloadUrl](../api/intune-devices-applogcollectionrequest-createdownloadurl.md)|[appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор. Это идентификатор Усерид_девицеид_аппид.|
|status|[appLogUploadState](../resources/intune-devices-apploguploadstate.md)|Запись состояния отправки. Возможные значения: `pending`, `completed`, `failed`.|
|Ошибк|Строка|Сообщение об ошибке, если оно возникло во время процесса отправки|
|Кустомлогфолдерс|Коллекция строк|Список папок журналов. |
|completedDateTime|DateTimeOffset|Время, когда запрос на отправку журнала достигает состояния терминала|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appLogCollectionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "String (identifier)",
  "status": "String",
  "errorMessage": "String",
  "customLogFolders": [
    "String"
  ],
  "completedDateTime": "String (timestamp)"
}
```




