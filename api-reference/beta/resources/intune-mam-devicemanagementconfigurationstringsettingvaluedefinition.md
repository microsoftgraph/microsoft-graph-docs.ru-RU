---
title: Тип ресурса deviceManagementConfigurationStringSettingValueDefinition
description: Ограничения строк
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7602bccd66669f9b54c8bad06bb17ac350f641b4
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671725"
---
# <a name="devicemanagementconfigurationstringsettingvaluedefinition-resource-type"></a>Тип ресурса deviceManagementConfigurationStringSettingValueDefinition

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничения строк


Наследует от [deviceManagementConfigurationSettingValueDefinition](../resources/intune-shared-devicemanagementconfigurationsettingvaluedefinition.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|format|[deviceManagementConfigurationStringFormat](../resources/intune-shared-devicemanagementconfigurationstringformat.md)|Предварительно определенный формат строки. Возможные значения: `none`, , `email`, `guid`, `ip`, `base64`, `url``version`, `xml`, `date`, `time`, `binary``regEx`, , `json`, . `dateTime``surfaceHub`|
|inputValidationSchema|String|Регулярное выражение или любая схема XML или JSON, которая должна соответствовать входной строке|
|maximumLength|Int64|Максимальная длина строки|
|minimumLength|Int64|Минимальная длина строки|
|isSecret|Логическое|Указывает, должен ли параметр обрабатываться как секрет. Параметры, помеченные как "да", будут зашифрованы при передаче и при хранении и будут отображаться в виде звездочки при их отображении в пользовательском интерфейсе.|

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




