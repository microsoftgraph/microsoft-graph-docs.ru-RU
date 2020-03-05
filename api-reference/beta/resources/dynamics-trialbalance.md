---
title: Тип ресурса Триалбаланце
description: Объект пробного баланса в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: b7d3fee76df5f60c47639183f7d3e7ce54164f81
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503217"
---
# <a name="trialbalance-resource-type"></a>Тип ресурса Триалбаланце

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пробный баланс в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение Триалбаланце](../api/dynamics-trialbalance-get.md)|триалбаланце|Получает объект пробного баланса.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|число|строка|Номер финансового счета для элемента Триалбаланце|
|accountId|GUID|Уникальный идентификатор финансового счета записи.|
|accountType|строка|Тип учетной записи финансового счета записи.|
|отображения|строка|Имя финансового счета для элемента Триалбаланце.|
|тоталдебит|строка|Представляет общую сумму дебета в финансовом счете.|
|тоталкредит|строка|Представляет общую сумму кредита в финансовом счете.|
|баланцеатдатедебит|строка|Представляет положительное сальдо на сумму даты в финансовом счете.|
|баланцеатдатекредит|строка|Представляет отрицательное сальдо на сумму даты в финансовом счете.|
|датефилтер|date|Фильтр даты, используемый для вычисления элементов Триалбаланце.|


## <a name="relationships"></a>Связи
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

