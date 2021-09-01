---
title: тип ресурса deviceManagementConfigurationSettingInstanceTemplate
description: Настройка шаблона экземпляра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b4ebc516dc521c022a5b5a5e9eeb460dec3e4497
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58782114"
---
# <a name="devicemanagementconfigurationsettinginstancetemplate-resource-type"></a>тип ресурса deviceManagementConfigurationSettingInstanceTemplate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Настройка шаблона экземпляра

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settingInstanceTemplateId|Строка|Настройка кода шаблона экземпляра|
|settingDefinitionId|Строка|Настройка Id определения|
|isRequired|Boolean|Указывает, должна ли политика указать этот параметр.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true
}
```



