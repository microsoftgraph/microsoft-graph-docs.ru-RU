---
title: Тип ресурса Дефаултдевицекомплианцеполици
description: Правила политики соответствия требованиям к устройствам по умолчанию, обеспечивающие ширину учетной записи.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0340b492f7efa9a4571c4f6c14d28ee72c4628da
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729772"
---
# <a name="defaultdevicecompliancepolicy-resource-type"></a>Тип ресурса Дефаултдевицекомплианцеполици

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Правила политики соответствия требованиям к устройствам по умолчанию, обеспечивающие ширину учетной записи.


Наследуется от [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список ДефаултдевицекомплианцеполиЦиес](../api/intune-deviceconfig-defaultdevicecompliancepolicy-list.md)|Коллекция [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)|Список свойств и связей объектов [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .|
|[Получение Дефаултдевицекомплианцеполици](../api/intune-deviceconfig-defaultdevicecompliancepolicy-get.md)|[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md);|Чтение свойств и связей объекта [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .|
|[Создание Дефаултдевицекомплианцеполици](../api/intune-deviceconfig-defaultdevicecompliancepolicy-create.md)|[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md);|Создание нового объекта [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .|
|[Удаление Дефаултдевицекомплианцеполици](../api/intune-deviceconfig-defaultdevicecompliancepolicy-delete.md)|Нет|Удаляет объект [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).|
|[Обновление Дефаултдевицекомплианцеполици](../api/intune-deviceconfig-defaultdevicecompliancepolicy-update.md)|[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md);|Обновление свойств объекта [дефаултдевицекомплианцеполици](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|scheduledActionsForRule|Коллекция [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|Список запланированных действий для этого правила. Наследуется от [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|deviceStatuses|Коллекция [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|Список DeviceComplianceDeviceStatus. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|userStatuses|Коллекция [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Список DeviceComplianceUserStatus. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|Обзор состояния обеспечения соответствия требованиям для устройств. Наследуется от [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|Обзор состояния обеспечения соответствия требованиям для устройств, указанного для пользователей. Наследуется от [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки обеспечения соответствия требованиям для устройств. Наследуется от [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|assignments|Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|Коллекция назначений для этой политики обеспечения соответствия требованиям. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultDeviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```





