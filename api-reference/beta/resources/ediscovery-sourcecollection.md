---
title: тип ресурса sourceCollection
description: Представляет коллекцию электронных данных, которая обычно называется поиском.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: a67599c4a813e1ac7e354d1fd2b0c26c8eb366bb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101888"
---
# <a name="sourcecollection-resource-type"></a>тип ресурса sourceCollection

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет коллекцию электронных данных, которая обычно называется поиском. Дополнительные сведения см. в статье [Сбор данных для дела в Advanced eDiscovery](/microsoft-365/compliance/collecting-data-for-ediscovery).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Добавление additionalSource](../api/ediscovery-sourcecollection-post-additionalsources.md)|[коллекция microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Добавьте дополнительный **объект dataSource** в исходный набор.|
|[Добавление custodianSource](../api/ediscovery-sourcecollection-post-custodiansources.md)|[коллекция microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Добавьте объект **dataSource хранителя в** исходный набор.|
|[Добавление noncustodialSource](../api/ediscovery-sourcecollection-post-noncustodialsources.md)|[коллекция microsoft.graph.ediscovery.noncustodialSource](../resources/ediscovery-noncustodialdatasource.md)|Добавьте объект **noncustodialSource,** не отстойный для источника.|
|[Список sourceCollections](../api/ediscovery-case-list-sourcecollections.md)|[коллекция microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Получите список объектов **sourceCollection** и их свойств.|
|[Создание sourceCollection](../api/ediscovery-case-post-sourcecollections.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Создайте новый **объект sourceCollection.**|
|[Get sourceCollection](../api/ediscovery-sourcecollection-get.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Ознакомьтесь с свойствами и отношениями **объекта sourceCollection.**|
|[Обновление sourceCollection](../api/ediscovery-sourcecollection-update.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Обновление свойств объекта **sourceCollection.**|
|[Удаление sourceCollection](../api/ediscovery-sourcecollection-delete.md)|Нет|Удаление **объекта sourceCollection.**|
|[estimateStatistics](../api/ediscovery-sourcecollection-estimatestatistics.md)|Нет|Запустите оценку количества электронных писем и документов в коллекции исходных данных.|
|[Список дополнительныхSources](../api/ediscovery-sourcecollection-list-additionalsources.md)|[коллекция microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Получите список дополнительных объектов **dataSource,** связанных с исходным собранием.|
|[List custodianSources](../api/ediscovery-sourcecollection-list-custodiansources.md)|[коллекция microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Получите список объектов **custodian dataSource,** связанных с исходным собранием.|
|[Список noncustodialSources](../api/ediscovery-sourcecollection-list-noncustodialsources.md)|[коллекция microsoft.graph.ediscovery.noncustodialSource](../resources/ediscovery-noncustodialdatasource.md)|Получите список объектов **noncustodialSource,** связанных с коллекцией источников, не связанных с источниками.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|contentQuery|Строка|Строка запроса в запросе KQL (Язык запросов ключевых слов). Подробные сведения см. в [статье Ключевые запросы и условия поиска для поиска контента и поиска электронных данных.](/microsoft-365/compliance/keyword-queries-and-search-conditions) Поиск можно уточнить с помощью полей в паре со значениями; например, *subject:"Quarterly Financials" And Date>=06/01/2016 and Date<=07/01/2016*.|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **sourceCollection.**|
|createdDateTime|DateTimeOffset|Дата и время создания **sourceCollection.**|
|dataSourceScopes|microsoft.graph.ediscovery.dataSourceScopes|При указании коллекция будет охватывать всю службу для всей рабочей нагрузки. Возможные значения: `none`, `allTenantMailboxes`, `allTenantSites`, `allCaseCustodians`, `allCaseNoncustodialDataSources`.|
|description|String|Описание **sourceCollection**.|
|displayName|Строка|Имя отображения **sourceCollection**.|
|id|String| ID для **sourceCollection**. Только для чтения. |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Последний пользователь, который изменил **sourceCollection**.|
|lastModifiedDateTime|DateTimeOffset|Последняя дата и время изменения **sourceCollection.**|

### <a name="datasourcescopes-values"></a>значения dataSourceScopes

|Member|Описание|
|:----|-----------|
|Нет|Не укажите какие-либо области — расположения будут ссылаться отдельно.|
|allTenantMailboxes|Включи все почтовые ящики клиента в **sourceCollection.**|
|allTenantSites|Включи все сайты-клиенты **в sourceCollection.**|
|allCaseCustodians|Включай все расположения хранителей в **sourceCollection.**|
|allCaseNoncustodialDataSources|Включай в **sourceCollection** все неконтратные источники данных.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|additionalSources|[коллекция microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Добавляет дополнительный источник **в sourceCollection.**|
|addToReviewSetOperation|[microsoft.graph.ediscovery.addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md)|Добавляет результаты **sourceCollection в** указанный **обзорSet**.|
|custodianSources|[коллекция microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|**Источники custodian,** включенные в **sourceCollection.**|
|lastEstimateStatisticsOperation|[microsoft.graph.ediscovery.estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md)|Последняя операция оценки, связанная с **sourceCollection.**|
|noncustodialSources|[коллекция microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)|**noncustodialDataSource** источники, включенные в **sourceCollection**|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.sourceCollection",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.sourceCollection",
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