---
title: Тип ресурса ediscoveryReviewTag
description: Представляет тег обнаружения электронных данных, который используется для пометки документов во время проверки, чтобы разделять адаптивный и неотвечивый контент.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 88f3a0a5590f0ebc7307b72cc47093a68f94fc9f
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839651"
---
# <a name="ediscoveryreviewtag-resource-type"></a>Тип ресурса ediscoveryReviewTag

Пространство имен: microsoft.graph.security



Представляет тег обнаружения электронных данных, который используется для пометки документов во время проверки для разделения адаптивного и неавторизованного содержимого.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление ediscoveryReviewTags](../api/security-ediscoverycase-list-tags.md)|[Коллекция microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Получение списка объектов [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) и их свойств.|
|[Создание ediscoveryReviewTag](../api/security-ediscoverycase-post-tags.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Создайте объект [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) .|
|[Получение ediscoveryReviewTag](../api/security-ediscoveryreviewtag-get.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Чтение свойств и связей объекта [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) .|
|[Обновление ediscoveryReviewTag](../api/security-ediscoveryreviewtag-update.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Обновление свойств объекта [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) .|
|[Удаление ediscoveryReviewTag](../api/security-ediscoverycase-delete-tags.md)|Нет|Удаление объекта [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) .|
|[asHierarchy](../api/security-ediscoveryreviewtag-ashierarchy.md)|[Коллекция microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Перечисление тегов, упорядоченных как иерархия.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|childSelectability|microsoft.graph.security.childSelectability|Указывает, может ли один или несколько дочерних тегов быть связаны с документом. Возможные значения: `One`, `Many`.  Это значение определяет, представляет ли пользовательский интерфейс теги как флажки или группу переключателей.|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший тег.|
|description|String|Описание тега.|
|displayName|Строка|Отображаемое имя тега.|
|id|String|Уникальный идентификатор тега.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения тега.|

### <a name="childselectability-values"></a>Значения childSelectability

|Member|Описание|
|:----|-----------|
|Одной|Можно выбрать только один дочерний элемент. Это соответствует пользовательскому интерфейсу, который представляет теги с переключатели.|
|Много|Можно выбрать ноль или много дочерних элементов. Это соответствует пользовательскому интерфейсу, который представляет теги с флажками.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|childTags|[Коллекция microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Возвращает теги, которые являются дочерними для тега.|
|родитель|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Возвращает родительский тег указанного тега.|
## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryReviewTag",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryReviewTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "childSelectability": "String"
}
```

