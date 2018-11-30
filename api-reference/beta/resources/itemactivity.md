---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivity
ms.openlocfilehash: 7c8cdab7adc705333d1aeaad526aeeb813de10a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081167"
---
# <a name="itemactivity-resource-type"></a>Тип ресурса ItemActivity

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **ItemActivity** предоставляет сведения о действиях, выполненных с элементом или в контейнере.
В настоящее время он доступен только в SharePoint и OneDrive для бизнеса.

## <a name="json-representation"></a>Представление в формате JSON

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
| id       | строка                  | Уникальный идентификатор действия. Только для чтения.
| Access   | [accessAction][]        | Обращения к элемента.
| action   | [itemActionSet][]       | Сведения о выполненном действии. Только для чтения.
| actor    | [identitySet][]         | Удостоверение, выполнившее действие. Только для чтения.
| location | [location][]            | Физическое расположение, где было выполнено действие. Только для чтения.
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

[accessAction]: accessaction.md
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

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity"
} -->
