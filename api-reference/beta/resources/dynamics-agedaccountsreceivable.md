---
title: Тип ресурса Ажедаккаунтсрецеивабле
description: Объект устаревших расчетов с клиентами в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ce5d010c08f956468398082821040e30b4ef2ace
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365579"
---
# <a name="agedaccountsreceivable-resource-type"></a>Тип ресурса Ажедаккаунтсрецеивабле
Представляет объект Ажедаккаунтсрецеивабле в Dynamics 365 Business Central, в котором отображается срок хранения учетной записи клиента.

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип  |Описание|
|:---------------|:-------------|:----------|
|[Получение Ажедаккаунтсрецеивабле](../api/dynamics-agedaccountsreceivable-get.md)|Ажедаккаунтсрецеивабле|Получение объекта Ажедаккаунтсрецеивабле|

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание                                  |
|:---------------|:--------|:--------------------------------------------|
|customerId      |GUID     |Уникальный идентификатор клиента.                   |
|Кустомернумбер  |строка   |Указывает номер клиента.                 |
|name            |строка   |Указывает имя клиента.                   |
|Курренцикоде    |строка   |Задает валюту.                      |
|Баланцедуе      |числовых  |Указывает общее сальдо клиента.      |
|Куррентамаунт   |числовых  |Указывает баланс для текущего периода распределения по срокам.|
|period1Amount   |числовых  |Указывает баланс в первом периоде распределения по срокам. |
|period2Amount   |числовых  |Указывает баланс во втором периоде распределения по срокам.|
|period3Amount   |числовых  |Указывает баланс в третьем периоде распределения по срокам. |
|Ажедасофдате    |дата     |Указывает дату начала периода, используемого для вычисления периодов распределения по срокам.|
|Периодленгсфилтер|строка |Указывает длину периодов. Допустимые единицы времени: D, WD, W, M, Q и Y. C, то есть текущая единица времени на основе даты может указываться в качестве префикса для единицы времени.|


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Описание в формате JSON

Ниже представлено описание ресурса в формате JSON.


```json
{
    "customerId": "GUID",
    "customerNumber": "string",
    "name": "string",
    "currencyCode": "string",
    "balanceDue": "decimal",
    "currentAmount": "decimal",
    "period1Amount": "decimal",
    "period2Amount": "decimal",
    "period3Amount": "decimal",
    "agedAsOfDate": "date",
    "periodLengthFilter": "string"
}

```


