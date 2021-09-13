---
title: тип ресурса securityBaselineTemplate
description: Базовый шаблон безопасности учетной записи
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0e67c7c9d6bd3d25e8a59daeed2819787c4eb6c4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068997"
---
# <a name="securitybaselinetemplate-resource-type"></a>тип ресурса securityBaselineTemplate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый шаблон безопасности учетной записи


Наследует [от deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список securityBaselineTemplates](../api/intune-deviceintent-securitybaselinetemplate-list.md)|[коллекция securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|Список свойств и связей объектов [securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)|
|[Получить securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-get.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|Чтение свойств и связей объекта [securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)|
|[Создание securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-create.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|Создайте новый [объект securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)|
|[Удаление securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-delete.md)|Нет|Удаляет [securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)|
|[Обновление securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-update.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|Обновление свойств объекта [securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID шаблона, унаследованный от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|displayName|String|Имя отображения шаблона, унаследованный от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|description|String|Описание шаблона, унаследованный от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|versionInfo|String|Сведения о версии шаблона, унаследованные от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|isDeprecated|Boolean|Шаблон обесценив или нет. Намерения не могут быть созданы из шаблона с законтятой расшифровкой. Унаследованный от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|intentCount|Int32|Количество намерений, созданных из этого шаблона. Унаследованный от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|templateType|[deviceManagementTemplateType](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|Тип шаблона. Наследуется [от deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md). Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.|
|platformType|[policyPlatformType](../resources/intune-deviceintent-policyplatformtype.md)|Платформа шаблона. Наследуется [от deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md). Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.|
|templateSubtype|[deviceManagementTemplateSubtype](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|Подтип шаблона. Наследуется [от deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md). Возможные значения: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.|
|publishedDateTime|DateTimeOffset|При публикации шаблона наследуется [из deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|settings|[коллекция deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Коллекция всех параметров, которые этот шаблон унаследовал от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|categories|[коллекция deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Коллекция категорий параметров в шаблоне, унаследованной от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|migratableTo|[коллекция deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Коллекция шаблонов, которые этот шаблон может перенести на унаследованные из [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|deviceStateSummary|[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|Сводка состояния базового устройства безопасности|
|deviceStates|[коллекция securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Состояния базового устройства безопасности|
|categoryDeviceStateSummaries|[коллекция securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|Базовый уровень безопасности для состояния устройства категории|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "versionInfo": "String",
  "isDeprecated": true,
  "intentCount": 1024,
  "templateType": "String",
  "platformType": "String",
  "templateSubtype": "String",
  "publishedDateTime": "String (timestamp)"
}
```



