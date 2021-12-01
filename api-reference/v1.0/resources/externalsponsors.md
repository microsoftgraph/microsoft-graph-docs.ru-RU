---
title: сложный тип externalSponsors
description: Определяет отношение к другому пользователю в клиенте, которому будет разрешено в качестве утвержденного.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 34db10f8efe76d324d2b6577a0e7a5efcb311dc8
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242665"
---
# <a name="externalsponsors-complex-type"></a>сложный тип externalSponsors

Пространство имен: microsoft.graph

Используется на этапе утверждения политики назначения пакета доступа.
Это подтип [subjectSet,](subjectset.md)в котором значение указывает, что автором утверждения должны быть внешние спонсоры связанной организации `@odata.type` `#microsoft.graph.externalSponsors` пользователя. Этот одобрение применимо только к запросам пользователей, которые являются частью связанной организации.  При создании этапа утверждения политики назначения пакета доступа с внешнимиSponsors также включаем другого участника, например одного пользователя или члена группы, в случае, если подключенная организация не имеет внешнего спонсора.

## <a name="properties"></a>Свойства

Нет
## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalSponsors",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalSponsors"
}
```



