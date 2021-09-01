---
title: deviceManagementConfigurationIntegerSettingValueDefinitionTemplate type
description: Шаблон определения значения параметра integer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6aa5571402ccddf6cf5524e2e2486caffcc550c7
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820725"
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

## <a name="relationships"></a>Связи
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



