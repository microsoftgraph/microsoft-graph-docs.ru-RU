---
title: тип ресурса mobileAppTroubleshootingEvent
description: Описывает ресурс mobileAppTroubleshootingEvent API microsoft Graph intune, который поддерживает несколько процессов.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3614a0562c6c57b43f12396bb1661df04678ead2
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266921"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a>тип ресурса mobileAppTroubleshootingEvent

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Событие, представляющее состояние установки приложения-устройства пользователей для управления устройствами и устранения неполадок в процессах событий.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileAppTroubleshootingEvents](../api/intune-shared-mobileapptroubleshootingevent-list.md)|[коллекция mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|Список свойств и связей объектов [mobileAppTroubleshootingEvent.](../resources/intune-shared-mobileapptroubleshootingevent.md)|
|[Get mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-get.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md);|Чтение свойств и связей объекта [mobileAppTroubleshootingEvent.](../resources/intune-shared-mobileapptroubleshootingevent.md)|
|[Создание mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-create.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md);|Создание нового [объекта mobileAppTroubleshootingEvent.](../resources/intune-shared-mobileapptroubleshootingevent.md)|
|[Удаление mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-delete.md)|Нет|Удаляет [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).|
|[Обновление mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-update.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md);|Обновление свойств объекта [mobileAppTroubleshootingEvent.](../resources/intune-shared-mobileapptroubleshootingevent.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|UUID для объекта.|
|**Устранение неполадок**|
|additionalInformation|Коллекция [keyValuePair](../resources/intune-troubleshooting-keyvaluepair.md)|Набор пар строк и пар значений строк, которые предоставляют дополнительные сведения о событии устранения неполадок, унаследованных от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|applicationId|String|Идентификатор приложения Intune.|
|correlationId|String|ID, используемый для отслеживания сбоя в службе. |
|eventDateTime|DateTimeOffset|Время возникновения события. |
|eventName|Строка|Имя события, соответствующее событию устранения неполадок. При необходимости|
|история|[коллекция mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|Элемент истории устранения неполадок для мобильных приложений Intune|
|managedDeviceIdentifier|String|Идентификатор события, созданный или полученный службой Intune.|
|устранение неполадокErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|Объект, содержащий подробные сведения об ошибке и ее исправлении. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|userId|String|Идентификатор пользователя, который пытался зарегистрировать устройство.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Управление устройствами**|
|appLogCollectionRequests|[коллекция appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Свойство коллекции AppLogUploadRequest.|


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  },
  "eventName": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "applicationId": "String",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "String (timestamp)"
    }
  ]
}
```





