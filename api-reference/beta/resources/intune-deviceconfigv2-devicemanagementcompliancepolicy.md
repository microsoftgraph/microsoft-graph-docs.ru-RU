---
title: тип ресурса deviceManagementCompliancePolicy
description: Политика соответствия требованиям к управлению устройствами
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 782d3de50a873e0bae994d54bebc2186c4ac06e3
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62290828"
---
# <a name="devicemanagementcompliancepolicy-resource-type"></a>тип ресурса deviceManagementCompliancePolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика соответствия требованиям к управлению устройствами

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementCompliancePolicies](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-list.md)|[коллекция deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)|Список свойств и связей объектов [deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) .|
|[Get deviceManagementCompliancePolicy](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-get.md)|[deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)|Чтение свойств и связей [объекта deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) .|
|[Создание deviceManagementCompliancePolicy](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-create.md)|[deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)|Создание нового [объекта deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) .|
|[Удаление deviceManagementCompliancePolicy](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-delete.md)|Нет|Удаляет [устройствоManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md).|
|[Обновление deviceManagementCompliancePolicy](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-update.md)|[deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)|Обновление свойств объекта [deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) .|
|[Действие assign](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-assign.md)|[коллекция deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Пока не задокументировано.|
|[действие setScheduledActions](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-setscheduledactions.md)|[коллекция deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ документа политики. Автоматически созданный.|
|name|String|Имя политики|
|description|String|Описание политики|
|платформы|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Платформы для этой политики. Возможные значения: `none`, `android`, `iOS`, `macOS`, `windows10X`, `windows10`, `linux`, `unknownFutureValue`.|
|технологии|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Технологии для этой политики. Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`, `exchangeOnline`, `linuxMdm`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Политика последней даты и времени изменения. Это свойство доступно только для чтения.|
|settingCount|Int32|Количество параметров. Это свойство доступно только для чтения.|
|creationSource|String|Источник создания политики|
|roleScopeTagIds|Коллекция строк|Список тегов области для этого экземпляра Entity.|
|isAssigned|Boolean|Состояние назначения политики. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|settings|[коллекция deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)|Параметры политики|
|assignments|[коллекция deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Назначения политик|
|scheduledActionsForRule|[коллекция deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|Список запланированных действий для этого правила.|

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




