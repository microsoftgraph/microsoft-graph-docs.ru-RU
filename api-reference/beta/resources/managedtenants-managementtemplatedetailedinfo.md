---
title: тип ресурсов managementTemplateDetailedInfo
description: Представляет подробные сведения для шаблона управления.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 7ece5863f33f447a6e79ea75e1959ea7011b0c32
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861353"
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
