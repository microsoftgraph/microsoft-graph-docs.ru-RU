---
title: Тип ресурса appLogCollectionRequest
description: Объект AppLogCollectionRequest.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b528f2ee74abf347b7ed31b323814197c8fa0bf
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805931"
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
|id|String|Уникальный идентификатор. Это идентификатор Усерид_девицеид_аппид.|
|status|[appLogUploadState](../resources/intune-devices-apploguploadstate.md)|Запись состояния отправки. Возможные значения: `pending`, `completed`, `failed`.|
|Ошибк|String|Сообщение об ошибке, если оно возникло во время процесса отправки|
|Кустомлогфолдерс|Коллекция String|Список папок журналов. |
|completedDateTime|DateTimeOffset|Время, когда запрос на отправку журнала достигает состояния терминала|

## <a name="relationships"></a>Отношения
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





