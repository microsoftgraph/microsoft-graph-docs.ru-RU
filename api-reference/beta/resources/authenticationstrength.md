---
title: тип ресурса authenticationStrength
description: Сила настраиваемой проверки подлинности, примененная в политике условного доступа
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a316d3d6f575183fcb59647355545746838b0cdf
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647241"
---
# <a name="authenticationstrength-resource-type"></a>тип ресурса authenticationStrength

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Настраиваемая сила проверки подлинности, примененная в политике условного доступа. 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|authenticationStrengthId|String|Идентификатор силы проверки подлинности.|
|displayName|String|Имя силы проверки подлинности.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationStrength"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationStrength",
  "authenticationStrengthId": "String",
  "displayName": "String"
}
```

