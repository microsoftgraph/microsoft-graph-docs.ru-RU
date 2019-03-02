---
title: Тип ресурса Ажедаккаунтспайабле
description: Объект кредиторской задолженности в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 679c24b7ef32ef59b34a5885ea745d8c244376b2
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365908"
---
# <a name="agedaccountspayable-resource-type"></a>Тип ресурса Ажедаккаунтспайабле
Представляет объект Ажедаккаунтспайабле в Dynamics 365 Business Central, в котором отображается срок хранения учетной записи поставщика.

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип  |Описание|
|:---------------|:-------------|:----------|
|[Получение Ажедаккаунтспайабле](../api/dynamics-agedaccountspayable-get.md)|Ажедаккаунтспайабле|Получение объекта Ажедаккаунтспайабле|

## <a name="properties"></a>Свойства
| Свойство      | Тип     |Описание                                 |
|:--------------|:---------|:-------------------------------------------|
|Поставщика       |GUID      |Уникальный идентификатор поставщика.                    |
|Вендорнумбер   |строка    |Указывает номер поставщика.                  |
|name           |строка    |Указывает имя поставщика.                    |
|Курренцикоде   |строка    |Задает валюту.                     |
|Баланцедуе     |числовых   |Указывает общее сальдо, которое связано с поставщиком.|
|Куррентамаунт  |числовых   |Указывает баланс перед первым периодом распределения по срокам.|
|period1Amount  |числовых   |Указывает баланс в первом периоде распределения по срокам.|
|period2Amount  |числовых   |Указывает баланс во втором периоде распределения по срокам.|
|period3Amount  |числовых   |Указывает баланс в третьем периоде распределения по срокам.|
|Ажедасофдате   |дата|Указывает дату начала периода, используемого для вычисления периодов распределения по срокам.|
|Периодленгсфилтер|строка |Указывает длину периодов. Допустимые значения для единиц времени: D, WD, W, M, Q или Y. C, то есть текущая единица времени на основе даты может быть указана в качестве префикса для единицы времени.|


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Описание в формате JSON

Ниже представлено описание ресурса в формате JSON.


```json
{
    "vendorId": "GUID",
    "vendorNumber": "string",
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
