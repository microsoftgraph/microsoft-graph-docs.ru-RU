---
title: тип ресурса deviceManagementConfigurationDependentOn
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f216b43ae577d670763a3fe3c2b26f3a14d84072
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128951"
---
# <a name="devicemanagementconfigurationdependenton-resource-type"></a>тип ресурса deviceManagementConfigurationDependentOn

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|dependentOn|String|Идентификатор родительского параметра и параметра родительского параметра, зависящих от|
|parentSettingId|String|Идентификатор родительского или родительского идентификатора параметров, зависящих от|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationDependentOn",
  "dependentOn": "String",
  "parentSettingId": "String"
}
```



