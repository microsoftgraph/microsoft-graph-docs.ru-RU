---
title: тип ресурса sourceCollection
description: Представляет коллекцию электронных данных, которая обычно называется поиском.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 86ecf3adb64be2b216fdc167b29c10a850e25af6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447354"
---
# <a name="sourcecollection-resource-type"></a>тип ресурса sourceCollection

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет коллекцию электронных данных, которая обычно называется поиском. Дополнительные сведения [см. в материале Сбор данных по делу в advanced eDiscovery.](/microsoft-365/compliance/collecting-data-for-ediscovery)

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список sourceCollections](../api/ediscovery-case-list-sourcecollections.md)|[коллекция microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Получите список объектов **sourceCollection** и их свойств.|
|[Создание sourceCollection](../api/ediscovery-case-post-sourcecollections.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Создайте новый **объект sourceCollection.**|
|[Get sourceCollection](../api/ediscovery-sourcecollection-get.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Ознакомьтесь с свойствами и отношениями **объекта sourceCollection.**|
|[Обновление sourceCollection](../api/ediscovery-sourcecollection-update.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Обновление свойств объекта **sourceCollection.**|
|[Удаление sourceCollection](../api/ediscovery-sourcecollection-delete.md)|Нет|Удаление **объекта sourceCollection.**|
|[estimateStatistics](../api/ediscovery-sourcecollection-estimatestatistics.md)|Нет|Запустите оценку количества электронных писем и документов в коллекции исходных данных.|
|[Список дополнительныхSources](../api/ediscovery-sourcecollection-list-additionalsources.md)|[коллекция microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Получите список дополнительных объектов **dataSource,** связанных с исходным собранием.|
|[List custodianSources](../api/ediscovery-sourcecollection-list-custodiansources.md)|[коллекция microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Получите список дополнительных объектов **dataSource,** связанных с исходным собранием.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|contentQuery|String|Строка запроса в запросе KQL (Язык запросов ключевых слов). Подробные сведения см. в [статье Ключевые запросы и условия поиска для поиска контента и поиска электронных данных.](https://docs.microsoft.com/microsoft-365/compliance/keyword-queries-and-search-conditions)  Поиск можно уточнить с помощью полей в паре со значениями; например, *subject:"Quarterly Financials" AND Date>=06/01/2016 and Date<=07/01/2016*|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **sourceCollection.**|
|createdDateTime|DateTimeOffset|Дата и время создания **sourceCollection.**|
|description|String|Описание **sourceCollection**|
|displayName|String|Имя отображения **sourceCollection**|
|id|String| ID для **sourceCollection**. Только для чтения. |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Последний пользователь, который изменил **sourceCollection**.|
|lastModifiedDateTime|DateTimeOffset|Последняя дата и время изменения **sourceCollection.**|
|tenantSources|microsoft.graph.ediscovery.tenantSources|При указании коллекция будет охватывать всю службу для всей рабочей нагрузки. Возможные значения: `allMailboxes`, `allSites`.|

### <a name="tenantsources-values"></a>tenantSources значения

|Member|Описание|
|:----|-----------|
|allMailboxes| Включи все почтовые ящики в коллекцию. |
|allSites| Включай все сайты в коллекцию. |

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|additionalSources|[коллекция microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Добавляет дополнительный источник **в sourceCollection.**|
|addToReviewSetOperation|[microsoft.graph.ediscovery.addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md)|Добавляет результаты **sourceCollection в** указанный **обзорSet**.|
|custodianSources|[коллекция microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|**Источники custodian,** включенные в **sourceCollection.**|
|lastEstimateStatisticsOperation|[microsoft.graph.ediscovery.estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md)|Последняя операция оценки, связанная с **sourceCollection.**|

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
  "tenantSources": "String"
}
```
