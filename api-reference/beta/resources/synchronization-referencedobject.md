---
title: Тип ресурса Референцедобжект
description: Описывает ссылку на другой объект, определенный в том же определении каталога.
localization_priority: Normal
ms.openlocfilehash: 185691c970a5555d23b7b349cef546fb85be0893
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345609"
---
# <a name="referencedobject-resource-type"></a>Тип ресурса Референцедобжект

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает ссылку на другой объект, определенный в том же [определении каталога](synchronization-directorydefinition.md).

## <a name="properties"></a>Свойства

| Свойство                   | Тип                      | Описание    |
|:---------------------------|:--------------------------|:---------------|
|Референцедобжектнаме        |String                     |Имя объекта, на который указывает ссылка. Должен сопоставлять один из объектов в [определении каталога](synchronization-directorydefinition.md).|
|Референцедпроперти          |String                     |**В настоящее время не поддерживается**. Имя свойства в объекте, на который указывает ссылка, значение, которое используется в качестве ссылки.|

## <a name="json-representation"></a>Представление в формате JSON

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
            
