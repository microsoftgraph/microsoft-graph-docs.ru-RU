---
title: Тип ресурса ediscoveryNoncustodialDataSource
description: Источники данных, не являясь хранителями, позволяют добавлять данные в дело без необходимости связывать их с хранителями.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 12b01d84aa5ce9642cc227bc192cb078f1484793
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839681"
---
# <a name="ediscoverynoncustodialdatasource-resource-type"></a>Тип ресурса ediscoveryNoncustodialDataSource

Пространство имен: microsoft.graph.security



Позволяет добавить данные в дело обнаружения электронных данных, не связывая их с хранителями. Дополнительные сведения см. в статье "Добавление источников данных, не теранимных" в дело обнаружения электронных данных [(цен. категория "Премиум"](/microsoft-365/compliance/non-custodial-data-sources)).


Наследуется [от dataSourceContainer](../resources/security-datasourcecontainer.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[List ediscoveryNoncustodialDataSources](../api/security-ediscoverysearch-list-noncustodialsources.md)|[Коллекция microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|Получение списка объектов [ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) и их свойств.|
|[Создание объекта ediscoveryNoncustodialDataSource](../api/security-ediscoverysearch-post-noncustodialsources.md)|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|Создайте объект [ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) .|
|[Get ediscoveryNoncustodialDataSource](../api/security-ediscoverynoncustodialdatasource-get.md)|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|Чтение свойств и связей объекта [ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) .|
|[updateIndex](../api/security-ediscoverynoncustodialdatasource-updateindex.md)|Нет|Активирует indexOperation, чтобы сделать источник данных, не связанный с хранением, и связанные источники данных доступны для поиска.|
|[Выпуска](../api/security-ediscoverynoncustodialdatasource-release.md)|Нет|Освобождение источника данных, не являемой хранителями, из дела.|
|[applyHold](../api/security-ediscoverynoncustodialdatasource-applyhold.md)|Нет|Запустите процесс применения удержания к источникам данных, не являымся источниками данных, не являмися хранителями.|
|[removeHold](../api/security-ediscoverynoncustodialdatasource-removehold.md)|Нет|Запустите процесс удаления удержания из источников данных, не охраняемых при обнаружении электронных данных.|
|[Перечисление ediscoveryIndexOperation](../api/security-ediscoverycustodian-list-lastindexoperation.md)|[Коллекция microsoft.graph.security.ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md)|Получение списка [объектов ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md) , связанных с [ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания объекта nonCustodialDataSource. Наследуется [от microsoft.graph.security.datasourcecontainer](../resources/security-datasourcecontainer.md).|
|displayName|Строка|Отображаемое имя noncustodialDataSource. Наследуется [от microsoft.graph.security.datasourcecontainer](../resources/security-datasourcecontainer.md).|
|id|Строка|Уникальный идентификатор объекта nonCustodialDataSource. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения nonCustodialDataSource. Наследуется [от microsoft.graph.security.datasourcecontainer](../resources/security-datasourcecontainer.md).|
|releasedDateTime|DateTimeOffset|Дата и время освобождения nonCustodialDataSource из дела. Наследуется [от microsoft.graph.security.datasourcecontainer](../resources/security-datasourcecontainer.md).|
|status|microsoft.graph.security.dataSourceContainerStatus|Последнее состояние nonCustodialDataSource. Наследуется [от microsoft.graph.security.datasourcecontainer](../resources/security-datasourcecontainer.md). Возможные значения: `Active`, `Released`.|
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|Состояние удержания nonCustodialDataSource.Возможные значения: `notApplied`, `applied`, `applying`, , `removing``partial`|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|Datasource|[microsoft.graph.security.dataSource](../resources/security-datasource.md)|Источник данных пользователя или источник данных сайта SharePoint в качестве источника данных, не являемого источником данных, не являемого хранителями.|
|lastIndexOperation|[microsoft.graph.security.ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md)|Сущность операции, представляющая последнее индексирование для источника данных, не являющееся источником данных, не являющееся хранителями.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryNoncustodialDataSource",
  "baseType": "microsoft.graph.security.dataSourceContainer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryNoncustodialDataSource",
  "id": "String (identifier)",
  "status": "String",
  "holdStatus": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```
