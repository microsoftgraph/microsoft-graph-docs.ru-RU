---
title: тип ресурса caseExportOperation
description: Представляет процесс экспорта электронных открытий.
ms.localizationpriority: medium
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c3f69f459aec067608f350daddb5892b5e9ec06b
ms.sourcegitcommit: f9e71d3b8a54a98c282ef49783babe5698300c06
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2021
ms.locfileid: "60793906"
---
# <a name="caseexportoperation-resource-type"></a>тип ресурса caseExportOperation

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет процесс экспорта электронных открытий. The **caseExportOperation** can only be retrieved from the `Location` header in the response to a [reviewset export.](../api/ediscovery-reviewset-export.md)

Наследует [от caseOperation](../resources/ediscovery-caseoperation.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[getDownloadUrl](../api/ediscovery-caseexportoperation-getdownloadurl.md)|Строка| Возвращает URL-адрес для экспорта.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|action|[microsoft.graph.ediscovery.caseAction](../resources/ediscovery-caseoperation.md#caseaction-values)| Действие случая для этой сущности всегда будет `contentExport` . Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|azureBlobContainer|Строка| Имя расположения хранилища Azure, в котором будет храниться экспорт. Это относится только к экспорту, хранямуся в вашем собственном хранилище Azure. |
|azureBlobToken|Строка| Маркер SAS для хранилища Azure.  Это относится только к экспорту, хранямуся в вашем собственном хранилище Azure. |
|completedDateTime|DateTimeOffset| Дата и время завершения экспорта.  Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|createdBy|[identitySet](../resources/identityset.md)| Пользователь, который инициировал экспортную операцию. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|createdDateTime|DateTimeOffset| Дата и время создания экспорта. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|description|Строка| Описание, предоставленное для экспорта. |
|ExportOptions|microsoft.graph.ediscovery.exportOptions| Параметры, предусмотренные для экспорта. Дополнительные сведения см. [в обзореSet: экспорт.](../api/ediscovery-reviewset-export.md) Возможные значения: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.|
|exportStructure|microsoft.graph.ediscovery.exportFileStructure|Параметры, которые указывают структуру экспорта. Дополнительные сведения см. [в обзореSet: экспорт.](../api/ediscovery-reviewset-export.md) Возможные значения: `none`, `directory`, `pst`.|
|id|String| ID для операции. Только для чтения. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|outputName|Строка| Имя, предоставленное для экспорта.|
|percentProgress|Int32| Ход операции. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|resultInfo|[resultInfo](../resources/resultinfo.md)|Содержит сведения о результатах, характерных для успешного и неудачного сбоя. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|status|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|Состояние операции дела. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md). Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

### <a name="exportoptions-values"></a>Значения exportOptions

|Member| Описание |
|:---|:---|
|originalFiles| Включай копии исходных файлов — исключить этот параметр только при создании отчетов. |
|текст| Включай необработанные извлеченные текстовые файлы для каждого документа. |
|pdfReplacement| Если во время проверки создаются отредактированные PDF-файлы, эти файлы доступны для экспорта. Вы можете экспортировать отредактировали PDFs вместо исходных родных файлов, включив этот параметр. |
|fileInfo| Включай сводку и файл нагрузки — это всегда должно быть включено. |
|tags| Включай теги документов, которые были применены во время проверки в файле нагрузки. |

### <a name="exportfilestructure-values"></a>значения exportFileStructure

|Member| Описание |
|:---|:---|
|каталог| Карты к структуре сгущенных каталогов, обычно используемой средствами eDiscovery. Все файлы экспортируются в корневой файл под названием NativeFiles. |
|pST| Сообщения электронной почты хранятся в PSTs, а документы с сайтов хранятся в папках, которые представляют исходную структуру папки. |

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|reviewSet|[microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md)| В обзоре установлено, из него экспортируется контент. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.caseExportOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.caseExportOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "percentProgress": "Integer",
  "status": "String",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  },
  "outputName": "String",
  "description": "String",
  "outputFolderId": "String",
  "azureBlobContainer": "String",
  "azureBlobToken": "String",
  "exportOptions": "String",
  "exportStructure": "String"
}
```
