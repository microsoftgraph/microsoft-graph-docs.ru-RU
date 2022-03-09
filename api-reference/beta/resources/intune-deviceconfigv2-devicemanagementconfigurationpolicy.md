---
title: тип ресурса deviceManagementConfigurationPolicy
description: Политика конфигурации управления устройствами
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d768f8986d80a407fb2496fdde31bf2e65194336
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367610"
---
# <a name="devicemanagementconfigurationpolicy-resource-type"></a>тип ресурса deviceManagementConfigurationPolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика конфигурации управления устройствами

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementConfigurationPolicies](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-list.md)|[коллекция deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|Список свойств и связей [объектов deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) .|
|[Get deviceManagementConfigurationPolicy](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-get.md)|[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|Чтение свойств и связей [объекта deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) .|
|[Создание deviceManagementConfigurationPolicy](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-create.md)|[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|Создание нового [объекта deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) .|
|[Удаление deviceManagementConfigurationPolicy](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-delete.md)|Нет|Удаляет [устройствоManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md).|
|[Обновление deviceManagementConfigurationPolicy](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-update.md)|[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|Обновление свойств объекта [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) .|
|[Действие assign](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-assign.md)|[коллекция deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Пока не задокументировано.|
|[действие createCopy](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-createcopy.md)|[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ документа политики. Автоматически созданный.|
|name|String|Имя политики|
|description|Строка|Описание политики|
|платформы|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Платформы для этой политики. Возможные значения: `none`, `android`, `iOS`, `macOS`, `windows10X`, `windows10`, `linux`, `unknownFutureValue`.|
|технологии|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Технологии для этой политики. Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`, `exchangeOnline`, `linuxMdm`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|Дата и время создания политики|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения политики|
|settingCount|Int32|Количество параметров|
|creationSource|Строка|Источник создания политики|
|roleScopeTagIds|Коллекция строк|Список тегов области для этого экземпляра Entity.|
|isAssigned|Boolean|Состояние назначения политики. Это свойство доступно только для чтения.|
|templateReference|[deviceManagementConfigurationPolicyTemplateReference](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplatereference.md)|Справочные сведения по шаблонам|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|settings|[коллекция deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)|Параметры политики|
|assignments|[коллекция deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Назначения политик|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
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
  "isAssigned": true,
  "templateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
    "templateId": "String",
    "templateFamily": "String",
    "templateDisplayName": "String",
    "templateDisplayVersion": "String"
  }
}
```




