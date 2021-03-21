---
title: тип ресурса appConsentRequestScope
description: Сведения о динамических области разрешений, для которых запрашивается доступ.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b960820e0d7cf20a37850256bb96ba3abf034038
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965232"
---
# <a name="appconsentrequestscope-resource-type"></a>тип ресурса appConsentRequestScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В **appConsentRequestScope** подробно извещаются динамические области разрешений, для которых запрашивается доступ.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя области.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConsentRequestScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConsentRequestScope",
  "displayName": "String"
}
```

