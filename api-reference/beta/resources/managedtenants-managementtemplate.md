---
title: тип ресурсов managementTemplate
description: Представляет группу действий и параметр, которые можно выполнить в отношении управляемого клиента.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 6dacd5d94c921ca4afd59219be24509f6879c5b8
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792052"
---
# <a name="managementtemplate-resource-type"></a>тип ресурсов managementTemplate

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет группу действий и параметр, которые можно выполнить в отношении управляемого клиента.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Управление спискамиTemplates](../api/managedtenants-managedtenant-list-managementtemplates.md)|[коллекция microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)|Получите список объектов [managementTemplate](../resources/managedtenants-managementtemplate.md) и их свойств.|
|[Get managementTemplate](../api/managedtenants-managementtemplate-get.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)|Ознакомьтесь с свойствами и отношениями [объекта managementTemplate.](../resources/managedtenants-managementtemplate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|category|managementCategory|Категория управления для шаблона управления. Возможные значения: `custom`, `devices`, `identity`, `unknownFutureValue`. Обязательный. Только для чтения.|
|description|String|Описание шаблона управления. Необязательно. Только для чтения.|
|displayName|String|Имя отображения шаблона управления. Обязательное. Только для чтения.|
|id|String|Уникальный идентификатор шаблона управления. Обязательное. Только для чтения.|
|parameters|[коллекция microsoft.graph.managedTenants.templateParameter](../resources/managedtenants-templateparameter.md)|Коллекция параметров, используемых шаблоном управления. Необязательно. Только для чтения.|
|workloadActions|[коллекция microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md)|Набор действий рабочей нагрузки, связанных с шаблоном управления. Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "category": "String",
  "parameters": [
    {
      "@odata.type": "microsoft.graph.managedTenants.templateParameter"
    }
  ],
  "workloadActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadAction"
    }
  ]
}
```
