---
author: daspek
title: тип ресурса itemActivity
description: Объект itemActivity предоставляет сведения о действии, которое произошло на элементе.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 2a22b78e517e3faf064073033ec1b4b9c582055d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089349"
---
# <a name="itemactivity-resource-type"></a>тип ресурса itemActivity

Пространство имен: microsoft.graph

Ресурс **itemActivity** предоставляет сведения о действиях, которые произошли на элементе или в контейнере.
В настоящее время доступен только в SharePoint и OneDrive для бизнеса.

Действия, которые произошли в itemActivity, подробно описаны в [свойстве itemActionSet.][]

>**Примечание.** **ItemActivity** в настоящее время доступна только на SharePoint и OneDrive для бизнеса.

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a>Свойства

| Свойство | Тип                    | Описание
|:---------|:------------------------|:----------------------------------------
| id       | string                  | Уникальный идентификатор действия. Только для чтения.
| доступ   | [accessAction][]        | Был доступ к элементу.
| actor    | [identitySet][]         | Удостоверение, выполнившее действие. Только для чтения.
| activityDateTime    | DateTimeOffset | Сведения о том, когда было выполнено действие. Только для чтения.

[accessAction]: accessaction.md
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
  "@type.aka&quot;: &quot;oneDrive.activityEntity"
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

