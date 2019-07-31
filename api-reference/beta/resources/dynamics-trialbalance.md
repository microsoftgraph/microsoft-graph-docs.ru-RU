---
title: Тип ресурса Триалбаланце
description: Объект пробного баланса в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 02e4f039411c992cd1d7335fc2463d660b8ff181
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972875"
---
# <a name="trialbalance-resource-type"></a>Тип ресурса Триалбаланце
Представляет пробный баланс в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение Триалбаланце](../api/dynamics-trialbalance-get.md)|Триалбаланце|Получает объект пробного баланса.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|число|string|Номер финансового счета для элемента Триалбаланце|
|accountId|GUID|Уникальный идентификатор финансового счета записи.|
|accountType|string|Тип учетной записи финансового счета записи.|
|отображения|string|Имя финансового счета для элемента Триалбаланце.|
|Тоталдебит|string|Представляет общую сумму дебета в финансовом счете.|
|Тоталкредит|string|Представляет общую сумму кредита в финансовом счете.|
|Баланцеатдатедебит|string|Представляет положительное сальдо на сумму даты в финансовом счете.|
|Баланцеатдатекредит|string|Представляет отрицательное сальдо на сумму даты в финансовом счете.|
|Датефилтер|date|Фильтр даты, используемый для вычисления элементов Триалбаланце.|


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.


```json
{
    "number": "string",
    "accountId": "GUID",
    "accountType": "string",
    "display": "string",
    "totalDebit": "string",
    "totalCredit": "string",
    "balanceAtDateDebit": "string",
    "balanceAtDateCredit": "string",
    "dateFilter": "date"
}

```

