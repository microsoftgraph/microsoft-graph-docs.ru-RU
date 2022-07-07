---
title: Тип ресурса deviceManagementConfigurationReferenceSettingValue
description: Модель для ReferenceSettingValue
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: edc233723cc655b6f0d731bceab9f10a1d92644c
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671750"
---
# <a name="devicemanagementconfigurationreferencesettingvalue-resource-type"></a>Тип ресурса deviceManagementConfigurationReferenceSettingValue

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Модель для ReferenceSettingValue


Наследует от [deviceManagementConfigurationStringSettingValue](../resources/intune-shared-devicemanagementconfigurationstringsettingvalue.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settingValueTemplateReference|[deviceManagementConfigurationSettingValueTemplateReference](../resources/intune-shared-devicemanagementconfigurationsettingvaluetemplatereference.md)|Установка ссылки на шаблон значения, унаследованного от [deviceManagementConfigurationSettingValue](../resources/intune-shared-devicemanagementconfigurationsettingvalue.md)|
|value|String|Значение параметра строки. Наследуется [от deviceManagementConfigurationStringSettingValue](../resources/intune-shared-devicemanagementconfigurationstringsettingvalue.md)|
|Примечание|String|Примечание, которое администратор может использовать для размещения контекстных сведений|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationReferenceSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationReferenceSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  },
  "value": "String",
  "note": "String"
}
```




