---
title: Тип ресурса Мобилеапптраублешутинжевент
description: Описывает ресурс Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 89e7800fcd0e6bec5c8097937f87a92c6f1e9fa3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49300572"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a>Тип ресурса Мобилеапптраублешутинжевент

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Событие, представляющее состояние установки приложения для устройства "Пользователи" для управления устройствами и устранения неполадок обработки событий.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Мобилеапптраублешутинжевентс](../api/intune-shared-mobileapptroubleshootingevent-list.md)|Коллекция [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md)|Список свойств и связей объектов [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) .|
|[Получение Мобилеапптраублешутинжевент](../api/intune-shared-mobileapptroubleshootingevent-get.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md);|Чтение свойств и связей объекта [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) .|
|[Создание Мобилеапптраублешутинжевент](../api/intune-shared-mobileapptroubleshootingevent-create.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md);|Создание нового объекта [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) .|
|[Удаление Мобилеапптраублешутинжевент](../api/intune-shared-mobileapptroubleshootingevent-delete.md)|Нет|Удаляет объект [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md).|
|[Обновление Мобилеапптраублешутинжевент](../api/intune-shared-mobileapptroubleshootingevent-update.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md);|Обновление свойств объекта [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|UUID для объекта.|
|**Устранение неполадок**|
|аддитионалинформатион|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок, наследуемом от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|applicationId|String|Идентификатор приложения Intune.|
|correlationId|String|Идентификатор, используемый для трассировки сбоя в службе. |
|eventDateTime|DateTimeOffset|Время возникновения события. |
|eventName|String|Имя события, соответствующее событию устранения неполадок. Необязательный|
|лист|Коллекция [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|Элемент журнала устранения неполадок мобильных приложений Intune|
|managedDeviceIdentifier|String|Идентификатор события, созданный или полученный службой Intune.|
|траублешутинжеррордетаилс|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|Объект, содержащий подробные сведения об ошибке и ее исправлении. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|userId|String|Идентификатор пользователя, который пытался зарегистрировать устройство.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Управление устройствами**|
|апплогколлектионрекуестс|Коллекция [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Свойство Collection объекта Апплогуплоадрекуест.|


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





