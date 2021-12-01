---
title: тип internalSponsors сложный
description: Определяет отношение к другому пользователю в клиенте, которому будет разрешено в качестве утвержденного.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b11305f40e7a16f833ee0ef42c66122126bea515
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242662"
---
# <a name="internalsponsors-complex-type"></a>тип internalSponsors сложный

Пространство имен: microsoft.graph

Используется на этапе утверждения политики назначения пакета доступа.
Это подтип [subjectSet,](subjectset.md)в котором значение указывает, что автором утверждения должны быть внутренние спонсоры связанной организации `@odata.type` `#microsoft.graph.internalSponsors` пользователя. Этот одобрение применимо только к запросам пользователей, которые являются частью связанной организации.  При создании этапа утверждения политики назначения пакетов доступа с помощью внутреннихSponsors также включаем другого участника, например одного пользователя или члена группы, в случае, если подключенная организация не имеет внутреннего спонсора.

## <a name="properties"></a>Свойства

Нет
## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.internalSponsors",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.internalSponsors"
}
```




