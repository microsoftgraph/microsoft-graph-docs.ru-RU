---
title: Тип ресурса referencedObject
description: Описывает ссылку на другой объект, определенных в одно и то же определение каталога.
ms.openlocfilehash: 63645048fd8ba6ad949da43baa261b2842ea4016
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082039"
---
# <a name="referencedobject-resource-type"></a>Тип ресурса referencedObject

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Описывает ссылку на другой объект, определенных в одно и то же [Определение каталога](synchronization-directorydefinition.md).

## <a name="properties"></a>Свойства

| Свойство                   | Тип                      | Description    |
|:---------------------------|:--------------------------|:---------------|
|referencedObjectName        |String                     |Имя объекта, на который указывает ссылка. Должно соответствовать одному из объектов в [каталоге определения](synchronization-directorydefinition.md).|
|referencedProperty          |String                     |**В настоящее время не поддерживается**. Имя свойства в этом объекте, значение которой используется в качестве ссылки.|

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
<!-- {
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
            