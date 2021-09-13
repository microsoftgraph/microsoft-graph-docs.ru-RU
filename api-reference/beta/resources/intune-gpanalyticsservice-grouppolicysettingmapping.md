---
title: тип ресурса groupPolicySettingMapping
description: Параметр Групповой политики для сопоставления MDM/Intune.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 90cacd1f89b75f1c6cf60fe64e9c9c141664423f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063904"
---
# <a name="grouppolicysettingmapping-resource-type"></a>тип ресурса groupPolicySettingMapping

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметр Групповой политики для сопоставления MDM/Intune.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicySettingMappings](../api/intune-gpanalyticsservice-grouppolicysettingmapping-list.md)|[коллекция groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Список свойств и связей объектов [groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|
|[Get groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-get.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Чтение свойств и связей объекта [groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|
|[Создание groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-create.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Создайте новый [объект groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|
|[Удаление groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-delete.md)|Нет|Удаляет [группуPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md).|
|[Update groupPolicySettingMapping](../api/intune-gpanalyticsservice-grouppolicysettingmapping-update.md)|[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Обновление свойств объекта [groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Пока не задокументировано.|
|parentId|String|Родительский Id параметра групповой политики.|
|childIdList|Коллекция объектов string|Список детских ид параметра групповой политики.|
|settingName|String|Имя этого параметра групповой политики.|
|settingValue|String|Значение этого параметра групповой политики.|
|settingValueType|String|Тип значения этого параметра групповой политики.|
|settingDisplayName|String|Отображение имени этого параметра групповой политики.|
|settingDisplayValue|String|Отображение значения этого параметра групповой политики.|
|settingDisplayValueType|String|Тип отображения значения этого параметра групповой политики.|
|settingValueDisplayUnits|String|Отображаемая единица этого значения групповой политики|
|settingCategory|String|Категория, в которая находится параметр групповой политики.|
|mdmCspName|String|CSP назовет эту групповую политику, устанавливая карты.|
|mdmSettingUri|String|MDM CSP URI этой групповой политики, устанавливая карты.|
|mdmMinimumOSVersion|Int32|Минимальная версия ОС, поддерживаемая этим параметром mdm.|
|settingType|[groupPolicySettingType](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|Тип параметра (безопасность или admx) групповой политики. Возможные значения: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.|
|isMdmSupported|Boolean|Указывает, поддерживает ли параметр Intune или нет.|
|mdmSupportedState|[mdmSupportedState](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|Указывает, поддерживается ли параметр в Mdm или нет. Возможные значения: `unknown`, `supported`, `unsupported`, `deprecated`.|
|settingScope|[groupPolicySettingScope](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|Область настройки. Возможные значения: `unknown`, `device`, `user`.|
|intuneSettingUriList|Коллекция объектов string|Список URL-адресов intune Setting this group policy setting maps to|
|intuneSettingDefinitionId|String|Id определения параметра Intune|
|admxSettingDefinitionId|String|Admx Group Policy Id|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicySettingMapping"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "String (identifier)",
  "parentId": "String",
  "childIdList": [
    "String"
  ],
  "settingName": "String",
  "settingValue": "String",
  "settingValueType": "String",
  "settingDisplayName": "String",
  "settingDisplayValue": "String",
  "settingDisplayValueType": "String",
  "settingValueDisplayUnits": "String",
  "settingCategory": "String",
  "mdmCspName": "String",
  "mdmSettingUri": "String",
  "mdmMinimumOSVersion": 1024,
  "settingType": "String",
  "isMdmSupported": true,
  "mdmSupportedState": "String",
  "settingScope": "String",
  "intuneSettingUriList": [
    "String"
  ],
  "intuneSettingDefinitionId": "String",
  "admxSettingDefinitionId": "String"
}
```



