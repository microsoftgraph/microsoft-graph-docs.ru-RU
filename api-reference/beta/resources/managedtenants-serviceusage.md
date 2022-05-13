---
title: Тип ресурса serviceUsage
description: Представляет ежемесячные активные данные об использовании для службы в управляемом клиенте.
author: kylewirpel
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: f680af26313e38da441408f6a127b21c14a7a045
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398954"
---
# <a name="serviceusage-resource-type"></a>Тип ресурса serviceUsage

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ежемесячные активные данные об использовании для службы в управляемом клиенте.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|monthlyActiveUsers|Int32|Количество ежемесячных активных пользователей службы. Обязательно. Только для чтения.|
|serviceName|String|Имя службы Microsoft 365, которая сгенерировала использование. Обязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.serviceUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.serviceUsage",
  "serviceName": "String",
  "monthlyActiveUsers": "Integer"
}
```

