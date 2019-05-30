---
author: daspek
ms.author: dspektor
title: Тип ресурса itemActivity
description: Объект itemActivity предоставляет сведения о действиях, которые были выполнены над элементом.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 98ae9e4881de18c94490469b10df43b2aaf58140
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536689"
---
# <a name="itemactivity-resource-type"></a>Тип ресурса itemActivity

Ресурс **itemActivity** предоставляет сведения о действиях, выполняемых над элементом или в контейнере.
В настоящее время доступен только в SharePoint и OneDrive для бизнеса.

Действия, выполняемые в itemActivity, подробно описаны в свойстве [itemActionSet][] .

>**Примечание:** **itemActivity** в настоящее время доступно только в SharePoint и OneDrive для бизнеса.

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a>Свойства

| Свойство | Тип                    | Описание
|:---------|:------------------------|:----------------------------------------
| id       | string                  | Уникальный идентификатор действия. Только для чтения.
| обращения   | [Акцессактион][]        | Доступ к элементу.
| actor    | [identitySet][]         | Удостоверение, выполнившее действие. Только для чтения.
| activityDateTime    | DateTimeOffset | Сведения о том, когда было выполнено действие. Только для чтения.

[Акцессактион]: accessaction.md
[identitySet]: identityset.md

## <a name="relationships"></a>Связи

| Имя связи | Тип          | Описание
|:------------------|:--------------|:-----------------------------------------
| driveItem         | [driveItem][] | Представляет объект **driveItem**, с которым было выполнено действие.
| listItem          | [listItem][]  | Представляет объект **listItem**, с которым было выполнено действие.

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivity",
  "@type.aka": "oneDrive.activityEntity"
}-->

```json
{
  "id": "string (identifier)",
  "access": "microsoft.graph.accessAction",
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "activityDateTime": {"@odata.type": "String (timestamp)"}
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActivity",
  "suppressions": []
}
-->
