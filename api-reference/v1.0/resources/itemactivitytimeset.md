---
author: daspek
ms.author: dspektor
title: Тип ресурса itemActivityTimeSet
description: Объект itemActionSet предоставляет сведения о действиях, которые были выполнены над элементом.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4ef0b56471afe78b13edc2f6efb25941c9a749df
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970816"
---
# <a name="itemactivitytimeset-resource-type"></a>Тип ресурса itemActivityTimeSet

Ресурс **itemActivityTimeSet** предоставляет сведения о том, когда выполнялось [действие] [ activity] для элемента.

>**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

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
