---
title: Тип ресурса mobileAppTroubleshootingEvent
description: Событие, представляющее приложение устройства пользователей установить состояние.
ms.openlocfilehash: 8e8f45c2008600ebfb75b3207b4f3bb310ae072b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075138"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a>Тип ресурса mobileAppTroubleshootingEvent

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Событие, представляющее приложение устройства пользователей установить состояние.

Наследуется от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileAppTroubleshootingEvents](../api/intune-troubleshooting-mobileapptroubleshootingevent-list.md)|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) коллекции|Свойства списка и связей объектов [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .|
|[Получение mobileAppTroubleshootingEvent](../api/intune-troubleshooting-mobileapptroubleshootingevent-get.md)|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md);|Чтение свойства и связи объекта [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .|
|[Создание mobileAppTroubleshootingEvent](../api/intune-troubleshooting-mobileapptroubleshootingevent-create.md)|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md);|Создание нового объекта [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .|
|[Удаление mobileAppTroubleshootingEvent](../api/intune-troubleshooting-mobileapptroubleshootingevent-delete.md)|Нет|Удаляет [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md).|
|[Обновление mobileAppTroubleshootingEvent](../api/intune-troubleshooting-mobileapptroubleshootingevent-update.md)|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md);|Обновление свойства объекта [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|eventDateTime|DateTimeOffset|Время возникновения события. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|correlationId|String|Идентификатор, используемый для трассировки сбоя в службе. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|managedDeviceIdentifier|String|Идентификатор события, созданный или полученный службой Intune.|
|userId|String|Идентификатор пользователя, который пытался зарегистрировать устройство.|
|applicationId|String|Идентификатор приложения Intune.|
|журнал|[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) коллекции|Устранение неполадок в элемент журнала Intune мобильного приложения|

## <a name="relationships"></a>Связи
Нет
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





