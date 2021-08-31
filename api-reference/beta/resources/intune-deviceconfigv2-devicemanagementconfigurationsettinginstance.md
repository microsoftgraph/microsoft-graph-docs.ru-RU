---
title: тип ресурса deviceManagementConfigurationSettingInstance
description: Настройка экземпляра в политике
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 33a7f9b14ded2dbc21df07f7ccde934fb16295f1
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788670"
---
# <a name="devicemanagementconfigurationsettinginstance-resource-type"></a>тип ресурса deviceManagementConfigurationSettingInstance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Настройка экземпляра в политике

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settingDefinitionId|Строка|Настройка Id определения|
|settingInstanceTemplateReference|[deviceManagementConfigurationSettingInstanceTemplateReference](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplatereference.md)|Настройка ссылки шаблона экземпляра|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingInstance",
  "settingDefinitionId": "String",
  "settingInstanceTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
    "settingInstanceTemplateId": "String"
  }
}
```



