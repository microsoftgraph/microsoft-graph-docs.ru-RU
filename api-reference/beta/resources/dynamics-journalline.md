---
title: Тип ресурса Жаурналлинес
description: Строка журнала в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 99d06b5a49bd2881ea6f329e8b0d3692a25444b4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013799"
---
# <a name="journallines-resource-type"></a>Тип ресурса Жаурналлинес

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет строку в журнале в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод                                                    | Возвращаемый тип|Описание         |
|:----------------------------------------------------------|:-----------|:-------------------|
|[Получение Жаурналлинес](../api/dynamics-journalline-get.md)      |жаурналлинес|Получает строку журнала.   |
|[POST Жаурналлинес](../api/dynamics-create-journalline.md)  |жаурналлинес|Создает строку журнала.|
|[Исправление Жаурналлинес](../api/dynamics-journalline-update.md) |жаурналлинес|Обновляет строку журнала.|
|[Удаление Жаурналлинес](../api/dynamics-journalline-delete.md)|Нет        |Удаляет строку журнала.|

## <a name="properties"></a>Свойства
| Свойство             | Тип                   |Описание                                                        |
|:---------------------|:-----------------------|:------------------------------------------------------------------|
|id                    |GUID                    |Уникальный идентификатор строки журнала. Не редактируемые.                   |
|жаурналдисплайнаме    |Строка, максимальный размер 10 |Отображаемое имя журнала, к которому относится эта строка. Только для чтения.|
|lineNumber            |целое                 |Номер строки журнала.                                    |
|accountId             |GUID                    |Уникальный идентификатор учетной записи, с которой связана строка журнала.  |
|аккаунтнумбер         |Строка, максимальный размер 20 |Номер учетной записи, с которой связана строка журнала.     |
|постингдате           |date                    |Дата, когда строка журнала разносится.                          |
|документнумбер        |Строка, максимальный размер 20 |Указывает номер документа для строки журнала.                  |
|екстерналдокументнумбер|Строка, максимальный размер 20 |Указывает номер внешнего документа для строки журнала.        |
|отступ                |числе                 |Указывает общую сумму (включая НДС), из которой состоит строка журнала.|
|description           |Строка, максимальный размер 50 |Описание строки журнала, предоставленное пользователем или созданным пользователем.|
|comment               |Строка, максимальный размер 250|Заданный пользователем комментарий в строке журнала.                      |
|lastModifiedDateTime  |datetime                |Дата и время последнего изменения строки журнала. Только для чтения.        |

## <a name="relationships"></a>Связи
Строка журнала является вложенной страницей журнала. Прямой доступ к нему невозможен.

Строка журнала может быть "родительским объектом" для строк измерения.

Учетная запись (accountId) должна существовать в таблице Accounts.


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.


```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "accountId": "GUID",
    "accountNumber": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```


