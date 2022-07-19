---
title: Тип ресурса ediscoveryExportOperation
description: Представляет процесс экспорта обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 14a4d85e2efada576b3e0d8ff9bc0a1bdfe64cf6
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838628"
---
# <a name="ediscoveryexportoperation-resource-type"></a>Тип ресурса ediscoveryExportOperation

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет процесс экспорта обнаружения электронных данных.

Наследуется от [caseOperation](../resources/security-caseoperation.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[getDownloadUrl](../api/security-ediscoveryexportoperation-getdownloadurl.md)|String| Возвращает URL-адрес для экспорта.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|[microsoft.graph.security.caseAction](../resources/security-caseoperation.md#caseaction-values)| Тип действия, представляемого операцией. Возможные значения: `addToReviewSet`,,,`contentExport`,`convertToPdf``estimateStatistics``applyTags`,`purgeData`|
|azureBlobContainer|Строка| Имя расположения хранилища Azure, в котором будет храниться экспорт. Это относится только к экспортам, хранящимся в вашем собственном хранилище Azure. |
|azureBlobToken|String| Маркер SAS для расположения хранилища Azure.  Это относится только к экспортам, хранящимся в вашем собственном хранилище Azure. |
|completedDateTime|DateTimeOffset| Дата и время завершения экспорта.|
|createdBy|[identitySet](../resources/identityset.md)| Пользователь, иницивший операцию экспорта.|
|createdDateTime|DateTimeOffset| Дата и время создания экспорта.|
|description|String| Описание, предоставленное для экспорта.|
|exportOptions|microsoft.graph.security.exportOptions| Параметры, предоставленные для экспорта. Дополнительные сведения см. в [разделе reviewSet: export](../api/security-ediscoveryreviewset-export.md). Возможные значения: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.|
|exportStructure|microsoft.graph.security.exportFileStructure|Предоставленные параметры, указывающие структуру экспорта. Дополнительные сведения см. в [разделе reviewSet: export](../api/security-ediscoveryreviewset-export.md). Возможные значения: `none`, `directory`, `pst`.|
|id|String| Идентификатор операции. Только для чтения. |
|outputName|Строка| Имя, указанное для экспорта.|
|percentProgress|Int32| Ход выполнения операции.|
|resultInfo|[resultInfo](../resources/resultinfo.md)|Содержит сведения о результатах успешного выполнения и сбоя. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|status|[microsoft.graph.security.caseOperationStatus](../resources/security-caseoperation.md#caseoperationstatus-values)| Состояние операции обращения. Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

### <a name="exportoptions-values"></a>Значения exportOptions

|Member|Описание|
|:----|-----------|
|originalFiles|Включите исходные файлы в собственном формате. Например: docx, xlsx, pptx, doc, xlst, pptm и т. д.|
|текст|Включите извлеченный текст из исходных файлов.|
|pdfReplacement|Замените исходный файл версией PDF, если она доступна.|
|Fileinfo|Включите метаданные исходных файлов в загрузочный файл.|
|tags|Включите сведения о теге в fileInfo.|

### <a name="exportfilestructure-values"></a>Значения exportFileStructure

|Member|Описание|
|:----|-----------|
|Нет|Структура файла по умолчанию.|
|Каталог|Все файлы в папке singe с именем NativeFiles.|
|Pst|Сообщения будут сгруппироваться в формате pst.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|reviewSet|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|    Набор для проверки, из которого экспортируются документы.|
|reviewSetQuery|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|Запрос набора для проверки, используемый для фильтрации документов для экспорта.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryExportOperation",
  "baseType": "microsoft.graph.security.caseOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryExportOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "percentProgress": "Integer",
  "status": "String",
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

