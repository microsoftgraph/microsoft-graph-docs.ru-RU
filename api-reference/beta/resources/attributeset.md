---
title: Тип ресурса attributeSet
description: Объект, который представляет группу связанных пользовательских определений атрибутов безопасности.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 958ecbd900a98cfe9f91bf5d7fe526b2f4050bfa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077157"
---
# <a name="attributeset-resource-type"></a>Тип ресурса attributeSet

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект, который представляет группу связанных пользовательских определений атрибутов безопасности.

В клиенте можно определить до 500 `attributeSet` объектов. Нельзя переименовать или удалить.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Атрибуты listSets](../api/directory-list-attributesets.md)|[коллекция attributeSet](../resources/attributeset.md)|Получите список объектов [attributeSet](../resources/attributeset.md) и их свойств.|
|[Get attributeSet](../api/attributeset-get.md)|[attributeSet](../resources/attributeset.md)|Ознакомьтесь с свойствами и отношениями объекта [attributeSet.](../resources/attributeset.md)|
|[Создание attributeSet](../api/directory-post-attributesets.md)|[attributeSet](../resources/attributeset.md)|Создайте новый [объект attributeSet.](../resources/attributeset.md)|
|[Update attributeSet](../api/attributeset-update.md)|[attributeSet](../resources/attributeset.md)|Обновление свойств объекта [attributeSet.](../resources/attributeset.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|Описание набора атрибутов. Может иметь длину до 128 символов и включать символы Unicode. Можно изменить позже.|
|id|String|Идентификатор для уникального набора атрибутов в клиенте. Может иметь длину до 32 символов и включать символы Unicode. Не может содержать пробелы или специальные символы. Не удается изменить позже. Случай нечувствительный.|
|maxAttributesPerSet|Int32|Максимальное количество пользовательских атрибутов безопасности, которые можно определить в этом наборе атрибутов. Значение по умолчанию — `null`. Если не указано, администратор может добавить не более 500 активных атрибутов на каждого клиента. Можно изменить позже.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attributeSet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attributeSet",
  "description": "String",
  "id": "String (identifier)",
  "maxAttributesPerSet": "Integer"
}
```
