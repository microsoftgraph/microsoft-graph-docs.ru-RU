---
title: Тип ресурса Референцедобжект
description: Описывает ссылку на другой объект, определенный в том же определении каталога.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7779fb851812c00c15749877517b79273752ab58
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217593"
---
# <a name="referencedobject-resource-type"></a>Тип ресурса Референцедобжект

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает ссылку на другой объект, определенный в том же [определении каталога](synchronization-directorydefinition.md).

## <a name="properties"></a>Свойства

| Свойство                   | Тип                      | Описание    |
|:---------------------------|:--------------------------|:---------------|
|референцедобжектнаме        |String                     |Имя объекта, на который указывает ссылка. Должен сопоставлять один из объектов в [определении каталога](synchronization-directorydefinition.md).|
|референцедпроперти          |String                     |**В настоящее время не поддерживается**. Имя свойства в объекте, на который указывает ссылка, значение, которое используется в качестве ссылки.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referencedObject"
}-->

```json
{
  "referencedObjectName": "String",
  "referencedProperty": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
            
