---
author: daspek
ms.author: dspektor
title: Тип ресурса ItemActionSet
description: Объект itemActionSet предоставляет сведения о действиях, выполняемых в рамках действия с элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a28a3380761e2d1914d7c088e5927fc5d3addd4b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036724"
---
# <a name="itemactionset-resource-type"></a>Тип ресурса itemActionSet

Ресурс **itemActionSet** предоставляет сведения о действиях, которые составляют [действие][itemActivity] для элемента.

>**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

[itemActivity]: itemactivity.md

## <a name="properties"></a>Свойства

В настоящее время доступны следующие действия. Так как новые действия могут быть добавлены в будущем, убедитесь, что ваше приложение может обрабатывать **itemActionSet** , который включает неизвестные действия.

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

## <a name="json-representation"></a>Представление JSON

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

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->
