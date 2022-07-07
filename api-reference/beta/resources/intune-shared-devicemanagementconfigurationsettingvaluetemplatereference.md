---
title: Тип ресурса deviceManagementConfigurationSettingValueTemplateReference
description: Настройка справочных сведений о шаблоне значений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fa4ecc07044d90bfc869467de8e8249f7581e228
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66672024"
---
# <a name="devicemanagementconfigurationsettingvaluetemplatereference-resource-type"></a>Тип ресурса deviceManagementConfigurationSettingValueTemplateReference

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Настройка справочных сведений о шаблоне значений

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settingValueTemplateId|String|Задание идентификатора шаблона значения|
|useTemplateDefault|Логическое|Указывает, следует ли обновлять значение параметра политики в соответствии со значением по умолчанию для параметра шаблона.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
  "settingValueTemplateId": "String",
  "useTemplateDefault": true
}
```




