---
title: тип ресурса deviceManagementComplianceActionItem
description: Запланированное действие для правила
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 097ab8a552e4675570fc85139924615f32b8fd0d
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697471"
---
# <a name="devicemanagementcomplianceactionitem-resource-type"></a>тип ресурса deviceManagementComplianceActionItem

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Запланированное действие для правила

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementComplianceActionItems](../api/intune-deviceconfigv2-devicemanagementcomplianceactionitem-list.md)|[коллекция deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|Список свойств и связей объектов [deviceManagementComplianceActionItem.](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|
|[Get deviceManagementComplianceActionItem](../api/intune-deviceconfigv2-devicemanagementcomplianceactionitem-get.md)|[deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|Чтение свойств и связей [объекта deviceManagementComplianceActionItem.](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|
|[Создание deviceManagementComplianceActionItem](../api/intune-deviceconfigv2-devicemanagementcomplianceactionitem-create.md)|[deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|Создание нового [объекта deviceManagementComplianceActionItem.](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|
|[Удаление deviceManagementComplianceActionItem](../api/intune-deviceconfigv2-devicemanagementcomplianceactionitem-delete.md)|Нет|Удаляет [устройствоManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md).|
|[Обновление deviceManagementComplianceActionItem](../api/intune-deviceconfigv2-devicemanagementcomplianceactionitem-update.md)|[deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|Обновление свойств объекта [deviceManagementComplianceActionItem.](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ этого параметра в политике, содержа которой он содержится. Автоматически созданный.|
|gracePeriodHours|Int32|Время ожидания (в часах) до применения действия. Допустимые значения: от 0 до 8760|
|actionType|[deviceManagementComplianceActionType](../resources/intune-deviceconfigv2-devicemanagementcomplianceactiontype.md)|Какие действия необходимо принять. Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.|
|notificationTemplateId|String|Используемый шаблон сообщения уведомления|
|notificationMessageCCList|Коллекция String|Список идентификаторов групп, которым будет отправлена копия этого уведомления. Эта коллекция может содержать не более 100 элементов.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementComplianceActionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementComplianceActionItem",
  "id": "String (identifier)",
  "gracePeriodHours": 1024,
  "actionType": "String",
  "notificationTemplateId": "String",
  "notificationMessageCCList": [
    "String"
  ]
}
```



