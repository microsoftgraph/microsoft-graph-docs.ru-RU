---
title: тип ресурса deviceManagementConfigurationReferredSettingInformation
description: Переданные сведения о параметре повторного параметров
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2a38d8566084999a291f770267745fe81015c5b9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58795531"
---
# <a name="devicemanagementconfigurationreferredsettinginformation-resource-type"></a>тип ресурса deviceManagementConfigurationReferredSettingInformation

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Переданные сведения о параметре повторного параметров

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settingDefinitionId|Строка|Настройка id определения, который ссылается на параметр. Применимо для повторного параметров|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
  "settingDefinitionId": "String"
}
```



