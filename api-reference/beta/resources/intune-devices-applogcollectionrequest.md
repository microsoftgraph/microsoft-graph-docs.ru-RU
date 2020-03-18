---
title: Тип ресурса appLogCollectionRequest
description: Объект AppLogCollectionRequest.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 29736e183237d284dfd7eddeff062607157fe212
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785149"
---
# <a name="applogcollectionrequest-resource-type"></a>Тип ресурса appLogCollectionRequest

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|String|Уникальный идентификатор. Это userId_DeviceId_AppId идентификатор.|
|status|[appLogUploadState](../resources/intune-devices-apploguploadstate.md)|Запись состояния отправки. Возможные значения: `pending`, `completed`, `failed`.|
|Ошибк|String|Сообщение об ошибке, если оно возникло во время процесса отправки|
|кустомлогфолдерс|Коллекция String|Список папок журналов. |
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



