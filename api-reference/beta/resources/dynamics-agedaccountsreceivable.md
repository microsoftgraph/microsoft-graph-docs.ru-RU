---
title: Тип ресурса Ажедаккаунтсрецеивабле
description: Объект устаревших расчетов с клиентами в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: f9589cbb4cb380eececdcc7adf7bd5dd682269f6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012676"
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
|Кустомернумбер  |string   |Указывает номер клиента.                 |
|name            |string   |Указывает имя клиента.                   |
|Курренцикоде    |string   |Задает валюту.                      |
|Баланцедуе      |числовых  |Указывает общее сальдо клиента.      |
|Куррентамаунт   |числовых  |Указывает баланс для текущего периода распределения по срокам.|
|period1Amount   |числовых  |Указывает баланс в первом периоде распределения по срокам. |
|period2Amount   |числовых  |Указывает баланс во втором периоде распределения по срокам.|
|period3Amount   |числовых  |Указывает баланс в третьем периоде распределения по срокам. |
|Ажедасофдате    |date     |Указывает дату начала периода, используемого для вычисления периодов распределения по срокам.|
|Периодленгсфилтер|string |Указывает длину периодов. Допустимые единицы времени: D, WD, W, M, Q и Y. C, то есть текущая единица времени на основе даты может указываться в качестве префикса для единицы времени.|


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

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


