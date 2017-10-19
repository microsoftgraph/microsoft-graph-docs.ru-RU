---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: UploadSession
ms.openlocfilehash: d84b588c28791ab8f1cf6cef1be6af767fa18e47
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="uploadsession-resource"></a>Ресурс UploadSession

Ресурс **UploadSession** предоставляет сведения о том, как отправлять большие файлы в OneDrive, OneDrive для бизнеса или библиотеки документов SharePoint.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession"
}-->

```json
{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["0-"]
}
```

## <a name="properties"></a>Свойства


| Свойство       | Тип              |Описание
|:-------------------|:------------------|:------------------------------------
| expirationDateTime | DateTimeOffset    | Дата и время (в формате UTC) истечения срока действия сеанса. Полный файл необходимо отправить до наступления этого момента.
| nextExpectedRanges | Коллекция строк | Коллекция диапазонов байтов файла, отсутствующих на сервере. Эти диапазоны имеют нулевую индексацию и формат "начало-конец" (например, "0–26" для указания первых 27 байтов файла).
| uploadUrl          | Строка            | URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла.

## <a name="additional-resources"></a>Дополнительные ресурсы

Сведения о том, как отправлять файлы с помощью сеанса отправки, см. в статье [Отправка больших файлов с помощью сеанса отправки](../api/driveitem_createuploadsession.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
