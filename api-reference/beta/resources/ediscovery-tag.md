---
title: Тип ресурса тегов
description: Представляет тег eDiscovery, который используется для маркировки документов во время проверки для отдельного отзывчивого и не отзывчивого контента.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: dee53c5a7d8320822101addcf5764420456e703f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447551"
---
# <a name="tag-resource-type"></a>Тип ресурса тегов

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тег eDiscovery, который используется для маркировки документов во время проверки, чтобы разделять отзывчивый и не отзывчивый контент.

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Теги списка](../api/ediscovery-case-list-tags.md)|[коллекция microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Получите список объектов **тегов** и их свойств.|
|[Создание тега](../api/ediscovery-case-post-tags.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Создайте новый **объект тегов.**|
|[Получить тег](../api/ediscovery-tag-get.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Ознакомьтесь с свойствами и отношениями объекта **тегов.**|
|[Тег обновления](../api/ediscovery-tag-update.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Обновление свойств объекта **тегов.**|
|[Удаление тега](../api/ediscovery-tag-delete.md)|Нет|Удаление объекта **тега.**|
|[asHierarchy](../api/ediscovery-tag-ashierarchy.md)|[коллекция microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Списки всех тегов, включая их иерархию.|
|[Список childTags](../api/ediscovery-tag-childtags.md)|[коллекция microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Получите список объектов детских **тегов,** связанных с тегом.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|childSelectability|[microsoft.graph.ediscovery.childSelectability](../resources/ediscovery-tag.md#childselectability-values)|Указывает, можно ли связывать один или несколько детских тегов с документом. Возможные значения: `One`, `Many`.  Это значение контролирует, представляет ли UX теги в качестве почтовых ящиков или группы кнопок радио.|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший тег.|
|description|String|Описание тега.|
|displayName|String|Отображение имени тега.|
|id|String|Уникальный идентификатор тега.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения тега.|

### <a name="childselectability-values"></a>значения childSelectability

|Member|Описание|
|:----|-----------|
|Один|Можно выбрать только одного ребенка. Это соответствует пользовательскому интерфейсу, который представляет теги с кнопками радио.|
|Многие|Ноль или много детей могут быть выбраны. Это соответствует пользовательскому интерфейсу, который представляет теги с почтовыми ящиками.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|childTags|[коллекция microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Возвращает теги, которые являются ребенком тега.|
|родитель|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Возвращает родительский тег указанного тега.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.tag",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.tag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "childSelectability": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```
