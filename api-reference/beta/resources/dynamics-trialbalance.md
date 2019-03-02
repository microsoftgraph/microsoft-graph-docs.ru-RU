---
title: Тип ресурса Триалбаланце
description: Объект пробного баланса в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1a7e906e50ddf39e4c9e2d3d9dde11226c7ec662
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365327"
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
|number|строка|Номер финансового счета для элемента Триалбаланце|
|accountId|GUID|Уникальный идентификатор финансового счета записи.|
|accountType|строка|Тип учетной записи финансового счета записи.|
|отображения|строка|Имя финансового счета для элемента Триалбаланце.|
|Тоталдебит|строка|Представляет общую сумму дебета в финансовом счете.|
|Тоталкредит|строка|Представляет общую сумму кредита в финансовом счете.|
|Баланцеатдатедебит|строка|Представляет положительное сальдо на сумму даты в финансовом счете.|
|Баланцеатдатекредит|строка|Представляет отрицательное сальдо на сумму даты в финансовом счете.|
|Датефилтер|дата|Фильтр даты, используемый для вычисления элементов Триалбаланце.|


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Описание в формате JSON

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

