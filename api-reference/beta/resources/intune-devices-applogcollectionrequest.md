---
title: тип ресурса appLogCollectionRequest
description: Объект AppLogCollectionRequest.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e2cd37ecd109720bf5a564c64d480037a9bd72fc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086311"
---
# <a name="applogcollectionrequest-resource-type"></a>тип ресурса appLogCollectionRequest

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект AppLogCollectionRequest.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список appLogCollectionRequests](../api/intune-devices-applogcollectionrequest-list.md)|[коллекция appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Список свойств и связей объектов [appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)|
|[Get appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-get.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Чтение свойств и связей объекта [appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)|
|[Создание appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-create.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Создайте новый [объект appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)|
|[Удаление appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-delete.md)|Нет|Удаляет [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).|
|[Обновление appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-update.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Обновление свойств объекта [appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)|
|[Действие createDownloadUrl](../api/intune-devices-applogcollectionrequest-createdownloadurl.md)|[appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор. Это userId_DeviceId_AppId id.|
|status|[appLogUploadState](../resources/intune-devices-apploguploadstate.md)|Состояние загрузки журнала. Возможные значения: `pending`, `completed`, `failed`.|
|errorMessage|String|Сообщение об ошибке, если таково сообщение во время процесса загрузки|
|customLogFolders|Коллекция объектов string|Список папок журнала. |
|completedDateTime|DateTimeOffset|Время, в течение которого запрос журнала загрузки достиг состояния терминала|

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



