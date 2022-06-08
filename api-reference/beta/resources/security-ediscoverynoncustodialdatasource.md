---
title: Тип ресурса ediscoveryNoncustodialDataSource
description: Источники данных, не являясь хранителями, позволяют добавлять данные в дело без необходимости связывать их с хранителями.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: fcf2022747ee7b98526d522eecc268be2def490d
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946092"
---
# <a name="ediscoverynoncustodialdatasource-resource-type"></a>Тип ресурса ediscoveryNoncustodialDataSource

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Источники данных, не являясь хранителями, позволяют добавлять данные в дело без необходимости связывать их с хранителями. Дополнительные сведения см. в статье ["Добавление неохраняемого источника данных в дело advanced eDiscovery"](/microsoft-365/compliance/non-custodial-data-sources).


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
|[Перечисление ediscoveryIndexOperation](../api/security-ediscoverycustodian-list-lastindexoperation.md)|[Коллекция microsoft.graph.security.ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md)|Получите ресурсы ediscoveryIndexOperation из свойства навигации lastIndexOperation.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания объекта nonCustodialDataSource. Наследуется [от microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|displayName|Строка|Отображаемое имя noncustodialDataSource. Наследуется [от microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|id|Строка|Уникальный идентификатор объекта nonCustodialDataSource. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения nonCustodialDataSource. Наследуется [от microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|releasedDateTime|DateTimeOffset|Дата и время освобождения nonCustodialDataSource из дела. Наследуется [от microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).|
|status|String|Последнее состояние nonCustodialDataSource. Наследуется [от microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md). Возможные значения: `Active`, `Released`.|
|holdStatus|String|Состояние удержания nonCustodialDataSource.Возможные значения: `notApplied`, `applied`, `applying`, , `removing``partial`|

## <a name="relationships"></a>Отношения
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