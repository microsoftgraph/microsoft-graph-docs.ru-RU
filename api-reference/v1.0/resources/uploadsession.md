---
author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
description: Ресурс UploadSession предоставляет сведения о том, как загружать большие файлы в библиотеки OneDrive, OneDrive для бизнеса или SharePoint или в виде вложений файлов в Outlook объекты событий и сообщений.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 08401209a720aeead1ce23d13179aabedd26320952ca0fa34aba878373ef218f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235270"
---
# <a name="uploadsession-resource-type"></a>тип ресурса uploadSession

Пространство имен: microsoft.graph

Ресурс **uploadSession** предоставляет сведения о том, как загружать большие файлы в библиотеки OneDrive, OneDrive для бизнеса или SharePoint документов, [](event.md) а [](message.md) также Outlook событий и сообщений в виде вложений.

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
| nextExpectedRanges | Коллекция строк | Коллекция диапазонов байтов файла, отсутствующих на сервере. Эти диапазоны имеют нулевую индексацию и формат "начало-конец" (например, "0–26" для указания первых 27 байтов файла). При загрузке файлов Outlook вложения вместо коллекции диапазонов это свойство всегда указывает одно значение "{start}", расположение в файле, где должна начаться следующая загрузка.
| uploadUrl          | Строка            | URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла.

## <a name="see-also"></a>См. также

- [Присоединение больших файлов к Outlook и событиям в качестве вложений](/graph/outlook-large-attachments)
- [Отправка больших файлов с помощью сеанса отправки](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->

