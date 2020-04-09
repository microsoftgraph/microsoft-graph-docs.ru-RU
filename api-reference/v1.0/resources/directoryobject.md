---
title: Тип ресурса directoryObject
description: Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.
localization_priority: Priority
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8014c238487d5ada0f05f1a6edfed0402b25ae1a
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181869"
---
# <a name="directoryobject-resource-type"></a>Тип ресурса directoryObject

Пространство имен: microsoft.graph

Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение объекта directoryObject](../api/directoryobject-get.md) | [directoryObject](directoryobject.md) |Чтение свойств объекта каталога.|
|[Удаление объекта directoryObject](../api/directoryobject-delete.md) | Нет |Удаление объекта каталога. |
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|Коллекция строк|Проверка членства в списке групп. Это транзитивная проверка.|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|Коллекция строк|Возвращает все группы, в которых состоит пользователь, группа или объект каталога. Это транзитивная проверка.|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|Коллекция строк| Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная проверка. |
|[getByIds](../api/directoryobject-getbyids.md) | Коллекция [directoryObject](directoryobject.md) | Получение набора объектов каталога на основе указанных идентификаторов. |
|[validateProperties](../api/directoryobject-validateproperties.md)|Json| Проверка соответствия отображаемого имени или почтового псевдонима группы Office 365 политикам именования. |

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|String|Уникальный идентификатор GUID объекта, например 12345678-9abc-def0-1234-56789abcde. Ключ. Значение null не допускается. Только для чтения.|

## <a name="relationships"></a>Связи

Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directoryObject",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
