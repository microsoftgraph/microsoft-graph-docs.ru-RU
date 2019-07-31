---
author: daspek
description: Ресурс ItemActivity предоставляет сведения о действиях, выполненных с элементом или в контейнере.
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ab96c3169a2d2dc37e6b94ab325866e93fa4d6c0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967105"
---
# <a name="itemactivity-resource-type"></a>Тип ресурса ItemActivity

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **ItemActivity** предоставляет сведения о действиях, выполненных с элементом или в контейнере.
В настоящее время доступен только в SharePoint и OneDrive для бизнеса.

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
  "action": {"@odata.type": "microsoft.graph.itemActionSet"},
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "location": {"@odata.type": "microsoft.graph.location"},
  "times": {"@odata.type": "microsoft.graph.itemActivityTimeSet"}
}
```

## <a name="properties"></a>Свойства

| Свойство | Тип                    | Описание
|:---------|:------------------------|:----------------------------------------
| id       | string                  | Уникальный идентификатор действия. Только для чтения.
| обращения   | [Акцессактион][]        | Доступ к элементу.
| action   | [itemActionSet][]       | Сведения о выполненном действии. Только для чтения.
| actor    | [identitySet][]         | Удостоверение, выполнившее действие. Только для чтения.
| location | [location][]            | Физическое расположение, в котором было выполнено действие. Только для чтения.
| times    | [itemActivityTimeSet][] | Сведения о том, когда было выполнено действие. Только для чтения.

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a>Связи

| Имя связи | Тип          | Описание
|:------------------|:--------------|:-----------------------------------------
| driveItem         | [driveItem][] | Представляет объект **driveItem**, с которым было выполнено действие.
| listItem          | [listItem][]  | Представляет объект **listItem**, с которым было выполнено действие.

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a>Действия

Операции, выполненные в ходе действия, описываются в свойстве **action**.
Ниже перечислены действия, доступные в настоящее время.
В будущем можно будет вносить в журнал новые действия, поэтому убедитесь, что ваше приложение позволяет обрабатывать объект **itemActivity** без каких-либо действий, которые "понимает" ваше приложение.

| Название действия | Тип              | Описание
|:------------|:------------------|:-------------------------------------------
| comment     | [commentAction][] | В элемент добавлен комментарий.
| create      | [createAction][]  | Был создан элемент.
| delete      | [deleteAction][]  | Был удален элемент.
| edit        | [editAction][]    | Был изменен элемент.
| mention     | [mentionAction][] | Пользователь был упомянут в элементе.
| move        | [moveAction][]    | Элемент был перемещен.
| rename      | [renameAction][]  | Элемент был переименован.
| restore     | [restoreAction][] | Элемент был восстановлен.
| share       | [shareAction][]   | К элементу был предоставлен общий доступ.
| version     | [versionAction][] | Для элемента была указана версия.

[Акцессактион]: accessaction.md
[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[location]: location.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a>Замечания

В настоящее время ресурс **ItemActivity** доступен только в SharePoint и OneDrive для бизнеса.

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity",
  "suppressions": []
}
-->
