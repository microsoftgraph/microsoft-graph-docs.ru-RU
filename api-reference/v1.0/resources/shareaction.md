---
author: daspek
title: тип ресурса shareAction
description: Объект shareAction предоставляет сведения о том, кому элемент был общим в действии общего обмена.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 65fc9fb0c9eb5aa71bc854f0fcfa25a6574898e0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126641"
---
# <a name="shareaction-resource-type"></a>тип ресурса shareAction

Пространство имен: microsoft.graph

Ресурс **shareAction** предоставляет сведения о [действии, которое][activity] разделяет элемент.

>**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

[activity]: itemactivity.md

## <a name="properties"></a>Свойства

| Имя свойства | Тип                       | Описание
|:--------------|:---------------------------|:-----------------------------
| recipients    | Коллекция [identitySet][] | Удостоверения, к которым был предоставлен доступ элементу в результате выполнения этого действия.

[identitySet]: identityset.md

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.shareAction"
}-->

```json
{
  "recipients": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The shareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/shareAction",
  "suppressions": []
}
-->

