---
title: Тип ресурса deviceManagementCompliancePolicy
description: Управление устройствами соответствия требованиям
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c89d202aafea0d5245dcc33d88836f09a68eabe4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65208782"
---
# <a name="devicemanagementcompliancepolicy-resource-type"></a>Тип ресурса deviceManagementCompliancePolicy

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Управление устройствами соответствия требованиям

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов deviceManagementCompliancePolicies](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-list.md)|[Коллекция deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)|Список свойств и связей объектов [deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) .|
|[Получение объекта deviceManagementCompliancePolicy](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-get.md)|[deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)|Чтение свойств и связей объекта [deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) .|
|[Создание объекта deviceManagementCompliancePolicy](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-create.md)|[deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)|Создайте объект [deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) .|
|[Удаление объекта deviceManagementCompliancePolicy](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-delete.md)|Нет|Удаляет [объект deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md).|
|[Обновление объекта deviceManagementCompliancePolicy](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-update.md)|[deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)|Обновление свойств объекта [deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) .|
|[Действие assign](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-assign.md)|[Коллекция deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Пока не задокументировано.|
|[Действие setScheduledActions](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-setscheduledactions.md)|[Коллекция deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ документа политики. Создается автоматически.|
|name|String|Имя политики|
|description|Строка|Описание политики|
|Платформ|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Платформы для этой политики. Возможные значения: `none`, `android`, `iOS`, `macOS`, `windows10X`, `windows10`, `linux`, `unknownFutureValue`.|
|Технологии|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Технологии для этой политики. Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`, `appleRemoteManagement`, `microsoftSense`, `exchangeOnline`, `linuxMdm`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения политики. Это свойство доступно только для чтения.|
|settingCount|Int32|Количество параметров. Это свойство доступно только для чтения.|
|creationSource|Строка|Источник создания политики|
|Идентификаторы roleScopeTagId|Коллекция строк|Список тегов области для этого экземпляра сущности.|
|isAssigned|Boolean|Состояние назначения политики. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|settings|[Коллекция deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)|Параметры политики|
|assignments|[Коллекция deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Назначения политик|
|scheduledActionsForRule|[Коллекция deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|Список запланированных действий для этого правила.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCompliancePolicy",
  "id": "String (identifier)",
  "name": "String",
  "description": "String",
  "platforms": "String",
  "technologies": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "settingCount": 1024,
  "creationSource": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "isAssigned": true
}
```




