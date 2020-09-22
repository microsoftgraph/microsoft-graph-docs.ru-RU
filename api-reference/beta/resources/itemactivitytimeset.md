---
author: daspek
description: Ресурс ItemActivityTimeSet предоставляет сведения о том, когда было совершено действие над элементом.
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9295337237c681fd0ec02c9fa8061bf206059600
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075667"
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
  "@property.aka": "observedDateTime=observedTime recordedDateTime=recordedTime"
}-->

```json
{
  "observedDateTime": "String (timestamp)",
  "recordedDateTime": "String (timestamp)"
}
```

## <a name="properties"></a>Свойства

| Имя свойства    | Тип           | Описание
|:-----------------|:---------------|:-----------------------------------------
| observedDateTime | DateTimeOffset | Сведения о том, когда было обнаружено действие.
| recordedDateTime | DateTimeOffset | Сведения о том, когда сведения об обнаружении действия были записаны в службе.

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


