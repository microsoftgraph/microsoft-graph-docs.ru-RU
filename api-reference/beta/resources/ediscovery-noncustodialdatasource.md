---
title: тип ресурса noncustodialDataSource
description: Неконтлиционные источники данных позволяют добавлять данные в дело, не связывая их с хранителями
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 1e7dd0d656a58e65e460742158cdcc70da1f1d5a
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080908"
---
# <a name="noncustodialdatasource-resource-type"></a>тип ресурса noncustodialDataSource

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Источники данных, не имеющие содержания под стражей, могут добавлять данные в дело, не связывая их с хранителями. Дополнительные сведения можно получить на [сайте Add non-custodial data sources to an Advanced eDiscovery case](https://docs.microsoft.com/microsoft-365/compliance/non-custodial-data-sources)

Наследует [от dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список noncustodialDataSources](../api/ediscovery-noncustodialdatasource-list.md)|[коллекция microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)|Получите список объектов [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) и их свойств.|
|[Получить noncustodialDataSource](../api/ediscovery-noncustodialdatasource-get.md)|[microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)|Ознакомьтесь с свойствами и отношениями [объекта noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)|
|[Release dataSource](../api/ediscovery-noncustodialdatasource-release.md)|Нет|Освобождает источник данных, не относясь к данным, не относяся к опеке.|
|[List dataSource](../api/ediscovery-noncustodialdatasource-list-datasource.md)|[коллекция microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Получите ресурсы dataSource из свойства навигации dataSource.|
|[Создание dataSource](../api/ediscovery-noncustodialdatasource-post.md)|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Создание нового объекта dataSource.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|applyHoldToSource|Boolean|Указывает, применяется ли удержание к источнику данных без хранения (например, к почтовому ящику или сайту).|
|createdDateTime|DateTimeOffset|Создана дата и время nonCustodialDataSource. Наследуется [от microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|displayName|String|Отображение имени noncustodialDataSource. Наследуется [от microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|id|String|Уникальный идентификатор nonCustodialDataSource. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Последняя измененная дата и время nonCustodialDataSource. Наследуется [от microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|releasedDateTime|DateTimeOffset|Дата и время освобождения nonCustodialDataSource из дела. Наследуется [от microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|status|microsoft.graph.ediscovery.dataSourceContainerStatus|Последний статус nonCustodialDataSource. Наследуется [от microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md). Возможные значения: `Active`, `Released`.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|dataSource|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Источник данных пользователя или SharePoint в качестве источника данных, не в качестве источника данных, не в виде хранения.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource",
  "baseType": "microsoft.graph.ediscovery.dataSourceContainer",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.noncustodialDataSource",
  "id": "String (identifier)",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "applyHoldToSource": "Boolean"
}
```
