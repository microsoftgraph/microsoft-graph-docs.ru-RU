---
title: excludeTarget resource type
description: Представляет пользователей или группы пользователей, которые исключены из политики.
author: mjsantani
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 368d6446d9dbead0ccacfb5538c3433050b6c79c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034409"
---
# <a name="excludetarget-resource-type"></a>excludeTarget resource type

Пространство имен: microsoft.graph

Представляет пользователей или группы пользователей, которые исключены из политики.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор объекта пользователя Azure Active Directory группы.|
|targetType|authenticationMethodTargetType|Тип целевой цели метода проверки подлинности. Возможные значения: `user`, `group`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludeTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludeTarget",
  "id": "String (identifier)",
  "targetType": "String"
}
```
