---
title: тип ресурса deviceManagementConfigurationStringSettingValueTemplate
description: Шаблон значения параметра строки
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8f09a8e9197a88a7de5954172703c1e18a109e5f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148195"
---
# <a name="devicemanagementconfigurationstringsettingvaluetemplate-resource-type"></a>тип ресурса deviceManagementConfigurationStringSettingValueTemplate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Шаблон значения параметра строки


Наследует [от deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settingValueTemplateId|String|Настройка кода шаблона значений, унаследованный от [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)|
|defaultValue|[deviceManagementConfigurationStringSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvaluedefaulttemplate.md)|Шаблон параметра параметра строки по умолчанию.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
  "settingValueTemplateId": "String",
  "defaultValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
    "constantValue": "String"
  }
}
```



