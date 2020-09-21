---
title: Тип ресурса Референцедобжект
description: Описывает ссылку на другой объект, определенный в том же определении каталога.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9ea400e40074b30943412cf7b5fbae75f9037ca1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023896"
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
            


