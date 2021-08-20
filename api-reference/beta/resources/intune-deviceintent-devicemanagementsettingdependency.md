---
title: тип ресурса deviceManagementSettingDependency
description: Сведения о зависимости для параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d5f29fecdde1b3a7a62ed72fcd96aceeb2a10385028106be288c7d8bcaff2254
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54173039"
---
# <a name="devicemanagementsettingdependency-resource-type"></a>тип ресурса deviceManagementSettingDependency

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения о зависимости для параметра

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|definitionId|Строка|ID определения параметра зависит от|
|ограничения|[коллекция deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)|Коллекция ограничений для значения параметра зависимостей|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDependency",
  "definitionId": "String",
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "String"
      ]
    }
  ]
}
```




