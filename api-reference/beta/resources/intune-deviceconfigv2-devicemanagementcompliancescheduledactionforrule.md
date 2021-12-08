---
title: тип ресурса deviceManagementComplianceScheduledActionForRule
description: Запланированное действие для правила
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8b5f5d652119f7a47e7543c82840d259174c3e59
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342811"
---
# <a name="devicemanagementcompliancescheduledactionforrule-resource-type"></a>тип ресурса deviceManagementComplianceScheduledActionForRule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Запланированное действие для правила

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementComplianceScheduledActionForRules](../api/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule-list.md)|[коллекция deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|Список свойств и связей [объектов deviceManagementComplianceScheduledActionForRule.](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|
|[Get deviceManagementComplianceScheduledActionForRule](../api/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule-get.md)|[deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|Чтение свойств и связей [объекта deviceManagementComplianceScheduledActionForRule.](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|
|[Создание deviceManagementComplianceScheduledActionForRule](../api/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule-create.md)|[deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|Создание нового [объекта deviceManagementComplianceScheduledActionForRule.](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|
|[Удаление deviceManagementComplianceScheduledActionForRule](../api/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule-delete.md)|Нет|Удаляет [устройствоManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md).|
|[Обновление deviceManagementComplianceScheduledActionForRule](../api/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule-update.md)|[deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|Обновление свойств объекта [deviceManagementComplianceScheduledActionForRule.](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ этого параметра в политике, содержа которой он содержится. Автоматически созданный.|
|ruleName|String|Имя правила, к которому применяется это запланированное действие.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|scheduledActionConfigurations|[коллекция deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|Список конфигураций запланированных действий для этой политики соответствия требованиям. Эта коллекция может содержать не более 100 элементов.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementComplianceScheduledActionForRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementComplianceScheduledActionForRule",
  "id": "String (identifier)",
  "ruleName": "String"
}
```




