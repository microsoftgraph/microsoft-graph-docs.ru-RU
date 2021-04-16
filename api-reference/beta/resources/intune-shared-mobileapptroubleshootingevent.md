---
title: тип ресурса mobileAppTroubleshootingEvent
description: Описывает ресурс mobileAppTroubleshootingEvent API Microsoft Graph для Intune, который поддерживает несколько процессов.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 387e21597c806e7aedf814128f809305999b19a6
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864958"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a>тип ресурса mobileAppTroubleshootingEvent

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

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
|id|String|UUID для объекта.|
|**Устранение неполадок**|
|additionalInformation|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Набор пар строк и пар значений строк, которые предоставляют дополнительные сведения о событии устранения неполадок, унаследованных от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|applicationId|String|Идентификатор приложения Intune.|
|correlationId|String|ID, используемый для отслеживания сбоя в службе. |
|eventDateTime|DateTimeOffset|Время возникновения события. |
|eventName|String|Имя события, соответствующее событию устранения неполадок. Необязательна|
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





