---
title: тип ресурса workloadAction
description: Представляет действие, которое будет выполняться для определенной рабочей нагрузки.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: fe63c772abfffb85c12d7f753c03bb6a1f168ad4
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792017"
---
# <a name="workloadaction-resource-type"></a>тип ресурса workloadAction

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, которое будет выполняться для определенной рабочей нагрузки.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionId|String|Уникальный идентификатор для действия рабочей нагрузки. Обязательное. Только для чтения.|
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
