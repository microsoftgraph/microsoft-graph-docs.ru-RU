---
title: тип ресурса deviceManagementConfigurationStringSettingValueDefinition
description: Ограничения строки
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a497972c8d84781cb5984993389fdb1163514f0d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128846"
---
# <a name="devicemanagementconfigurationstringsettingvaluedefinition-resource-type"></a>тип ресурса deviceManagementConfigurationStringSettingValueDefinition

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничения строки


Наследует [от deviceManagementConfigurationSettingValueDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|format|[deviceManagementConfigurationStringFormat](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringformat.md)|Заранее определенный формат строки. Возможные значения: `none` `email` , , , , , `guid` , `ip` , `base64` `url` `version` `xml` `date` , `time` `binary` `regEx` `json` `dateTime` `surfaceHub` , .|
|inputValidationSchema|String|Регулярное выражение или схема xml или json, которая должна соответствовать строке ввода|
|maximumLength|Int64|Максимальная длина строки. Допустимые значения от 0 до 87516|
|minimumLength|Int64|Минимальная длина строки. Допустимые значения от 0 до 87516|
|isSecret|Логическое|Указывает, нужно ли относиться к параметру как к секрету. Параметры пометка да будет зашифрована в транзите и в покое и будет отображаться в виде звездочек при их представлении в UX.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationStringSettingValueDefinition",
  "format": "String",
  "inputValidationSchema": "String",
  "maximumLength": 1024,
  "minimumLength": 1024,
  "isSecret": true
}
```



