---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionSet
ms.openlocfilehash: 3b2f77ea21f2352b0a8fa647af84d9b0af08a2ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075124"
---
# <a name="itemactionset-resource-type"></a>Тип ресурса ItemActionSet

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **ItemActionSet** содержит сведения о действиях, входящих в состав [операции][itemActivity] над элементом.

[itemActivity]: itemactivity.md

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActionSet",
  "@type.aka": "oneDrive.action"
}-->

```json
{
  "comment": {"@odata.type": "microsoft.graph.commentAction"},
  "create": {"@odata.type": "microsoft.graph.createAction"},
  "delete": {"@odata.type": "microsoft.graph.deleteAction"},
  "edit": {"@odata.type": "microsoft.graph.editAction"},
  "mention": {"@odata.type": "microsoft.graph.mentionAction"},
  "move": {"@odata.type": "microsoft.graph.moveAction"},
  "rename": {"@odata.type": "microsoft.graph.renameAction"},
  "restore": {"@odata.type": "microsoft.graph.restoreAction"},
  "share": {"@odata.type": "microsoft.graph.shareAction"},
  "version": {"@odata.type": "microsoft.graph.versionAction"},
  
}
```

## <a name="properties"></a>Свойства

Ниже перечислены действия, доступные в настоящее время.
В будущем можно будет вносить в журнал новые действия, поэтому ваше приложение должно быть способно обрабатывать объект **itemActionSet**, содержащий действия, не предусмотренные в приложении.

| Имя свойства | Тип              | Описание
|:--------------|:------------------|:-----------------------------------------
| comment       | [commentAction][] | В элемент добавлен комментарий.
| create        | [createAction][]  | Был создан элемент.
| delete        | [deleteAction][]  | Был удален элемент.
| edit          | [editAction][]    | Был изменен элемент.
| mention       | [mentionAction][] | Пользователь был упомянут в элементе.
| move          | [moveAction][]    | Элемент был перемещен.
| rename        | [renameAction][]  | Элемент был переименован.
| restore       | [restoreAction][] | Элемент был восстановлен.
| share         | [shareAction][]   | К элементу был предоставлен общий доступ.
| version       | [versionAction][] | Для элемента была указана версия.

[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a>Замечания

На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet"
} -->
