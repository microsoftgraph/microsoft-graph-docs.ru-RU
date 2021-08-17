---
title: тип ресурса deviceManagementConfigurationPolicy
description: Политика конфигурации управления устройствами
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 318cd01000b2f1302c55b696883cf3e0b6e3cf1d3bcc64e36c4a484b94de10c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54139455"
---
# <a name="devicemanagementconfigurationpolicy-resource-type"></a>тип ресурса deviceManagementConfigurationPolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика конфигурации управления устройствами

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementConfigurationPolicies](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-list.md)|[коллекция deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|Список свойств и связей [объектов deviceManagementConfigurationPolicy.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|
|[Get deviceManagementConfigurationPolicy](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-get.md)|[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|Чтение свойств и связей [объекта deviceManagementConfigurationPolicy.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|
|[Создание deviceManagementConfigurationPolicy](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-create.md)|[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|Создание нового [объекта deviceManagementConfigurationPolicy.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|
|[Удаление deviceManagementConfigurationPolicy](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-delete.md)|Нет|Удаляет [устройствоManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md).|
|[Обновление deviceManagementConfigurationPolicy](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-update.md)|[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|Обновление свойств объекта [deviceManagementConfigurationPolicy.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|
|[Действие assign](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-assign.md)|[коллекция deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Пока не задокументировано.|
|[действие createCopy](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-createcopy.md)|[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ документа политики. Автоматически созданный.|
|name|String|Имя политики|
|description|Строка|Описание политики|
|платформы|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Платформы для этой политики. Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.|
|технологии|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Технологии для этой политики. Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Политика последней даты и времени изменения. Это свойство доступно только для чтения.|
|settingCount|Int32|Количество параметров. Это свойство доступно только для чтения.|
|creationSource|String|Источник создания политики|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity.|
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




