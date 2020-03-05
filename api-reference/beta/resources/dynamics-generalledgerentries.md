---
title: Тип ресурса Женералледжерентриес
description: Запись главной книги в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: f1dc4ec7bb3fa30f7dc6362c850893953c4aa6aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503987"
---
# <a name="generalledgerentries-resource-type"></a>Тип ресурса Женералледжерентриес

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объект Женералледжерентри в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:-------------|:-------------|:----------|
|[Получение Женералледжерентриес](../api/dynamics-generalledgerentries-get.md)|женералледжерентриес|Получение объекта финансовой операции.|

## <a name="properties"></a>Свойства
| Свойство           | Тип                  |Описание                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|id                  |числовых                |Уникальный идентификатор финансовой операции.              |
|постингдате         |date                   |Указывает дату учета финансовой операции. |
|документнумбер      |Строка, максимальный размер 20|Указывает номер документа в финансовой операции.|
|documentType        |строка                 |Указывает тип документа для финансовой операции.|
|accountId           |GUID                   |Определяет accountId финансовой операции.    |
|аккаунтнумбер       |Строка, максимальный размер 20|Указывает Аккаунтнумбер финансовой операции.|
|description         |Строка, максимальный размер 50|Задает описание финансовой операции.  |
|дебитамаунт         |числовых                |Указывает Дебитамаунт финансовой операции.  |
|кредитамаунт        |числовых                |Указывает Кредитамаунт финансовой операции. |
|lastModifiedDateTime|datetime               |Дата и время последнего изменения финансовой операции.|


## <a name="relationships"></a>Связи
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

