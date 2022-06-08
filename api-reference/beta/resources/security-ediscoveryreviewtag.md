---
title: Тип ресурса ediscoveryReviewTag
description: Представляет тег обнаружения электронных данных, который используется для пометки документов во время проверки, чтобы разделять адаптивный и неотвечивый контент.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 1e5ba6fecb006a270d256e0f53f63e643874cec4
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946079"
---
# <a name="ediscoveryreviewtag-resource-type"></a>Тип ресурса ediscoveryReviewTag

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тег обнаружения электронных данных, который используется для пометки документов во время проверки для разделения адаптивного и неавторизованного содержимого.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление ediscoveryReviewTags](../api/security-ediscoverycase-list-tags.md)|[Коллекция microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Получение списка объектов [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) и их свойств.|
|[Создание ediscoveryReviewTag](../api/security-ediscoverycase-post-tags.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Создайте объект [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) .|
|[Получение ediscoveryReviewTag](../api/security-ediscoveryreviewtag-get.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Чтение свойств и связей объекта [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) .|
|[Обновление ediscoveryReviewTag](../api/security-ediscoveryreviewtag-update.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Обновление свойств объекта [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) .|
|[Удаление ediscoveryReviewTag](../api/security-ediscoverycase-delete-tags.md)|Нет|Удаляет объект [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) .|
|[asHierarchy](../api/security-ediscoveryreviewtag-ashierarchy.md)|[Коллекция microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Перечисление тегов, упорядоченных как иерархия.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|childSelectability|Строка|Указывает, может ли один или несколько дочерних тегов быть связаны с документом. Возможные значения: `One`, `Many`.  Это значение определяет, представляет ли пользовательский интерфейс теги как флажки или группу переключателей.|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший тег.|
|description|Строка|Описание тега.|
|displayName|String|Отображаемое имя тега.|
|id|Строка|Уникальный идентификатор тега.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения тега.|

### <a name="childselectability-values"></a>Значения childSelectability

|Member|Описание|
|:----|-----------|
|Одной|Можно выбрать только один дочерний элемент. Это соответствует пользовательскому интерфейсу, который представляет теги с переключатели.|
|Много|Можно выбрать ноль или много дочерних элементов. Это соответствует пользовательскому интерфейсу, который представляет теги с флажками.|

## <a name="relationships"></a>Отношения

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

