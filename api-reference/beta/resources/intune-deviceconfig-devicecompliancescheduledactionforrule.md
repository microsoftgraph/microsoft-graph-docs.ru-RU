---
title: Тип ресурса deviceComplianceScheduledActionForRule
description: Запланированное действие для правила
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30dbd1bd1114983e3077674273cc211c44c002a3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260336"
---
# <a name="devicecompliancescheduledactionforrule-resource-type"></a>Тип ресурса deviceComplianceScheduledActionForRule

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Запланированное действие для правила

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceComplianceScheduledActionForRule](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-list.md)|Коллекция [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|Список свойств и связей объектов [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).|
|[Получение объекта deviceComplianceScheduledActionForRule](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-get.md)|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|Чтение свойств и связей объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).|
|[Создание объекта deviceComplianceScheduledActionForRule](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-create.md)|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|Создание объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).|
|[Удаление объекта deviceComplianceScheduledActionForRule](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-delete.md)|Нет|Удаляет объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).|
|[Обновление объекта deviceComplianceScheduledActionForRule](../api/intune-deviceconfig-devicecompliancescheduledactionforrule-update.md)|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|Обновление свойств объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|ruleName|String|Имя правила, к которому применяется это запланированное действие.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|scheduledActionConfigurations|Коллекция [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md)|Список конфигураций запланированных действий для этой политики соответствия требованиям.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScheduledActionForRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "String (identifier)",
  "ruleName": "String"
}
```




