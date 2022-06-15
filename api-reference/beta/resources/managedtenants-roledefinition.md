---
title: Тип ресурса roleDefinition
description: Представляет подробные сведения об определении роли.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 6d2a34d8e6130a894341bcbbb735910c9357d3ce
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096408"
---
# <a name="roledefinition-resource-type"></a>Тип ресурса roleDefinition

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения об определении роли.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|Описание роли.|
|displayName|Строка|Отображаемое имя для назначения роли.|
|templateId|String|Уникальный идентификатор шаблона.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.roleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.roleDefinition",
  "description": "String",
  "displayName": "String",
  "templateId": "String"
}
```
