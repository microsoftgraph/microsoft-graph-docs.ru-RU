---
title: Тип ресурса Девицеманажементконфигуратионстрингсеттингвалуедефинитион
description: Ограничения строк
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03a96252cffabddd2acb613ff365fd16951fd55c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242384"
---
# <a name="devicemanagementconfigurationstringsettingvaluedefinition-resource-type"></a>Тип ресурса Девицеманажементконфигуратионстрингсеттингвалуедефинитион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничения строк


Наследуется от [девицеманажементконфигуратионсеттингвалуедефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|format|[девицеманажементконфигуратионстрингформат](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringformat.md)|Предварительно определенный формат строки. Возможные значения: `none` , `email` ,,,,, `guid` `ip` `base64` `url` `version` ,,, `xml` `date` `time` , `binary` , `regEx` , `json` , `dateTime` , `surfaceHub` .|
|инпутвалидатионсчема|String|Регулярное выражение или любая схема XML или JSON, которой должна быть соотнесена входная строка|
|максимумленгс|Int64|Максимальная длина строки. Допустимые значения — от 0 до 87516|
|минимумленгс|Int64|Минимальная длина строки. Допустимые значения — от 0 до 87516|
|Secret|Boolean|Указывает, нужно ли считать параметр секретом. Параметры, помеченные как "Да", будут зашифрованы на транспорте и будут отображаться в виде звездочек, когда они представлены в пользовательском интерфейсе.|

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




