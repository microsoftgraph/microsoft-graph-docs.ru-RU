---
author: daspek
title: Тип ресурса itemActivityTimeSet
description: Объект itemActionSet предоставляет сведения о действии, которое произошло с элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 1f614c597efdb95b04c4079bd68240aa865d66dd
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238675"
---
# <a name="itemactivitytimeset-resource-type"></a>Тип ресурса itemActivityTimeSet

Пространство имен: microsoft.graph

Ресурс **itemActivityTimeSet** предоставляет сведения [][activity] о том, когда произошло действие с элементом.

>**Примечание.** Записи о действиях с элементами в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

[activity]: itemactivity.md

## <a name="properties"></a>Свойства

| Имя свойства    | Тип           | Описание
|:-----------------|:---------------|:-----------------------------------------
| observedDateTime | DateTimeOffset | Сведения о том, когда было обнаружено действие.
| recordedDateTime | DateTimeOffset | Сведения о том, когда сведения об обнаружении действия были записаны в службе.

Разница между временем **обнаружения** и **записи** особенно важна для сценариев совместной работы в автономном режиме.
Если пользователь добавляет комментарий к файлу в автономном режиме, то время добавления этого комментария будет указано в свойстве **observedDateTime**.
Позже при подключении пользователя к облаку и отправке изменений это время будет указано в свойстве **recordedDateTime**.

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

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->

