---
title: Тип ресурса deviceManagementConfigurationPolicyTemplate
description: Управление устройствами политики конфигурации
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 75cde2337e2e210b91afefede54eafae7fa8ed0f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211587"
---
# <a name="devicemanagementconfigurationpolicytemplate-resource-type"></a>Тип ресурса deviceManagementConfigurationPolicyTemplate

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Управление устройствами политики конфигурации

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление deviceManagementConfigurationPolicyTemplates](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-list.md)|[Коллекция deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|Список свойств и связей объектов [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) .|
|[Получение объекта deviceManagementConfigurationPolicyTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-get.md)|[deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|Чтение свойств и связей объекта [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) .|
|[Создание объекта deviceManagementConfigurationPolicyTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-create.md)|[deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|Создайте объект [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) .|
|[Удаление объекта deviceManagementConfigurationPolicyTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-delete.md)|Нет|Удаляет [объект deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md).|
|[Обновление объекта deviceManagementConfigurationPolicyTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate-update.md)|[deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)|Обновление свойств объекта [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ документа шаблона, состоящий из BaseId и Version. Создается автоматически.|
|BaseId|Строка|Базовый идентификатор шаблона|
|version|Int32|Версия шаблона. Допустимые значения от 1 до 2147483647. Это свойство доступно только для чтения.|
|displayName|Строка|Отображаемое имя шаблона|
|description|Строка|Описание шаблона|
|displayVersion|Строка|Описание версии шаблона|
|lifecycleState|[deviceManagementTemplateLifecycleState](../resources/intune-deviceconfigv2-devicemanagementtemplatelifecyclestate.md)|Укажите текущее состояние жизненного цикла шаблона. Возможные значения: `invalid`, `draft`, `active`, `superseded`, `deprecated`, `retired`.|
|Платформ|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Платформы для этого шаблона. Возможные значения: `none`, `android`, `iOS`, `macOS`, `windows10X`, `windows10`, `linux`, `unknownFutureValue`.|
|Технологии|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Технологии для этого шаблона. Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`, `appleRemoteManagement`, `microsoftSense`, `exchangeOnline`, `linuxMdm`, `unknownFutureValue`.|
|templateFamily|[deviceManagementConfigurationTemplateFamily](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|TemplateFamily для этого шаблона. Возможные значения: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`, `baseline`.|
|allowUnmanagedSettings|Логический|Разрешить неуправляемые шаблоны параметров|
|settingTemplateCount|Int32|Количество шаблонов параметров. Допустимые значения от 0 до 2147483647. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|settingTemplates|[Коллекция deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|Настройка шаблонов|

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




