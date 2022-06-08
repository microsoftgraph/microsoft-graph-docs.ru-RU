---
title: Тип ресурса ediscoveryExportOperation
description: Представляет процесс экспорта обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 499f019fa9933522b91d9d0f1aeff518e43ff13b
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946116"
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
|azureBlobContainer|String| Имя расположения хранилища Azure, в котором будет храниться экспорт. Это относится только к экспортам, хранящимся в вашем собственном хранилище Azure. |
|azureBlobToken|String| Маркер SAS для расположения хранилища Azure.  Это относится только к экспортам, хранящимся в вашем собственном хранилище Azure. |
|completedDateTime|DateTimeOffset| Дата и время завершения экспорта.|
|createdBy|[identitySet](../resources/identityset.md)| Пользователь, иницивший операцию экспорта.|
|createdDateTime|DateTimeOffset| Дата и время создания экспорта.|
|description|Строка| Описание, предоставленное для экспорта.|
|exportOptions|microsoft.graph.ediscovery.exportOptions| Параметры, предоставленные для экспорта. Дополнительные сведения см. в [разделе reviewSet: export](../api/security-ediscoveryreviewset-export.md). Возможные значения: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.|
|exportStructure|microsoft.graph.ediscovery.exportFileStructure|Предоставленные параметры, указывающие структуру экспорта. Дополнительные сведения см. в [разделе reviewSet: export](../api/security-ediscoveryreviewset-export.md). Возможные значения: `none`, `directory`, `pst`.|
|id|String| Идентификатор операции. Только для чтения. |
|outputName|Строка| Имя, указанное для экспорта.|
|percentProgress|Int32| Ход выполнения операции.|
|resultInfo|[resultInfo](../resources/resultinfo.md)|Содержит сведения о результатах успешного выполнения и сбоя. Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).|
|status|[microsoft.graph.security.caseOperationStatus](../resources/security-caseoperation.md#caseoperationstatus-values)| Состояние операции обращения. Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

## <a name="relationships"></a>Отношения
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

