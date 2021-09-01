---
title: тип ресурса deviceManagementTemplate
description: Сущность, представляюая определенный набор параметров устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e830e4d879b3cf3a096e9919ad75c0e3966dc21e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819012"
---
# <a name="devicemanagementtemplate-resource-type"></a>тип ресурса deviceManagementTemplate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляюая определенный набор параметров устройств

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementTemplates](../api/intune-deviceintent-devicemanagementtemplate-list.md)|[коллекция deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Список свойств и связей [объектов deviceManagementTemplate.](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|[Get deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Чтение свойств и связей [объекта deviceManagementTemplate.](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|[Создание deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Создание нового [объекта deviceManagementTemplate.](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|[Удаление deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|Нет|Удаляет [устройствоManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).|
|[Обновление deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Обновление свойств объекта [deviceManagementTemplate.](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|[Действие createInstance](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Пока не задокументировано.|
|[сравнение функции](../api/intune-deviceintent-devicemanagementtemplate-compare.md)|[коллекция deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md)|Пока не задокументировано.|
|[importOffice365DeviceConfigurationPolicies action](../api/intune-deviceintent-devicemanagementtemplate-importoffice365deviceconfigurationpolicies.md)|[коллекция deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID шаблона|
|displayName|String|Имя отображения шаблона|
|description|String|Описание шаблона|
|versionInfo|String|Сведения о версии шаблона|
|isDeprecated|Логический|Шаблон обесценив или нет. Намерения не могут быть созданы из шаблона с законтятой расшифровкой.|
|intentCount|Int32|Количество намерений, созданных из этого шаблона.|
|templateType|[deviceManagementTemplateType](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|Тип шаблона. Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.|
|platformType|[policyPlatformType](../resources/intune-deviceintent-policyplatformtype.md)|Платформа шаблона. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.|
|templateSubtype|[deviceManagementTemplateSubtype](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|Подтип шаблона. Возможные значения: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.|
|publishedDateTime|DateTimeOffset|После публикации шаблона|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|settings|[коллекция deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Коллекция всех параметров этого шаблона|
|categories|[коллекция deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Коллекция категорий параметров в шаблоне|
|migratableTo|[коллекция deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Коллекция шаблонов, которые этот шаблон может перенести в|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
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



