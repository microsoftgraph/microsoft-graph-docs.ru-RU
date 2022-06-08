---
title: Тип ресурса ediscoveryReviewSet
description: Представляет статический набор хранимых в электронном виде сведений, собранных для использования в судебном процессе, расследовании или нормативных запросах.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 9c828a92d32e4d43d952c91e0820e575c3d2f59e
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946084"
---
# <a name="ediscoveryreviewset-resource-type"></a>Тип ресурса ediscoveryReviewSet

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет статический набор хранимых в электронном виде сведений, собранных для использования в судебном разбирательствах, расследованиях или нормативных запросах.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление ediscoveryReviewSets](../api/security-ediscoverycase-list-reviewsets.md)|[Коллекция microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|Получение списка объектов [ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md) и их свойств.|
|[Создание объекта ediscoveryReviewSet](../api/security-ediscoverycase-post-reviewsets.md)|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|Создайте объект [ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md) .|
|[Получение ediscoveryReviewSet](../api/security-ediscoveryreviewset-get.md)|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|Чтение свойств и связей объекта [ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md) .|
|[Экспорт](../api/security-ediscoveryreviewset-export.md)|Нет|Инициируйте экспорт данных из **набора проверок**.|
|[addToReviewSet](../api/security-ediscoveryreviewset-addtoreviewset.md)|Нет|Добавьте данные из **поиска обнаружения** электронных данных в **набор проверок**.|
|[Список файлов](../api/security-ediscoveryreviewset-list-files.md)|[Коллекция microsoft.graph.security.ediscoveryFile](../resources/security-ediscoveryfile.md)|Получите ресурсы ediscoveryFile из свойства навигации файлов.|
|[Перечисление запросов](../api/security-ediscoveryreviewset-list-queries.md)|[Коллекция microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|Получите ресурсы ediscoveryReviewSetQuery из свойства навигации запросов.|
|[Создание ediscoveryReviewSetQuery](../api/security-ediscoveryreviewset-post-queries.md)|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|Создайте объект ediscoveryReviewSetQuery.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[Microsoft.graph.identitySet](../resources/identityset.md)|Пользователь, создавший набор для проверки. Только для чтения. |
|createdDateTime|DateTimeOffset|Дата и время создания набора для проверки. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|displayName|Строка|Имя набора для проверки. Имя уникально с максимальным ограничением в 64 символа.|
|id|String|Уникальный идентификатор набора проверки. Только для чтения.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|files|[Коллекция microsoft.graph.security.ediscoveryFile](../resources/security-ediscoveryfile.md)|Представляет файлы в наборе для проверки.|
|Запросов|[Коллекция microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|Представляет запросы в наборе для проверки.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryReviewSet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryReviewSet",
  "id": "String (identifier)",
  "displayName": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)"
}
```

