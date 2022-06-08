---
title: Тип ресурса ediscoverySearch
description: Представляет поиск обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: d32540ccfd74f79fdad282f7d708a458bdf7705f
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946072"
---
# <a name="ediscoverysearch-resource-type"></a>Тип ресурса ediscoverySearch

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет поиск обнаружения электронных данных. Дополнительные сведения см [. в статье "Сбор данных для дела в службе обнаружения электронных данных (премиум)"](/microsoft-365/compliance/collecting-data-for-ediscovery).


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов ediscoverySearches](../api/security-ediscoverycase-list-searches.md)|[Коллекция microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Получение списка объектов [ediscoverySearch](../resources/security-ediscoverysearch.md) и их свойств.|
|[Создание ediscoverySearch](../api/security-ediscoverycase-post-searches.md)|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Создайте объект [ediscoverySearch](../resources/security-ediscoverysearch.md) .|
|[Получение ediscoverySearch](../api/security-ediscoverysearch-get.md)|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Чтение свойств и связей объекта [ediscoverySearch](../resources/security-ediscoverysearch.md) .|
|[Обновление ediscoverySearch](../api/security-ediscoverysearch-update.md)|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|Обновление свойств объекта [ediscoverySearch](../resources/security-ediscoverysearch.md) .|
|[Удаление ediscoverySearch](../api/security-ediscoverycase-delete-searches.md)|Нет|Удаляет объект [ediscoverySearch](../resources/security-ediscoverysearch.md) .|
|[estimateStatistics](../api/security-ediscoverysearch-estimatestatistics.md)|Нет|Выполните операцию оценки статистики для данных, содержащихся в поиске обнаружения электронных данных.|
|[purgeData](../api/security-ediscoverysearch-purgedata.md)|Нет|Выполните операцию очистки данных для данных Teams, содержащихся в поиске eDiscovery.|
|[Перечисление additionalSources](../api/security-ediscoverysearch-list-custodiansources.md)|[Коллекция microsoft.graph.security.dataSource](../resources/security-datasource.md)|Получите ресурсы dataSource из свойства навигации additionalSources.|
|[Создание источника данных](../api/security-ediscoverysearch-post-additionalsources.md)|[microsoft.graph.security.dataSource](../resources/security-datasource.md)|Создайте объект dataSource.|
|[List ediscoveryEstimateOperation](../api/security-ediscoverysearch-list-lastestimatestatisticsoperation.md)|[Коллекция microsoft.graph.security.ediscoveryEstimateOperation](../resources/security-ediscoveryestimateoperation.md)|Получите ресурсы ediscoveryEstimateOperation из свойства навигации lastEstimateStatisticsOperation.|
|[Перечисление объектов custodianSource](../api/security-ediscoverysearch-list-custodiansources.md)|[Коллекция microsoft.graph.security.dataSource](../resources/security-datasource.md)|Получение ресурсов dataSource из свойства навигации custodianSources.|
|[Добавление custodianSources](../api/security-ediscoverysearch-post-custodiansources.md)|[microsoft.graph.security.dataSource](../resources/security-datasource.md)|Добавьте custodianSources, выполнив публикацию в коллекции custodianSources.|
|[Удаление custodianSources](../api/security-ediscoverysearch-delete-custodiansources.md)|Нет|Удаление [объекта dataSource](../resources/security-datasource.md) .|
|[Перечисление noncustodialSources](../api/security-ediscoverysearch-list-noncustodialsources.md)|[Коллекция microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|Получите ресурсы ediscoveryNoncustodialDataSource из свойства навигации noncustodialSources.|
|[Добавление ediscoveryNoncustodialDataSource](../api/security-ediscoverysearch-post-noncustodialsources.md)|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|Добавьте noncustodialSources, выполнив публикацию в коллекции noncustodialSources.|
|[Удаление noncustodialSources](../api/security-ediscoverysearch-delete-noncustodialsources.md)|Нет|Удалите [объект ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|contentQuery|String|Строка запроса в запросе KQL (язык запросов ключевых слов). Дополнительные сведения см. в [запросах по ключевым словам и условиях поиска для поиска контента и обнаружения электронных данных](/microsoft-365/compliance/keyword-queries-and-search-conditions). Поиск можно уточнить с помощью полей, связанных со значениями; Например, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*.|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **поиск по обнаружению электронных данных**.|
|createdDateTime|DateTimeOffset|Дата и время создания **поиска eDiscovery** .|
|dataSourceScopes|microsoft.graph.ediscovery.dataSourceScopes|Если этот параметр указан, коллекция будет охватывать всю службу для всей рабочей нагрузки. Возможные значения: `none`, `allTenantMailboxes`, `allTenantSites`, `allCaseCustodians`, `allCaseNoncustodialDataSources`.|
|description|String|Описание поиска **eDiscovery**.|
|displayName|String|Отображаемое имя поиска **eDiscovery**.|
|id|String| Идентификатор для поиска **eDiscovery**. Только для чтения. |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Последний пользователь, который изменил **поиск по обнаружению электронных данных**.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения поиска **eDiscovery** .|

### <a name="datasourcescopes-values"></a>Значения dataSourceScopes

|Member|Описание|
|:----|-----------|
|Нет|Не указывайте области — ссылки на расположения будут указываться отдельно.|
|allTenantMailboxes|Включите все почтовые ящики клиента в поиск **по обнаружению электронных данных**.|
|allTenantSites|Включите все сайты клиентов в **поиск по обнаружению электронных данных**.|
|allCaseCustodians|Включите все расположения хранителей в поиск **по обнаружению электронных данных**.|
|allCaseNoncustodialDataSources|Включите все источники данных, не связанные с хранением, в поиск **eDiscovery**.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|additionalSources|[Коллекция microsoft.graph.security.dataSource](../resources/security-datasource.md)|Добавляет дополнительный источник в поиск **по обнаружению электронных данных**.|
|addToReviewSetOperation|[microsoft.graph.security.ediscoveryAddToReviewSetOperation](../resources/security-ediscoveryaddtoreviewsetoperation.md)|Добавляет результаты поиска **eDiscovery** в указанный **набор reviewSet**.|
|custodianSources|[Коллекция microsoft.graph.security.dataSource](../resources/security-datasource.md)|**Источники хранителей** , включенные в поиск **по обнаружению электронных данных**.|
|lastEstimateStatisticsOperation|[microsoft.graph.security.ediscoveryEstimateOperation](../resources/security-ediscoveryestimateoperation.md)|Последняя операция оценки, связанная с **поиском обнаружения электронных данных**.|
|noncustodialSources|[Коллекция microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|**Источники noncustodialDataSource** , включенные в поиск **eDiscovery**|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoverySearch",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoverySearch",
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
  "contentQuery": "String",
  "dataSourceScopes": "String"
}
```