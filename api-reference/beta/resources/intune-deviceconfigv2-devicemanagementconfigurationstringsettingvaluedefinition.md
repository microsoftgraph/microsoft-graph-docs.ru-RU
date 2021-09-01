---
title: тип ресурса deviceManagementConfigurationStringSettingValueDefinition
description: Ограничения строки
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9731c46e9ae80f346bef29d951f4e430d76743f3
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58815080"
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
|inputValidationSchema|Строка|Регулярное выражение или схема xml или json, которая должна соответствовать строке ввода|
|maximumLength|Int64|Максимальная длина строки. Допустимые значения от 0 до 87516|
|minimumLength|Int64|Минимальная длина строки. Допустимые значения от 0 до 87516|
|isSecret|Логический|Указывает, нужно ли относиться к параметру как к секрету. Параметры пометка да будет зашифрована в транзите и в покое и будет отображаться в виде звездочек при их представлении в UX.|

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



