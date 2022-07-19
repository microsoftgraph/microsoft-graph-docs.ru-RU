---
title: Тип ресурса ediscoveryFile
description: Представляет файл обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c47688daed5d5113c6b51fe096a06b93e78a8ae0
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66837368"
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
|Расширение|String|Расширение файла, например png, msg, docx и т. д.|
|extractedTextContent|Stream|Извлеченный текст из исходного файла. Для файлов на основе изображений это будет текст OCR.|
|id|Строка|Уникальный идентификатор файла.|
|MediaType|Строка|mimeType файла. Например: text/plain, charset=UTF-8, application/vnd.ms-outlook.|
|name|String|Имя файла Тема сообщения в случае сообщения электронной почты.|
|otherProperties|microsoft.graph.security.stringValueDictionary|Список дополнительных свойств файла, таких как titleOfSharepointDocument, emailRecipients. [Подробнее](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).|
|processingStatus|microsoft.graph.security.fileProcessingStatus|Состояние обработки после добавления элемента в набор для проверки. Возможные значения: `success`, , `internalError`, `unknownError`, `processingTimeout`, `invalidFileId`, `fileSizeIsZero`, `fileSizeIsTooLarge``fileDepthLimitExceeded`, `fileBodyIsTooLong`, `fileTypeIsUnknown`, `fileTypeIsNotSupported`, `malformedFile`, `protectedFile`, `poisonFile`, , `noReviewSetSummaryGenerated`, . `ocrProcessingTimeout``ocrFileSizeExceedsLimit``extractionException`|
|senderAuthor|Коллекция строк|Отправитель сообщения электронной почты или авторов документа.|
|size|Int64|размер файла.|
|Sourcetype|microsoft.graph.security.sourceType|Исходный источник содержимого. Возможные значения: `mailbox`, `site`.|
|subjectTitle|String|Тема сообщения электронной почты или заголовка документа|

### <a name="fileprocessingstatus-values"></a>Значения fileProcessingStatus

|Member|Описание|
|:----|-----------|
|success|   Файл успешно обработан.|
|internalError| Во время обработки файла возникло необработанное исключение.|
|unknownError|Состояние обработки равно NULL или пусто.|
|processingTimeout|Истекло время ожидания во время обработки.|
|invalidFileId|Не удалось создать уникальный идентификатор поля для файла.|
|fileSizeIsZero|Размер файла равен нулю или отрицательному значению.|
|fileSizeIsTooLarge|Размер файла превышает ограничения для обработки.|
|fileDepthLimitExceeded|Глубина файла превысила предел обработки (30).|
|fileBodyIsTooLong|Длина текста в документе превышает предел обработки.|
|fileTypeIsUnknown| MimeType не поддерживается.|
|fileTypeIsNotSupported| Формат файла не поддерживается.|
|malformedFile|Файл имеет неправильный формат.|
|protectedFile|Сообщение электронной почты защищено правами или документ зашифрован.|
|poisonFile|Файл уже обработан.|
|noReviewSetSummaryGenerated|Сбой создания сводки по набору проверки.|
|extractionException|Не удалось выполнить извлечение внедренных документов.|
|ocrProcessingTimeout|Время ожидания при ocrProcessing файла.|
|ocrFileSizeExceedsLimit|Размер файла превышает ограничения для обработки OCR.|


### <a name="datetime-values"></a>Значения dateTime
|Тип файла|Определение|
|:---|:---|
Электронная почта |Дата отправки.
Вложения электронной почты | Дата последнего изменения документа; если она недоступна, дата отправки родительского элемента.
Embedded documents | Дата последнего изменения документа; Значение , если оно недоступно, дата последнего изменения родительского элемента.
Документы SPO (включая современные вложения) | Дата последнего изменения SharePoint; Если он недоступен, дата последнего изменения документов.
Документы, не Office 365 | Дата последнего изменения.
Собрания | Дата начала собрания.
Голосовую почту | Дата отправки.
"IM" (Обмен мгновенными сообщениями); |Дата отправки.
## <a name="relationships"></a>Связи
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

