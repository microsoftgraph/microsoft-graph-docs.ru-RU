---
title: Тип ресурса Референцедобжект
description: Описывает ссылку на другой объект, определенный в том же определении каталога.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c1c7e1554764031efbfa3a5d1c1280f4b72bc160
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007860"
---
# <a name="referencedobject-resource-type"></a>Тип ресурса Референцедобжект

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает ссылку на другой объект, определенный в том же [определении каталога](synchronization-directorydefinition.md).

## <a name="properties"></a>Свойства

| Свойство                   | Тип                      | Описание    |
|:---------------------------|:--------------------------|:---------------|
|Референцедобжектнаме        |String                     |Имя объекта, на который указывает ссылка. Должен сопоставлять один из объектов в [определении каталога](synchronization-directorydefinition.md).|
|Референцедпроперти          |String                     |**В настоящее время не поддерживается**. Имя свойства в объекте, на который указывает ссылка, значение, которое используется в качестве ссылки.|

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
            
