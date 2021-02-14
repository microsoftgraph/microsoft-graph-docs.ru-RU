---
author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
description: Ресурс UploadSession предоставляет сведения о том, как отправлять большие файлы в OneDrive, OneDrive для бизнеса или в библиотеки документов SharePoint или в виде вложений в объекты событий и сообщений Outlook.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0104b9349427b07ffef570d66b98720155bd7728
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239473"
---
# <a name="uploadsession-resource-type"></a>Тип ресурса uploadSession

Пространство имен: microsoft.graph

Ресурс **uploadSession** предоставляет сведения о том, как отправлять большие файлы в OneDrive, OneDrive для [](message.md) бизнеса или в библиотеки документов SharePoint, а также в элементы событий [и](event.md) сообщений Outlook в виде вложений.

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
| nextExpectedRanges | Коллекция строк | Коллекция диапазонов байтов файла, отсутствующих на сервере. Эти диапазоны имеют нулевую индексацию и формат "начало-конец" (например, "0–26" для указания первых 27 байтов файла). При отправке файлов в виде вложений Outlook, а не коллекции диапазонов, это свойство всегда указывает одно значение "{start}", расположение в файле, где должна начаться следующая отправка.
| uploadUrl          | Строка            | URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла.

## <a name="see-also"></a>См. также

- [Вложение больших файлов в сообщения и события Outlook в виде вложений ](/graph/outlook-large-attachments)
- [Отправка больших файлов с помощью сеанса отправки](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->

