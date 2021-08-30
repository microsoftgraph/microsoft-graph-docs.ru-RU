---
title: Тип ресурса directoryObject
description: Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.
ms.localizationpriority: high
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e704c59e594095f45abd03ce48937c45cdcf6d30
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696416"
---
# <a name="directoryobject-resource-type"></a>Тип ресурса directoryObject

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.

Этот ресурс поддерживает:

- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryobject-delta.md)).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение объекта directoryObject](../api/directoryobject-get.md) | [directoryObject](directoryobject.md) |Чтение свойств объекта каталога.|
|[Удаление](../api/directoryobject-delete.md) | Нет |Удаление объекта каталога. |
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|Коллекция String|Проверка членства в списке групп. Это транзитивная проверка.|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|Коллекция строк|Возвращает все группы, в которых состоит пользователь, группа или объект каталога. Это транзитивная проверка.|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|Коллекция строк| Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная проверка. |
|[getByIds](../api/directoryobject-getbyids.md) | Коллекция [directoryObject](directoryobject.md) | Получение набора объектов каталога на основе указанных идентификаторов. |
|[validateProperties](../api/directoryobject-validateproperties.md)|Json| Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования. |
|[delta](../api/directoryobject-delta.md)|Коллекция [directoryObject](directoryobject.md)| Получение добавочных изменений для объектов каталога. Поддерживает фильтрацию по производному типу. |

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|String|Уникальный идентификатор объекта. Например, 12345678-9abc-def0-1234-56789abcde. Значение свойства **идентификатор** оформлено часто, но не всегда в виде GUID; необходимо считать его непрозрачным идентификатором и не полагаться на то, что он является GUID. Ключевое. Не допускается значение NULL. Только для чтения.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject",
  "openType": true
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


