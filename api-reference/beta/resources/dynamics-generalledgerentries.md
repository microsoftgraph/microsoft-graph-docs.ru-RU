---
title: Тип ресурса Женералледжерентриес
description: Запись главной книги в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 500c78d0e29d83c68c2b7247a9787b977cc8a7b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973606"
---
# <a name="generalledgerentries-resource-type"></a>Тип ресурса Женералледжерентриес
Представляет объект Женералледжерентри в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:-------------|:-------------|:----------|
|[Получение Женералледжерентриес](../api/dynamics-generalledgerentries-get.md)|Женералледжерентриес|Получение объекта финансовой операции.|

## <a name="properties"></a>Свойства
| Свойство           | Тип                  |Описание                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|id                  |числовых                |Уникальный идентификатор финансовой операции.              |
|Постингдате         |date                   |Указывает дату учета финансовой операции. |
|Документнумбер      |Строка, максимальный размер 20|Указывает номер документа в финансовой операции.|
|documentType        |string                 |Указывает тип документа для финансовой операции.|
|accountId           |GUID                   |Определяет accountId финансовой операции.    |
|Аккаунтнумбер       |Строка, максимальный размер 20|Указывает Аккаунтнумбер финансовой операции.|
|description         |Строка, максимальный размер 50|Задает описание финансовой операции.  |
|Дебитамаунт         |числовых                |Указывает Дебитамаунт финансовой операции.  |
|Кредитамаунт        |числовых                |Указывает Кредитамаунт финансовой операции. |
|lastModifiedDateTime|отличным               |Дата и время последнего изменения финансовой операции.|


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.


```json
{
  "id": "int",
  "postingDate": "Date",
  "documentNumber": "string",
  "documentType": "string",
  "accountId": "GUID",
  "accountNumber": "string",
  "description": "string",
  "debitAmount": "decimal",
  "creditAmount": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

