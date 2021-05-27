---
title: excludeTarget resource type
description: Представляет пользователей или группы пользователей, которые исключены из политики.
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9d2786a6107e524fe00430658542dea374cae275
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682948"
---
# <a name="excludetarget-resource-type"></a>excludeTarget resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователей или группы пользователей, которые исключены из политики.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор объекта пользователя или группы Azure AD.|
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
