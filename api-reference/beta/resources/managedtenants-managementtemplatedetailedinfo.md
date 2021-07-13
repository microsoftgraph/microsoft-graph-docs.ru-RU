---
title: тип ресурсов managementTemplateDetailedInfo
description: Представляет подробные сведения для шаблона управления.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: e98d2ca41bc972a5dca33c575363b1bac27d87a5
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403096"
---
# <a name="managementtemplatedetailedinfo-resource-type"></a>тип ресурсов managementTemplateDetailedInfo

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения для шаблона управления.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|category|managementCategory|Категория управления для шаблона управления. Возможные значения: `custom`, `devices`, `identity`, `unknownFutureValue`. Обязательный. Только для чтения.|
|displayName|String|Имя отображения шаблона управления. Обязательный. Только для чтения.|
|managementTemplateId|String|Уникальный идентификатор шаблона управления. Обязательный. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateDetailedInfo",
  "managementTemplateId": "String",
  "displayName": "String",
  "category": "String"
}
```
