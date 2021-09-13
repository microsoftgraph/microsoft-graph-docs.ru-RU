---
title: deviceManagementConfigurationIntegerSettingValueDefinitionTemplate type
description: Шаблон определения значения параметра integer
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1a39f6c3224487c826cbfd8dcabf6e4cb629b665
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59069035"
---
# <a name="devicemanagementconfigurationintegersettingvaluedefinitiontemplate-resource-type"></a>deviceManagementConfigurationIntegerSettingValueDefinitionTemplate type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Шаблон определения значения параметра integer

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|minValue|Int32|Параметр "Integer", устанавливая минимальное значение. Допустимые значения 2147483648 2147483647|
|maxValue|Int32|Параметр "Integer", устанавливая максимальное значение. Допустимые значения 2147483648 2147483647|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate",
  "minValue": 1024,
  "maxValue": 1024
}
```



