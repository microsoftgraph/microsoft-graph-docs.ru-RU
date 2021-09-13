---
author: daspek
title: Тип ресурса versionAction
description: Объект VersionAction предоставляет сведения о действии, которое привело к новой версии элемента.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4fbeb09d0fd2f209d436578e29ae7bf1fd404c3c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139556"
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

