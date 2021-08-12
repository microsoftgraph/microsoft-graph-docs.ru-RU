---
author: daspek
title: Тип ресурса versionAction
description: Объект VersionAction предоставляет сведения о действии, которое привело к новой версии элемента.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: bb1061e09b78a2069b1182811573564804b25d9dfe7d1f8dced0cfb55e62e5dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129885"
---
# <a name="versionaction-resource-type"></a>Тип ресурса versionAction

Пространство имен: microsoft.graph

Наличие ресурса **versionAction** в [**itemActivity**][activity] указывает на то, что действие привело к создания новой версии.

>**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

[activity]: itemactivity.md

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание
|:--------------|:-------|:----------------------------------------------------
| newVersion    | string | Имя новой версии, созданной при выполнении этого действия.

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.versionAction"
}-->

```json
{
  "newVersion&quot;: &quot;string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction",
  "suppressions": []
}
-->

