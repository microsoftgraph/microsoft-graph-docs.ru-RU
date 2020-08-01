---
title: задать тип ресурса
description: Представляет набор в банке терминов.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5e74e0a603d088c7964b13fad51018171642c6ec
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539387"
---
# <a name="set-resource-type"></a>задать тип ресурса

Пространство имен: Microsoft. Graph. банка

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет набор, используемый в [банке]терминов. Набор представляет единицу измерения, которая содержит коллекцию иерархических терминов. [Группа] может содержать несколько наборов.

Наследуется от [объекта Entity](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Наборы списков](../api/termstore-group-list-sets.md)|Коллекция [Microsoft. Graph. банка. Set] | Возвращает список наборов, содержащихся в [группе] [банка] терминов. |
|[Создание набора](../api/termstore-set-post.md)|[Microsoft. Graph. банка. Set](../resources/termstore-set.md)|Создайте новый объект set в [банке]терминов.|
|[Создание термина](../api/termstore-term-post.md)|[Microsoft. Graph. Банк. Term](../resources/termstore-term.md)|Создайте новый объект [Term] в [банке]терминов.|
|[Получение набора](../api/termstore-set-get.md)|[Microsoft. Graph. банка. Set](../resources/termstore-set.md)| Получение объекта Set в [банке]терминов.|
|[Получение термина](../api/termstore-term-get.md)|[Microsoft. Graph. Банк. Term](../resources/termstore-term.md)| Получение объекта [Term] в [банке]терминов.|
|[Набор обновлений](../api/termstore-set-update.md)|[Microsoft. Graph. банка. Set](../resources/termstore-set.md)|Обновление свойств объекта Set в [банке]терминов.|
|[Удаление набора](../api/termstore-set-delete.md)|Нет|Удаляет объект set в [банке]терминов.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания набора. Только для чтения.|
|description|String|Описание, содержащее сведения об использовании терминов.|
|id|Строка|Уникальный идентификатор. Только для чтения.|
|локализеднамес|Коллекция [Microsoft. Graph. банка Microsoft. Graph. локализеднаме](../resources/termstore-localizedname.md)|Имя набора для каждого Лангуажетаг.|
|properties|Коллекция [Microsoft. Graph. ключзначение](../resources/keyvalue.md)|Настраиваемые свойства для набора.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|children|Коллекция [Microsoft. Graph. Банк терминов Microsoft. Graph.](../resources/termstore-term.md)|Дочерние термины набора в [банке]терминов.|
|парентграуп|[Microsoft. Graph. Банк.](../resources/termstore-group.md)|Родительская [Группа] , содержащая набор.|
|отношениях|Коллекция [Microsoft. Graph. Банк. relation](../resources/termstore-relation.md)|Указывает, какие термины были закреплены или повторно использованы непосредственно в наборе.|
|терм|Коллекция [Microsoft. Graph. Банк терминов Microsoft. Graph.](../resources/termstore-term.md)|Все термины в наборе.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.set",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.set",
  "id": "String (identifier)",
  "localizedNames": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedName"
    }
  ],
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "properties": [
    {
      "@odata.type": "microsoft.graph.termStore.keyValue"
    }
  ]
}
```

[microsoft.graph.termStore.term]: termstore-term.md
[Microsoft. Graph. банка. Set]: termstore-set.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.relation]: termstore-relation.md
[microsoft.graph.termStore.store]: termstore-store.md
[microsoft.graph.termStore.localizedName]: termstore-localizedname.md
[восстановлен]: ../resources/termstore-store.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
[банком]: ../resources/termstore-term.md


<!--
{
  "type": "#page.annotation",
  "description": "TermSet is the entity containing the particular taxonomy for a tenant",
  "keywords": "termSet,facet,resource",
  "section": "documentation",
  "tocPath": "TermSet",
  "tocBookmarks": {
    "Resources/termStore.set": "#"
  },
  "suppressions": []
}
-->
