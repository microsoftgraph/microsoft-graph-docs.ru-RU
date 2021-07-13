---
title: тип ресурса workloadAction
description: Представляет действие, которое будет выполняться для определенной рабочей нагрузки.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: e6dbbe1458aa6dba37a26af70ee0e64b92a52cf4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402598"
---
# <a name="workloadaction-resource-type"></a>тип ресурса workloadAction

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, которое будет выполняться для определенной рабочей нагрузки.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionId|String|Уникальный идентификатор для действия рабочей нагрузки. Обязательный. Только для чтения.|
|category|workloadActionCategory|Категория действия рабочей нагрузки. Возможные значения: `automated`, `manual`, `unknownFutureValue`. Необязательно. Только для чтения.|
|description|String|Описание действия рабочей нагрузки. Необязательно. Только для чтения.|
|displayName|String|Отображает имя для действия рабочей нагрузки. Необязательно. Только для чтения.|
|service|String|Служба, связанная с действием рабочей нагрузки. Необязательно. Только для чтения.|
|settings|[коллекция microsoft.graph.managedTenants.setting](../resources/managedtenants-setting.md)|Коллекция параметров, связанных с действием рабочей нагрузки. Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadAction",
  "actionId": "String",
  "category": "String",
  "displayName": "String",
  "description": "String",
  "service": "String",
  "settings": [
    {
      "@odata.type": "microsoft.graph.managedTenants.setting"
    }
  ]
}
```
