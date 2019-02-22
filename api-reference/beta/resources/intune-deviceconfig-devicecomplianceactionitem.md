---
title: Тип ресурса deviceComplianceActionItem
description: Конфигурация запланированного действия
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f1aa0ae42243fd1dbe44484f7bdbb4c226d7b15
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150514"
---
# <a name="devicecomplianceactionitem-resource-type"></a>Тип ресурса deviceComplianceActionItem

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация запланированного действия

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceComplianceActionItem](../api/intune-deviceconfig-devicecomplianceactionitem-list.md)|Коллекция [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|Список свойств и связей объектов [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).|
|[Получение объекта deviceComplianceActionItem](../api/intune-deviceconfig-devicecomplianceactionitem-get.md)|[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md);|Чтение свойств и связей объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).|
|[Создание объекта deviceComplianceActionItem](../api/intune-deviceconfig-devicecomplianceactionitem-create.md)|[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md);|Создание объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).|
|[Удаление объекта deviceComplianceActionItem](../api/intune-deviceconfig-devicecomplianceactionitem-delete.md)|Нет|Удаляет объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).|
|[Обновление объекта deviceComplianceActionItem](../api/intune-deviceconfig-devicecomplianceactionitem-update.md)|[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|Обновление свойств объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|gracePeriodHours|Int32|Время ожидания (в часах) до применения действия. Допустимые значения: от 0 до 8760.|
|actionType|[deviceComplianceActionType](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|Действия, которые необходимо выполнить. Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.|
|notificationTemplateId|String|Используемый шаблон сообщения уведомления|
|notificationMessageCCList|Коллекция строк|Список идентификаторов групп, которым будет отправлена копия этого сообщения уведомления.|

## <a name="relationships"></a>Связи
None

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceActionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "String (identifier)",
  "gracePeriodHours": 1024,
  "actionType": "String",
  "notificationTemplateId": "String",
  "notificationMessageCCList": [
    "String"
  ]
}
```




