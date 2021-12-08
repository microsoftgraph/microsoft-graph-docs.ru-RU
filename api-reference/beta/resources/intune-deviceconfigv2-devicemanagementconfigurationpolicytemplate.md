---
title: тип ресурса deviceManagementConfigurationPolicyTemplate
description: Шаблон политики конфигурации управления устройствами
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d3472765c7c6ae7b6c3327f8e1e1b94b3680e2e6
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342813"
---
# <a name="devicemanagementconfigurationpolicytemplate-resource-type"></a>тип ресурса deviceManagementConfigurationPolicyTemplate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Шаблон политики конфигурации управления устройствами

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementConfigurationPolicyTemplates](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-list.md)|[коллекция deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|Список свойств и связей [объектов deviceManagementConfigurationPolicyTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|
|[Get deviceManagementConfigurationPolicyTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-get.md)|[deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|Чтение свойств и связей [объекта deviceManagementConfigurationPolicyTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|
|[Создание deviceManagementConfigurationPolicyTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-create.md)|[deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|Создание нового [объекта deviceManagementConfigurationPolicyTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|
|[Удаление deviceManagementConfigurationPolicyTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-delete.md)|Нет|Удаляет [устройствоManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md).|
|[Обновление deviceManagementConfigurationPolicyTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-update.md)|[deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|Обновление свойств объекта [deviceManagementConfigurationPolicyTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ документа шаблона, состоящего из BaseId и Version. Автоматически созданный.|
|baseId|String|Идентификатор базы шаблонов|
|version|Int32|Версия шаблона. Допустимые значения от 1 до 2147483647. Это свойство доступно только для чтения.|
|displayName|String|Имя отображения шаблона|
|description|Строка|Описание шаблона|
|displayVersion|Строка|Описание версии шаблона|
|lifecycleState|[deviceManagementTemplateLifecycleState](../resources/intune-deviceconfigv2-devicemanagementtemplatelifecyclestate.md)|Указать текущее состояние жизненного цикла шаблона. Возможные значения: `invalid`, `draft`, `active`, `superseded`, `deprecated`, `retired`.|
|платформы|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Платформы для этого шаблона. Возможные значения: `none`, `android`, `iOS`, `macOS`, `windows10X`, `windows10`.|
|технологии|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Технологии для этого шаблона. Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`, `exchangeOnline`, `linuxMdm`, `unknownFutureValue`.|
|templateFamily|[deviceManagementConfigurationTemplateFamily](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|TemplateFamily для этого шаблона. Возможные значения: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`, `baseline`.|
|allowUnmanagedSettings|Boolean|Разрешить неугодные шаблоны параметров|
|settingTemplateCount|Int32|Количество шаблонов параметров. Допустимые значения от 0 до 2147483647. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|settingTemplates|[коллекция deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|Настройка шаблонов|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplate",
  "id": "String (identifier)",
  "baseId": "String",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "displayVersion": "String",
  "lifecycleState": "String",
  "platforms": "String",
  "technologies": "String",
  "templateFamily": "String",
  "allowUnmanagedSettings": true,
  "settingTemplateCount": 1024
}
```




