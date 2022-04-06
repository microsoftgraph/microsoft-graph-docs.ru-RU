---
author: daspek
description: Ресурс ItemActivityTimeSet предоставляет сведения о том, когда было совершено действие над элементом.
ms.date: 09/14/2017
title: ItemActivityTimeSet
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: eb0477255783b3aba7aaa61a0e9ece868c1882d1
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63724327"
---
# <a name="itemactivitytimeset-resource-type"></a>Тип ресурса ItemActivityTimeSet

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **ItemActivityTimeSet** предоставляет сведения о том, когда было совершено [действие][activity] над элементом.

[activity]: itemactivity.md

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivityTimeSet",
  "@type.aka": "oneDrive.times",
  "@property.aka&quot;: &quot;observedDateTime=observedTime recordedDateTime=recordedTime"
}-->

```json
{
  "observedDateTime": "String (timestamp)",
  "recordedDateTime": "String (timestamp)"
}
```

## <a name="properties"></a>Свойства

| Свойство         | Тип           | Описание                                       |
| :--------------- | :------------- | :------------------------------------------------ |
| observedDateTime | DateTimeOffset | Сведения о том, когда было обнаружено действие.     |
| recordedDateTime | DateTimeOffset | Сведения о том, когда сведения об обнаружении действия были записаны в службе. |

Разница между временем **обнаружения** и **записи** особенно важна для сценариев совместной работы в автономном режиме.
Если пользователь добавляет комментарий к файлу в автономном режиме, то время добавления этого комментария будет указано в свойстве **observedDateTime**.
Позже при подключении пользователя к облаку и отправке изменений это время будет указано в свойстве **recordedDateTime**.

## <a name="remarks"></a>Замечания

На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": []
}
-->
