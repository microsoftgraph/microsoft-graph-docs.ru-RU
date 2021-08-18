---
title: deviceManagementConfigurationIntegerSettingValueDefinitionTemplate type
description: Шаблон определения значения параметра integer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a7fa81700aa71a076da45b7703f1f638987a4f1b9aa107409bf8fb4934b90d1d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182912"
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




