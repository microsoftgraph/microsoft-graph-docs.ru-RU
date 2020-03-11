---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
description: Ресурс UploadSession предоставляет сведения о том, как отправлять большие файлы в OneDrive, OneDrive для бизнеса или библиотеки документов SharePoint, а также в виде вложений файлов в события и объекты сообщений Outlook.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b2540c1abdd5e40ea960dc3672ab7cc788e08ddd
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590015"
---
# <a name="uploadsession-resource-type"></a>Тип ресурса uploadSession

Пространство имен: microsoft.graph

Ресурс **uploadSession** предоставляет сведения о том, как отправлять большие файлы в OneDrive, Onedrive для бизнеса или библиотеки документов SharePoint, а также [события](event.md) и элементы [сообщений](message.md) Outlook в качестве вложений.

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
| nextExpectedRanges | Коллекция строк | Коллекция диапазонов байтов файла, отсутствующих на сервере. Эти диапазоны имеют нулевую индексацию и формат "начало-конец" (например, "0–26" для указания первых 27 байтов файла). При отправке файлов в виде вложений Outlook вместо коллекции диапазонов это свойство всегда указывает на одно значение "{Start}", расположение в файле, в котором должна начаться следующая загрузка.
| uploadUrl          | Строка            | URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла.

## <a name="see-also"></a>См. также

- [Присоединение больших файлов к сообщениям и событиям Outlook в качестве вложений](/graph/outlook-large-attachments)
- [Отправка больших файлов с помощью сеанса отправки](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
