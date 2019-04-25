---
title: Тип ресурса Триалбаланце
description: Объект пробного баланса в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1a7e906e50ddf39e4c9e2d3d9dde11226c7ec662
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534852"
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
|accountId|Глобальный уникальный идентификатор (GUID)|Уникальный идентификатор финансового счета записи.|
|accountType|string|Тип учетной записи финансового счета записи.|
|отображения|string|Имя финансового счета для элемента Триалбаланце.|
|Тоталдебит|string|Представляет общую сумму дебета в финансовом счете.|
|Тоталкредит|string|Представляет общую сумму кредита в финансовом счете.|
|Баланцеатдатедебит|string|Представляет положительное сальдо на сумму даты в финансовом счете.|
|Баланцеатдатекредит|string|Представляет отрицательное сальдо на сумму даты в финансовом счете.|
|Датефилтер|дата|Фильтр даты, используемый для вычисления элементов Триалбаланце.|


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление в формате JSON

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

