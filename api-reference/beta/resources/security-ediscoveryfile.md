---
title: Тип ресурса ediscoveryFile
description: Представляет файл обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 6e952dcc8299b43817fca48beb4a705c522d12f4
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946108"
---
# <a name="ediscoveryfile-resource-type"></a>Тип ресурса ediscoveryFile

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сущность, представляющая файлы ediscovery ReviewSet.
## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление файлов ediscoveryFiles](../api/security-ediscoveryreviewset-list-files.md)|[Коллекция microsoft.graph.security.ediscoveryFile](../resources/security-ediscoveryfile.md)|Получение списка объектов [ediscoveryFile](../resources/security-ediscoveryfile.md) и их свойств.|
|[Получение ediscoveryFile](../api/security-ediscoveryfile-get.md)|[microsoft.graph.security.ediscoveryFile](../resources/security-ediscoveryfile.md)|Чтение свойств и связей объекта [ediscoveryFile](../resources/security-ediscoveryfile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|содержимое|Поток|Поток содержимого исходного файла.|
|dateTime|DateTimeOffset|Дата и время последнего изменения файла. Дополнительные сведения см. в разделе значений dateTime.|
|Расширение|Строка|Расширение файла, например png, msg, docx и т. д.|
|extractedTextContent|Stream|Извлеченный текст из исходного файла. Для файлов на основе изображений это будет текст OCR.|
|id|String|Уникальный идентификатор файла.|
|MediaType|String|mimeType файла. Например: text/plain, charset=UTF-8, application/vnd.ms-outlook.|
|name|String|Имя файла Тема сообщения в случае сообщения электронной почты.|
|otherProperties|Строка|Список дополнительных свойств файла, таких как titleOfSharepointDocument, emailRecipients. [Подробнее](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).|
|processingStatus|Строка|Состояние обработки после добавления элемента в набор для проверки. Возможные значения: `success`, , `internalError`, `unknownError`, `processingTimeout`, `invalidFileId`, `fileSizeIsZero`, `fileSizeIsTooLarge``fileDepthLimitExceeded`, `fileBodyIsTooLong`, `fileTypeIsUnknown`, `fileTypeIsNotSupported`, `malformedFile`, `protectedFile`, `poisonFile`, , `noReviewSetSummaryGenerated`, . `ocrProcessingTimeout``ocrFileSizeExceedsLimit``extractionException`|
|senderAuthor|Коллекция строк|Отправитель сообщения электронной почты или авторов документа.|
|size|Int64|размер файла.|
|Sourcetype|Строка|Исходный источник содержимого. Возможные значения: `mailbox`, `site`.|
|subjectTitle|Строка|Тема сообщения электронной почты или заголовка документа|

### <a name="datetime-values"></a>Значения dateTime
|Тип файла|Определение|
|:---|:---|
Электронная почта |Дата отправки.
Вложения электронной почты | Дата последнего изменения документа; если она недоступна, дата отправки родительского элемента.
Embedded documents | Дата последнего изменения документа; Значение , если оно недоступно, дата последнего изменения родительского элемента.
Документы SPO (включая современные вложения) | Дата последнего изменения SharePoint; Если он недоступен, дата последнего изменения документов.
Документы, отличные от Office 365 | Дата последнего изменения.
Собрания | Дата начала собрания.
Голосовую почту | Дата отправки.
"IM" (Обмен мгновенными сообщениями); |Дата отправки.
## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|Хранителя|[microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|Хранители, связанные с файлом.|
|tags|[Коллекция microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|Теги, связанные с файлом.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryFile",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryFile",
  "id": "String (identifier)",
  "dateTime": "String (timestamp)",
  "size": "Integer",
  "name": "String",
  "sourceType": "String",
  "senderAuthor": [
    "String"
  ],
  "subjectTitle": "String",
  "extension": "String",
  "mediaType": "String",
  "content": "Stream",
  "extractedTextContent": "Stream",
  "processingStatus": "String",
  "otherProperties": {
    "@odata.type": "microsoft.graph.security.stringValueDictionary"
  }
}
```

