---
title: тип ресурса deviceManagementConfigurationSettingValueTemplateReference
description: Настройка справочной информации шаблона значений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 19360005b1076256898454be1d5463e21d67fa25
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58804843"
---
# <a name="devicemanagementconfigurationsettingvaluetemplatereference-resource-type"></a>тип ресурса deviceManagementConfigurationSettingValueTemplateReference

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Настройка справочной информации шаблона значений

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settingValueTemplateId|Строка|Настройка id шаблона значений|
|useTemplateDefault|Логический|Указывает, следует ли обновлять значение параметра политики, чтобы соответствовать значению параметра шаблона по умолчанию|

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



