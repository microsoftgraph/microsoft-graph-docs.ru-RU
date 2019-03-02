---
title: Тип ресурса Женералледжерентриес
description: Запись главной книги в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0a5701451bf96773428b12b6bb715320e2ba81b5
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365761"
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
|Постингдате         |дата                   |Указывает дату учета финансовой операции. |
|Документнумбер      |Строка, максимальный размер 20|Указывает номер документа в финансовой операции.|
|documentType        |строка                 |Указывает тип документа для финансовой операции.|
|accountId           |GUID                   |Определяет accountId финансовой операции.    |
|Аккаунтнумбер       |Строка, максимальный размер 20|Указывает Аккаунтнумбер финансовой операции.|
|description         |Строка, максимальный размер 50|Задает описание финансовой операции.  |
|Дебитамаунт         |числовых                |Указывает Дебитамаунт финансовой операции.  |
|Кредитамаунт        |числовых                |Указывает Кредитамаунт финансовой операции. |
|lastModifiedDateTime|отличным               |Дата и время последнего изменения финансовой операции.|


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Описание в формате JSON

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

