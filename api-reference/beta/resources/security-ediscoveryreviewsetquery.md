---
title: Тип ресурса ediscoveryReviewSetQuery
description: Представляет запрос набора для проверки, который используется для запроса и кэширования данных, хранящихся в наборе проверки обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 1fd3a579783929eb587055ad4ff0c2a7d6d222ec
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838243"
---
# <a name="ediscoveryreviewsetquery-resource-type"></a>Тип ресурса ediscoveryReviewSetQuery

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запрос набора для проверки, который используется для запроса и кэширования данных, хранящихся в наборе проверки [обнаружения электронных данных](security-ediscoveryreviewset.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление ediscoveryReviewSetQueries](../api/security-ediscoveryreviewset-list-queries.md)|[Коллекция microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|Получение списка объектов [ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) и их свойств.|
|[Создание ediscoveryReviewSetQuery](../api/security-ediscoveryreviewset-post-queries.md)|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|Создайте объект [ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) .|
|[Получение ediscoveryReviewSetQuery](../api/security-ediscoveryreviewsetquery-get.md)|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|Чтение свойств и связей объекта [ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) .|
|[Обновление ediscoveryReviewSetQuery](../api/security-ediscoveryreviewsetquery-update.md)|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|Обновление свойств объекта [ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) .|
|[Удаление ediscoveryReviewSetQuery](../api/security-ediscoveryreviewset-delete-queries.md)|Нет|Удаление объекта [ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) .|
|[Экспорт](../api/security-ediscoveryreviewsetquery-export.md)|Нет|Экспорт документов, соответствующих указанному запросу, из набора для проверки.|
|[applyTags](../api/security-ediscoveryreviewsetquery-applytags.md)|Нет|Примените теги к документам, которые соответствуют указанному запросу.|
|[Запустить](../api/security-ediscoveryreviewsetquery-run.md)|[Коллекция microsoft.graph.security.ediscoveryFile](../resources/security-ediscoveryfile.md)|Получение файлов из запроса.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| createdBy | [identitySet](/graph/api/resources/identityset) | Пользователь, создавший запрос. |
| createdDateTime |DateTimeOffset| Время и дата создания запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
| displayName | Строка | Имя запроса.|
| id |String| Уникальный идентификатор запроса. Только для чтения.|
| lastModifiedBy | [identitySet](/graph/api/resources/identityset) | Пользователь, который последним изменил запрос. |
| lastModifiedDateTime |DateTimeOffset | Дата и время последнего изменения запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
| Запрос | String | Строка запроса в запросе KQL (язык запросов ключевых слов). Дополнительные сведения см[. в полях метаданных документа в eDiscovery (Premium).](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)  Это поле сопоставляется непосредственно с условием ключевых слов.  Поиск можно уточнить с помощью полей, перечисленных в имени поля *, доступного для* поиска, в паре со значениями. Например, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*. |


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryReviewSetQuery",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryReviewSetQuery",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "contentQuery": "String"
}
```

